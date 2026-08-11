

# CashReserveBreakdown

Breakdown of the minimum USD cash reserve requirement.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**completedPac** | **String** | Completed PAC (partially accrued coupon) obligations the user owes, in USD. |  |
|**outstandingLai** | **String** | Outstanding LAI (leverage accrued interest) the user owes, in USD. |  |
|**estimatedFees** | **String** | Estimated trading fees for the current settlement period, capped at a configured fraction (1% by default) of the user&#39;s traded USD volume since 00:00:00 UTC. |  |
|**borrowedPortion** | **String** | Configured fraction (10% by default) of the user&#39;s total outstanding borrowed value, in USD. |  |
|**floor** | **String** | Configured absolute minimum requirement, in USD. |  |
|**total** | **String** | The amount of USD the user must keep available in their Global Account. |  |



