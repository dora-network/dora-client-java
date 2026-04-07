

# RealizedPnlSettlement


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** | The ID of the realized PnL settlement |  |
|**userId** | **UUID** | The ID of the user associated with the realized PnL settlement |  |
|**tenantId** | **String** | The ID of the tenant associated with the realized PnL settlement |  |
|**positionId** | **UUID** | The ID of the position associated with the realized PnL settlement |  |
|**orderId** | **UUID** | The ID of the position-closing order associated with the realized PnL settlement |  |
|**realizedUsd** | **BigDecimal** | The amount of realized PnL in USD |  |
|**settledAt** | **OffsetDateTime** | The timestamp when the realized PnL settlement was settled |  [optional] |
|**createdAt** | **OffsetDateTime** | The timestamp when the realized PnL settlement was created |  |



