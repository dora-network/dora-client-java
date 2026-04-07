

# Bond


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**kind** | **BondKind** |  |  |
|**couponStartAt** | **OffsetDateTime** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  |
|**finalCouponAt** | **OffsetDateTime** |  |  [optional] |
|**isin** | **String** |  |  |
|**issuedAt** | **OffsetDateTime** |  |  |
|**issuer** | **String** |  |  |
|**maturityAt** | **OffsetDateTime** |  |  |
|**principalValue** | **String** |  |  |
|**paymentsPerYear** | **Integer** |  |  |
|**paymentsEvery** | **Long** | Coupon payment frequency in nanoseconds (minimum 1000 i.e. 1 microsecond) |  [optional] |
|**nextCouponPayment** | **OffsetDateTime** |  |  [optional] |



