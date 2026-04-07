

# CreateConditionalOrderRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**price** | **BigDecimal** |  |  |
|**orderBookId** | **UUID** | Required: the order book to submit the order to |  |
|**positionId** | **UUID** | Required: the position to submit the order to |  |
|**assetId** | **UUID** | Required: the asset to submit the order to |  |
|**stopLossPrice** | **BigDecimal** | Stop loss price |  [optional] |
|**takeProfitPrice** | **BigDecimal** | Take profit price |  [optional] |



