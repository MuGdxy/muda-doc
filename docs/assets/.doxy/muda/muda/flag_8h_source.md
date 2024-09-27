

# File flag.h

[**File List**](files.md) **>** [**muda**](dir_be047e8c00f93e2e88c2a417393a7f42.md) **>** [**tools**](dir_4d62fb1c1e2c9fb3fa1c4847a09b7b77.md) **>** [**flag.h**](flag_8h.md)

[Go to the documentation of this file](flag_8h.md)


```C++
#pragma once
#include <type_traits>
#include <muda/muda_def.h>

namespace muda
{
template <typename BitType>
class Flags
{
  public:
    using bit_type  = BitType;
    using mask_type = typename ::std::underlying_type<bit_type>::type;

    // constructors
    MUDA_GENERIC MUDA_CONSTEXPR Flags() MUDA_NOEXCEPT : m_mask(0) {}

    MUDA_GENERIC MUDA_CONSTEXPR Flags(BitType bit) MUDA_NOEXCEPT
        : m_mask(static_cast<mask_type>(bit))
    {
    }

    MUDA_GENERIC MUDA_CONSTEXPR Flags(Flags<BitType> const& rhs) MUDA_NOEXCEPT = default;

    MUDA_GENERIC MUDA_CONSTEXPR explicit Flags(mask_type flags) MUDA_NOEXCEPT : m_mask(flags)
    {
    }

    // relational operators
    // auto operator<=>(Flags<BitType> const&) const = default;

    MUDA_GENERIC MUDA_CONSTEXPR bool operator<(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return m_mask < rhs.m_mask;
    }

    MUDA_GENERIC MUDA_CONSTEXPR bool operator<=(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return m_mask <= rhs.m_mask;
    }

    MUDA_GENERIC MUDA_CONSTEXPR bool operator>(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return m_mask > rhs.m_mask;
    }

    MUDA_GENERIC MUDA_CONSTEXPR bool operator>=(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return m_mask >= rhs.m_mask;
    }

    MUDA_GENERIC MUDA_CONSTEXPR bool operator==(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return m_mask == rhs.m_mask;
    }

    MUDA_GENERIC MUDA_CONSTEXPR bool operator!=(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return m_mask != rhs.m_mask;
    }


    // logical operator
    MUDA_GENERIC MUDA_CONSTEXPR bool operator!() const MUDA_NOEXCEPT
    {
        return !m_mask;
    }

    // bitwise operators
    MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator&(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return Flags<BitType>(m_mask & rhs.m_mask);
    }

    MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator|(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return Flags<BitType>(m_mask | rhs.m_mask);
    }

    MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator^(Flags<BitType> const& rhs) const MUDA_NOEXCEPT
    {
        return Flags<BitType>(m_mask ^ rhs.m_mask);
    }

    // assignment operators
    MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType>& operator=(Flags<BitType> const& rhs) MUDA_NOEXCEPT = default;

    MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType>& operator|=(Flags<BitType> const& rhs) MUDA_NOEXCEPT
    {
        m_mask |= rhs.m_mask;
        return *this;
    }

    MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType>& operator&=(Flags<BitType> const& rhs) MUDA_NOEXCEPT
    {
        m_mask &= rhs.m_mask;
        return *this;
    }

    MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType>& operator^=(Flags<BitType> const& rhs) MUDA_NOEXCEPT
    {
        m_mask ^= rhs.m_mask;
        return *this;
    }

    // cast operators
    explicit MUDA_GENERIC MUDA_CONSTEXPR operator bool() const MUDA_NOEXCEPT
    {
        return !!m_mask;
    }

    explicit MUDA_GENERIC MUDA_CONSTEXPR operator mask_type() const MUDA_NOEXCEPT
    {
        return m_mask;
    }

    MUDA_GENERIC MUDA_CONSTEXPR bool has(BitType bit) const MUDA_NOEXCEPT
    {
        return (m_mask & static_cast<mask_type>(bit)) == static_cast<mask_type>(bit);
    }

  private:
    mask_type m_mask;
};

//template <typename BitType>
//MUDA_GENERIC MUDA_CONSTEXPR bool operator<(BitType bit, Flags<BitType> const& flags) MUDA_NOEXCEPT
//{
//    return flags.operator>(bit);
//}
//
//template <typename BitType>
//MUDA_GENERIC MUDA_CONSTEXPR bool operator<=(BitType bit, Flags<BitType> const& flags) MUDA_NOEXCEPT
//{
//    return flags.operator>=(bit);
//}
//
//template <typename BitType>
//MUDA_GENERIC MUDA_CONSTEXPR bool operator>(BitType bit, Flags<BitType> const& flags) MUDA_NOEXCEPT
//{
//    return flags.operator<(bit);
//}
//
//template <typename BitType>
//MUDA_GENERIC MUDA_CONSTEXPR bool operator>=(BitType bit, Flags<BitType> const& flags) MUDA_NOEXCEPT
//{
//    return flags.operator<=(bit);
//}
//
//template <typename BitType>
//MUDA_GENERIC MUDA_CONSTEXPR bool operator==(BitType bit, Flags<BitType> const& flags) MUDA_NOEXCEPT
//{
//    return flags.operator==(bit);
//}
//
//template <typename BitType>
//MUDA_GENERIC MUDA_CONSTEXPR bool operator!=(BitType bit, Flags<BitType> const& flags) MUDA_NOEXCEPT
//{
//    return flags.operator!=(bit);
//}


// bitwise operators
template <typename BitType>
MUDA_INLINE MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator&(BitType bit,
                                                                 Flags<BitType> const& flags) MUDA_NOEXCEPT
{
    return flags.operator&(bit);
}

template <typename BitType>
MUDA_INLINE MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator|(BitType bit,
                                                                 Flags<BitType> const& flags) MUDA_NOEXCEPT
{
    return flags.operator|(bit);
}

template <typename BitType>
MUDA_INLINE MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator^(BitType bit,
                                                                 Flags<BitType> const& flags) MUDA_NOEXCEPT
{
    return flags.operator^(bit);
}

//template <typename BitType, typename ::std::enable_if<is_flag_type<BitType>::isBitmask, bool>::type = true>
//MUDA_INLINE MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator&(BitType lhs, BitType rhs) MUDA_NOEXCEPT
//{
//    return Flags<BitType>(lhs) & rhs;
//}
//
//template <typename BitType, typename ::std::enable_if<is_flag_type<BitType>::isBitmask, bool>::type = true>
//MUDA_INLINE MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator|(BitType lhs, BitType rhs) MUDA_NOEXCEPT
//{
//    return Flags<BitType>(lhs) | rhs;
//}
//
//template <typename BitType, typename ::std::enable_if<is_flag_type<BitType>::isBitmask, bool>::type = true>
//MUDA_INLINE MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator^(BitType lhs, BitType rhs) MUDA_NOEXCEPT
//{
//    return Flags<BitType>(lhs) ^ rhs;
//}
//
//template <typename BitType, typename ::std::enable_if<is_flag_type<BitType>::isBitmask, bool>::type = true>
//MUDA_INLINE MUDA_GENERIC MUDA_CONSTEXPR Flags<BitType> operator~(BitType bit) MUDA_NOEXCEPT
//{
//    return ~(Flags<BitType>(bit));
//}
}  // namespace muda
```


