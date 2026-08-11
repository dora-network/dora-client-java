

# CashReserveResponse


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**enforced** | **Boolean** | Whether the minimum cash reserve guard is active in this environment. |  |
|**availableUsd** | **String** | The user&#39;s currently available USD balance in their Global Account. |  |
|**committedUsd** | **String** | USD still counted in available_usd but already claimed by the user&#39;s open market buy orders on the Global Account, which reserve no funds at submission time. The reserve is evaluated against available_usd minus committed_usd. |  |
|**requiredUsd** | **String** | The user&#39;s minimum USD cash reserve requirement. |  |
|**satisfied** | **Boolean** | Whether available_usd minus committed_usd is at least required_usd. |  |
|**breakdown** | [**CashReserveBreakdown**](CashReserveBreakdown.md) |  |  |



