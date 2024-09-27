

# File device\_run\_length\_encode.h

[**File List**](files.md) **>** [**cub**](dir_98c5d599fe44dff86fbf620b2a1f3e8e.md) **>** [**device**](dir_e7785ab0b6a4810de2e8c4f6e4ccf5c0.md) **>** [**device\_run\_length\_encode.h**](device__run__length__encode_8h.md)

[Go to the documentation of this file](device__run__length__encode_8h.md)


```C++
#pragma once
#include <muda/cub/device/cub_wrapper.h>
#include "details/cub_wrapper_macro_def.inl"
#ifndef __INTELLISENSE__
#include <cub/device/device_run_length_encode.cuh>
#endif

namespace muda
{
//ref: https://nvlabs.github.io/cub/structcub_1_1_device_run_length_encode.html
class DeviceRunLengthEncode : public CubWrapper<DeviceRunLengthEncode>
{
    using Base = CubWrapper<DeviceRunLengthEncode>;

  public:
    using Base::Base;

    template <typename InputIteratorT, typename UniqueOutputIteratorT, typename LengthsOutputIteratorT, typename NumRunsOutputIteratorT>
    DeviceRunLengthEncode& Encode(InputIteratorT         d_in,
                                  UniqueOutputIteratorT  d_unique_out,
                                  LengthsOutputIteratorT d_counts_out,
                                  NumRunsOutputIteratorT d_num_runs_out,
                                  int                    num_items)
    {
        MUDA_CUB_WRAPPER_IMPL(cub::DeviceRunLengthEncode::Encode(
            d_temp_storage, temp_storage_bytes, d_in, d_unique_out, d_counts_out, d_num_runs_out, num_items, _stream, false));
    }

    template <typename InputIteratorT, typename OffsetsOutputIteratorT, typename LengthsOutputIteratorT, typename NumRunsOutputIteratorT>
    DeviceRunLengthEncode& NonTrivialRuns(InputIteratorT         d_in,
                                          OffsetsOutputIteratorT d_offsets_out,
                                          LengthsOutputIteratorT d_lengths_out,
                                          NumRunsOutputIteratorT d_num_runs_out,
                                          int                    num_items)
    {
        MUDA_CUB_WRAPPER_IMPL(cub::DeviceRunLengthEncode::NonTrivialRuns(
            d_temp_storage, temp_storage_bytes, d_in, d_offsets_out, d_lengths_out, d_num_runs_out, num_items, _stream, false));
    }


    // Origin:

    template <typename InputIteratorT, typename UniqueOutputIteratorT, typename LengthsOutputIteratorT, typename NumRunsOutputIteratorT>
    DeviceRunLengthEncode& Encode(void*                  d_temp_storage,
                                  size_t&                temp_storage_bytes,
                                  InputIteratorT         d_in,
                                  UniqueOutputIteratorT  d_unique_out,
                                  LengthsOutputIteratorT d_counts_out,
                                  NumRunsOutputIteratorT d_num_runs_out,
                                  int                    num_items)
    {
        MUDA_CUB_WRAPPER_FOR_COMPUTE_GRAPH_IMPL(cub::DeviceRunLengthEncode::Encode(
            d_temp_storage, temp_storage_bytes, d_in, d_unique_out, d_counts_out, d_num_runs_out, num_items, _stream, false));
    }

    template <typename InputIteratorT, typename OffsetsOutputIteratorT, typename LengthsOutputIteratorT, typename NumRunsOutputIteratorT>
    DeviceRunLengthEncode& NonTrivialRuns(void*          d_temp_storage,
                                          size_t&        temp_storage_bytes,
                                          InputIteratorT d_in,
                                          OffsetsOutputIteratorT d_offsets_out,
                                          LengthsOutputIteratorT d_lengths_out,
                                          NumRunsOutputIteratorT d_num_runs_out,
                                          int                    num_items)
    {
        MUDA_CUB_WRAPPER_FOR_COMPUTE_GRAPH_IMPL(cub::DeviceRunLengthEncode::NonTrivialRuns(
            d_temp_storage, temp_storage_bytes, d_in, d_offsets_out, d_lengths_out, d_num_runs_out, num_items, _stream, false));
    }
};
}  // namespace muda

#include "details/cub_wrapper_macro_undef.inl"
```


