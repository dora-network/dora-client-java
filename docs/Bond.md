# Bond

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | [**UUID**](UUID.md) |  |  [optional]
**kind** | [**BondKind**](BondKind.md) |  |  [optional]
**couponStartAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**createdAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**finalCouponAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**isin** | **String** |  |  [optional]
**issuedAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**issuer** | **String** |  |  [optional]
**maturityAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**principalValue** | **String** |  |  [optional]
**paymentsPerYear** | **Integer** |  |  [optional]
**paymentsEvery** | **Integer** | Coupon payment frequency in nanoseconds (minimum 1000 i.e. 1 microsecond) |  [optional]
**nextCouponPayment** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
