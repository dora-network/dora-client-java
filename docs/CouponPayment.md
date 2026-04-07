

# CouponPayment


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**assetId** | **UUID** |  |  |
|**yield** | **BigDecimal** |  |  |
|**startAt** | **OffsetDateTime** |  |  |
|**endAt** | **OffsetDateTime** |  |  |
|**payAt** | **OffsetDateTime** |  |  |
|**availableToPay** | **String** |  |  |
|**completedAt** | **OffsetDateTime** |  |  |
|**createdAt** | **OffsetDateTime** |  |  |
|**processEvery** | **Integer** | Number of nanoseconds to wait between coupon payment processing, must be at least 1000 (1 microsecond) |  |
|**lastProcessedAt** | **OffsetDateTime** |  |  |



