

# File triplet\_matrix\_view.h

[**File List**](files.md) **>** [**ext**](dir_dee31a662aa40cb7fc08cb07824f4a9a.md) **>** [**linear\_system**](dir_6f09a74f7ee1db37d591c4a0fc2f2223.md) **>** [**triplet\_matrix\_view.h**](triplet__matrix__view_8h.md)

[Go to the documentation of this file](triplet__matrix__view_8h.md)


```C++
#pragma once
#include <muda/buffer/buffer_view.h>
#include <muda/ext/linear_system/triplet_matrix_viewer.h>
#include <muda/view/view_base.h>

namespace muda
{
template <bool IsConst, typename Ty, int N>
class TripletMatrixViewT : public ViewBase<IsConst>
{
    using Base = ViewBase<IsConst>;
    template <typename U>
    using auto_const_t = typename Base::template auto_const_t<U>;

    template <bool OtherIsConst, typename U, int M>
    friend class TripletMatrixViewT;

  public:
    static_assert(!std::is_const_v<Ty>, "Ty must be non-const");
    using ConstView    = TripletMatrixViewT<true, Ty, N>;
    using NonConstView = TripletMatrixViewT<false, Ty, N>;
    using ThisView     = TripletMatrixViewT<IsConst, Ty, N>;

  private:
    using ConstViewer    = CTripletMatrixViewer<Ty, N>;
    using NonConstViewer = TripletMatrixViewer<Ty, N>;
    using ThisViewer = std::conditional_t<IsConst, ConstViewer, NonConstViewer>;

  public:
    using BlockMatrix = Eigen::Matrix<Ty, N, N>;

  protected:
    // matrix info
    int m_total_block_rows = 0;
    int m_total_block_cols = 0;

    // triplet info
    int m_triplet_index_offset = 0;
    int m_triplet_count        = 0;
    int m_total_triplet_count  = 0;

    // sub matrix info
    int2 m_submatrix_offset = {0, 0};
    int2 m_submatrix_extent = {0, 0};

    // data
    auto_const_t<int>*         m_block_row_indices = nullptr;
    auto_const_t<int>*         m_block_col_indices = nullptr;
    auto_const_t<BlockMatrix>* m_block_values      = nullptr;

  public:
    MUDA_GENERIC TripletMatrixViewT() = default;
    MUDA_GENERIC TripletMatrixViewT(int total_block_rows,
                                    int total_block_cols,

                                    int triplet_index_offset,
                                    int triplet_count,
                                    int total_triplet_count,

                                    int2 submatrix_offset,
                                    int2 submatrix_extent,

                                    auto_const_t<int>* block_row_indices,
                                    auto_const_t<int>* block_col_indices,
                                    auto_const_t<BlockMatrix>* block_values)
        : m_total_block_rows(total_block_rows)
        , m_total_block_cols(total_block_cols)
        , m_triplet_index_offset(triplet_index_offset)
        , m_triplet_count(triplet_count)
        , m_total_triplet_count(total_triplet_count)
        , m_block_row_indices(block_row_indices)
        , m_block_col_indices(block_col_indices)
        , m_block_values(block_values)
        , m_submatrix_offset(submatrix_offset)
        , m_submatrix_extent(submatrix_extent)
    {
        MUDA_KERNEL_ASSERT(triplet_index_offset + triplet_count <= total_triplet_count,
                           "TripletMatrixView: out of range, m_total_triplet_count=%d, "
                           "your triplet_index_offset=%d, triplet_count=%d",
                           total_triplet_count,
                           triplet_index_offset,
                           triplet_count);

        MUDA_KERNEL_ASSERT(submatrix_offset.x >= 0 && submatrix_offset.y >= 0,
                           "TripletMatrixView: submatrix_offset is out of range, submatrix_offset.x=%d, submatrix_offset.y=%d",
                           submatrix_offset.x,
                           submatrix_offset.y);

        MUDA_KERNEL_ASSERT(submatrix_offset.x + submatrix_extent.x <= total_block_rows,
                           "TripletMatrixView: submatrix is out of range, submatrix_offset.x=%d, submatrix_extent.x=%d, total_block_rows=%d",
                           submatrix_offset.x,
                           submatrix_extent.x,
                           total_block_rows);

        MUDA_KERNEL_ASSERT(submatrix_offset.y + submatrix_extent.y <= total_block_cols,
                           "TripletMatrixView: submatrix is out of range, submatrix_offset.y=%d, submatrix_extent.y=%d, total_block_cols=%d",
                           submatrix_offset.y,
                           submatrix_extent.y,
                           total_block_cols);
    }

    MUDA_GENERIC TripletMatrixViewT(int                total_block_rows,
                                    int                total_block_cols,
                                    int                total_triplet_count,
                                    auto_const_t<int>* block_row_indices,
                                    auto_const_t<int>* block_col_indices,
                                    auto_const_t<BlockMatrix>* block_values)
        : TripletMatrixViewT(total_block_rows,
                             total_block_cols,
                             0,
                             total_triplet_count,
                             total_triplet_count,
                             {0, 0},
                             {total_block_rows, total_block_cols},
                             block_row_indices,
                             block_col_indices,
                             block_values)
    {
    }

    template <bool OtherIsConst>
    MUDA_GENERIC TripletMatrixViewT(const TripletMatrixViewT<OtherIsConst, Ty, N>& other) MUDA_NOEXCEPT
        MUDA_REQUIRES(IsConst)
        : m_total_block_rows(other.m_total_block_rows)
        , m_total_block_cols(other.m_total_block_cols)
        , m_triplet_index_offset(other.m_triplet_index_offset)
        , m_triplet_count(other.m_triplet_count)
        , m_total_triplet_count(other.m_total_triplet_count)
        , m_submatrix_offset(other.m_submatrix_offset)
        , m_submatrix_extent(other.m_submatrix_extent)
        , m_block_row_indices(other.m_block_row_indices)
        , m_block_col_indices(other.m_block_col_indices)
        , m_block_values(other.m_block_values)
    {
        static_assert(IsConst);
    }

    MUDA_GENERIC ConstView as_const() const
    {
        return ConstView{m_total_block_rows,
                         m_total_block_cols,
                         m_triplet_index_offset,
                         m_triplet_count,
                         m_total_triplet_count,
                         m_submatrix_offset,
                         m_submatrix_extent,
                         m_block_row_indices,
                         m_block_col_indices,
                         m_block_values};
    }

    MUDA_GENERIC auto subview(int offset, int count) const
    {
        MUDA_ASSERT(offset + count <= m_triplet_count,
                    "TripletMatrixView: offset is out of range, size=%d, your offset=%d, your count=%d",
                    m_triplet_count,
                    offset,
                    count);

        return ThisView{m_total_block_rows,
                        m_total_block_cols,
                        m_triplet_index_offset + offset,
                        count,
                        m_total_triplet_count,
                        m_submatrix_offset,
                        m_submatrix_extent,
                        m_block_row_indices,
                        m_block_col_indices,
                        m_block_values};
    }

    MUDA_GENERIC auto subview(int offset) const
    {
        return subview(offset, m_triplet_count - offset);
    }

    MUDA_GENERIC auto cviewer() const
    {
        return ConstViewer{m_total_block_rows,
                           m_total_block_cols,
                           m_triplet_index_offset,
                           m_triplet_count,
                           m_total_triplet_count,
                           m_submatrix_offset,
                           m_submatrix_extent,
                           m_block_row_indices,
                           m_block_col_indices,
                           m_block_values};
    }

    MUDA_GENERIC auto viewer() const
    {
        return ThisViewer{m_total_block_rows,
                          m_total_block_cols,
                          m_triplet_index_offset,
                          m_triplet_count,
                          m_total_triplet_count,
                          m_submatrix_offset,
                          m_submatrix_extent,
                          m_block_row_indices,
                          m_block_col_indices,
                          m_block_values};
    }

    MUDA_GENERIC auto submatrix(int2 offset, int2 extent) const
    {
        MUDA_KERNEL_ASSERT(offset.x >= 0 && offset.y >= 0,
                           "TripletMatrixView: submatrix is out of range, offset=(%d, %d)",
                           offset.x,
                           offset.y);

        MUDA_KERNEL_ASSERT(offset.x + extent.x <= m_submatrix_extent.x
                               && offset.y + extent.y <= m_submatrix_extent.y,
                           "TripletMatrixView: submatrix is out of range, offset=(%d, %d), extent=(%d, %d), origin offset=(%d,%d), extent(%d,%d).",
                           offset.x,
                           offset.y,
                           extent.x,
                           extent.y,
                           m_submatrix_offset.x,
                           m_submatrix_offset.y,
                           m_submatrix_extent.x,
                           m_submatrix_extent.y);

        return ThisView{m_total_block_rows,
                        m_total_block_cols,
                        m_triplet_index_offset,
                        m_triplet_count,
                        m_total_triplet_count,
                        m_submatrix_offset + offset,
                        extent,
                        m_block_row_indices,
                        m_block_col_indices,
                        m_block_values};
    }

    MUDA_GENERIC auto total_block_rows() const { return m_total_block_rows; }
    MUDA_GENERIC auto total_block_cols() const { return m_total_block_cols; }
    MUDA_GENERIC auto total_extent() const
    {
        return int2{m_total_block_rows, m_total_block_cols};
    }

    MUDA_GENERIC auto submatrix_offset() const { return m_submatrix_offset; }
    MUDA_GENERIC auto extent() const { return m_submatrix_extent; }

    MUDA_GENERIC auto triplet_count() const { return m_triplet_count; }
    MUDA_GENERIC auto tripet_index_offset() const
    {
        return m_triplet_index_offset;
    }
    MUDA_GENERIC auto total_triplet_count() const
    {
        return m_total_triplet_count;
    }
};

template <bool IsConst, typename Ty>
class TripletMatrixViewT<IsConst, Ty, 1> : public ViewBase<IsConst>
{
    using Base = ViewBase<IsConst>;

  protected:
    template <typename U>
    using auto_const_t = typename Base::template auto_const_t<U>;

    template <bool OtherIsConst, typename U, int M>
    friend class TripletMatrixViewT;

  public:
    static_assert(!std::is_const_v<Ty>, "Ty must be non-const");
    using ConstView    = TripletMatrixViewT<true, Ty, 1>;
    using NonConstView = TripletMatrixViewT<false, Ty, 1>;
    using ThisView     = TripletMatrixViewT<IsConst, Ty, 1>;

  private:
    using ConstViewer    = CTripletMatrixViewer<Ty, 1>;
    using NonConstViewer = TripletMatrixViewer<Ty, 1>;
    using ThisViewer = std::conditional_t<IsConst, ConstViewer, NonConstViewer>;

  protected:
    // matrix info
    int m_total_rows = 0;
    int m_total_cols = 0;

    // triplet info
    int m_triplet_index_offset = 0;
    int m_triplet_count        = 0;
    int m_total_triplet_count  = 0;

    // sub matrix info
    int2 m_submatrix_offset = {0, 0};
    int2 m_submatrix_extent = {0, 0};

    // data
    auto_const_t<int>* m_row_indices;
    auto_const_t<int>* m_col_indices;
    auto_const_t<Ty>*  m_values;


  public:
    MUDA_GENERIC TripletMatrixViewT() = default;

    MUDA_GENERIC TripletMatrixViewT(int total_rows,
                                    int total_cols,
                                    int triplet_index_offset,
                                    int triplet_count,
                                    int total_triplet_count,

                                    int2 submatrix_offset,
                                    int2 submatrix_extent,

                                    auto_const_t<int>* row_indices,
                                    auto_const_t<int>* col_indices,
                                    auto_const_t<Ty>*  values)
        : m_total_rows(total_rows)
        , m_total_cols(total_cols)
        , m_triplet_index_offset(triplet_index_offset)
        , m_triplet_count(triplet_count)
        , m_total_triplet_count(total_triplet_count)
        , m_submatrix_offset(submatrix_offset)
        , m_submatrix_extent(submatrix_extent)
        , m_row_indices(row_indices)
        , m_col_indices(col_indices)
        , m_values(values)
    {
        MUDA_KERNEL_ASSERT(triplet_index_offset + triplet_count <= total_triplet_count,
                           "TripletMatrixView: out of range, m_total_triplet_count=%d, "
                           "your triplet_index_offset=%d, triplet_count=%d",
                           total_triplet_count,
                           triplet_index_offset,
                           triplet_count);

        MUDA_KERNEL_ASSERT(submatrix_offset.x >= 0 && submatrix_offset.y >= 0,
                           "TripletMatrixView: submatrix_offset is out of range, submatrix_offset.x=%d, submatrix_offset.y=%d",
                           submatrix_offset.x,
                           submatrix_offset.y);

        MUDA_KERNEL_ASSERT(submatrix_offset.x + submatrix_extent.x <= total_rows,
                           "TripletMatrixView: submatrix is out of range, submatrix_offset.x=%d, submatrix_extent.x=%d, total_rows=%d",
                           submatrix_offset.x,
                           submatrix_extent.x,
                           total_rows);

        MUDA_KERNEL_ASSERT(submatrix_offset.y + submatrix_extent.y <= total_cols,
                           "TripletMatrixView: submatrix is out of range, submatrix_offset.y=%d, submatrix_extent.y=%d, total_cols=%d",
                           submatrix_offset.y,
                           submatrix_extent.y,
                           total_cols);
    }

    MUDA_GENERIC TripletMatrixViewT(int                total_rows,
                                    int                total_cols,
                                    int                total_triplet_count,
                                    auto_const_t<int>* row_indices,
                                    auto_const_t<int>* col_indices,
                                    auto_const_t<Ty>*  values)
        : TripletMatrixViewT(total_rows,
                             total_cols,
                             0,
                             total_triplet_count,
                             total_triplet_count,
                             {0, 0},
                             {total_rows, total_cols},
                             row_indices,
                             col_indices,
                             values)
    {
    }

    template <bool OtherIsConst>
    MUDA_GENERIC TripletMatrixViewT(const TripletMatrixViewT<OtherIsConst, Ty, 1>& other) MUDA_NOEXCEPT
        MUDA_REQUIRES(IsConst)
        : m_total_rows(other.m_total_rows)
        , m_total_cols(other.m_total_cols)
        , m_triplet_index_offset(other.m_triplet_index_offset)
        , m_triplet_count(other.m_triplet_count)
        , m_total_triplet_count(other.m_total_triplet_count)
        , m_submatrix_offset(other.m_submatrix_offset)
        , m_submatrix_extent(other.m_submatrix_extent)
        , m_row_indices(other.m_row_indices)
        , m_col_indices(other.m_col_indices)
        , m_values(other.m_values)
    {
        static_assert(IsConst);
    }

    MUDA_GENERIC ConstView as_const() const
    {
        return ConstView{m_total_rows,
                         m_total_cols,
                         m_triplet_index_offset,
                         m_triplet_count,
                         m_total_triplet_count,
                         m_submatrix_offset,
                         m_submatrix_extent,
                         m_row_indices,
                         m_col_indices,
                         m_values};
    }

    MUDA_GENERIC auto subview(int offset, int count) const
    {
        MUDA_ASSERT(offset + count <= m_triplet_count,
                    "TripletMatrixView: offset is out of range, size=%d, your offset=%d, your count=%d",
                    m_triplet_count,
                    offset,
                    count);

        return ThisView{m_total_rows,
                        m_total_cols,
                        m_triplet_index_offset + offset,
                        count,
                        m_total_triplet_count,
                        m_submatrix_offset,
                        m_submatrix_extent,
                        m_row_indices,
                        m_col_indices,
                        m_values};
    }

    MUDA_GENERIC auto submatrix(int2 offset, int2 extent) const
    {
        MUDA_KERNEL_ASSERT(offset.x >= 0 && offset.y >= 0,
                           "TripletMatrixView: submatrix is out of range, submatrix_offset.x=%d, submatrix_offset.y=%d",
                           offset.x,
                           offset.y);

        MUDA_KERNEL_ASSERT(offset.x + extent.x <= m_submatrix_extent.x
                               && offset.y + extent.y <= m_submatrix_extent.y,
                           "TripletMatrixView: submatrix is out of range, submatrix_offset.x=%d, submatrix_extent.x=%d, submatrix_offset.y=%d, submatrix_extent.y=%d",
                           offset.x,
                           m_submatrix_extent.x,
                           offset.y,
                           m_submatrix_extent.y);

        return ThisView{m_total_rows,
                        m_total_cols,
                        m_triplet_index_offset,
                        m_triplet_count,
                        m_total_triplet_count,
                        m_submatrix_offset + offset,
                        extent,
                        m_row_indices,
                        m_col_indices,
                        m_values};
    }

    MUDA_GENERIC auto subview(int offset) const
    {
        return subview(offset, m_triplet_count - offset);
    }

    MUDA_GENERIC auto cviewer() const
    {
        return ConstViewer{m_total_rows,
                           m_total_cols,
                           m_triplet_index_offset,
                           m_triplet_count,
                           m_total_triplet_count,
                           m_submatrix_offset,
                           m_submatrix_extent,
                           m_row_indices,
                           m_col_indices,
                           m_values};
    }

    MUDA_GENERIC auto viewer() const
    {
        return ThisViewer{m_total_rows,
                          m_total_cols,
                          m_triplet_index_offset,
                          m_triplet_count,
                          m_total_triplet_count,
                          m_submatrix_offset,
                          m_submatrix_extent,
                          m_row_indices,
                          m_col_indices,
                          m_values};
    }

    MUDA_GENERIC auto values() const { return m_values; }
    MUDA_GENERIC auto row_indices() const { return m_row_indices; }
    MUDA_GENERIC auto col_indices() const { return m_col_indices; }

    MUDA_GENERIC auto total_rows() const { return m_total_rows; }
    MUDA_GENERIC auto total_cols() const { return m_total_cols; }

    MUDA_GENERIC auto triplet_count() const { return m_triplet_count; }
    MUDA_GENERIC auto tripet_index_offset() const
    {
        return m_triplet_index_offset;
    }
    MUDA_GENERIC auto total_triplet_count() const
    {
        return m_total_triplet_count;
    }

    MUDA_GENERIC auto submatrix_offset() const { return m_submatrix_offset; }
    MUDA_GENERIC auto extent() const { return m_submatrix_extent; }
    MUDA_GENERIC auto total_extent() const
    {
        return int2{m_total_rows, m_total_cols};
    }
};

template <typename Ty, int N>
using TripletMatrixView = TripletMatrixViewT<false, Ty, N>;
template <typename Ty, int N>
using CTripletMatrixView = TripletMatrixViewT<true, Ty, N>;
}  // namespace muda

namespace muda
{
template <typename Ty, int N>
struct read_only_view<TripletMatrixView<Ty, N>>
{
    using type = CTripletMatrixView<Ty, N>;
};

template <typename Ty, int N>
struct read_write_view<TripletMatrixView<Ty, N>>
{
    using type = TripletMatrixView<Ty, N>;
};
}  // namespace muda


#include "details/triplet_matrix_view.inl"
```


