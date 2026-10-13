

# AutoRebalanceConfigStatus


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**accountId** | **UUID** |  |  |
|**enabled** | **Boolean** |  |  |
|**minUtilization** | **String** |  |  |
|**maxUtilization** | **String** |  |  |
|**availableUsd** | **String** |  |  [optional] |
|**borrowedValue** | **String** |  |  [optional] |
|**borrowLimit** | **String** |  |  [optional] |
|**currentUtilization** | **String** |  |  [optional] |
|**aboveMax** | **Boolean** | True when current_utilization is greater than max_utilization. |  [optional] |
|**inActiveLiquidation** | **Boolean** |  |  [optional] |
|**lastRebalanceOutcome** | **String** | Most recent persisted auto-rebalance attempt status for this account, when available. |  [optional] |



