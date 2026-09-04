

# CashReserveResponse


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**enforced** | **Boolean** | Whether the minimum cash reserve guard is active in this environment. |  |
|**availableUsd** | **String** | The user&#39;s currently available USD balance in their Global Account. |  |
|**committedUsd** | **String** | USD still counted in available_usd but already claimed by the user&#39;s open market buy orders on the Global Account, which reserve no funds at submission time. The reserve is evaluated against available_usd minus committed_usd. |  |
|**requiredUsd** | **String** | The user&#39;s minimum USD cash reserve requirement. |  |
|**satisfied** | **Boolean** | Whether available_usd minus committed_usd is at least required_usd. |  |
|**maxVolumeUsd** | **String** | How much more traded USD notional the user can add to the current settlement period before the reserve stops being covered, for an order that borrows nothing. Null means the fee leg does not constrain the user, because the guard is disabled or the trading fee volume cap is zero. |  |
|**maxBorrowUsd** | **String** | How much more the user can borrow before the reserve stops being covered, for an order that adds no traded volume. Null means the borrow leg does not constrain the user, because the guard is disabled or the borrowed fraction is zero. The two caps are single axis: a leveraged order consumes both at once and is admissible when notional/max_volume_usd + borrowed/max_borrow_usd &lt;&#x3D; 1. |  |
|**breakdown** | [**CashReserveBreakdown**](CashReserveBreakdown.md) |  |  |



