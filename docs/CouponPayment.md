# CouponPayment

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | [**UUID**](UUID.md) |  |  [optional]
**assetId** | [**UUID**](UUID.md) |  |  [optional]
**yield** | [**BigDecimal**](BigDecimal.md) |  |  [optional]
**startAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**endAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**payAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**availableToPay** | **String** |  |  [optional]
**completedAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**createdAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**processEvery** | **Integer** | Number of nanoseconds to wait between coupon payment processing, must be at least 1000 (1 microsecond) |  [optional]
**lastProcessedAt** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
