

# CreateOrderRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**quantity** | **String** |  |  |
|**inverseLeverage** | **String** |  |  |
|**price** | **String** |  |  [optional] |
|**kind** | **OrderKind** |  |  |
|**side** | **Side** | Required: Must be either &#39;BUY&#39; or &#39;SELL&#39; |  |
|**fromGlobalPosition** | **Boolean** | use global position for the order or isolated. required. |  |
|**orderBookId** | **UUID** | Required: the order book to submit the order to |  |
|**orderModifiers** | **List&lt;OrderModifierKind&gt;** |  |  [optional] |
|**goodTillDate** | **OffsetDateTime** |  |  [optional] |
|**clientOrderId** | **String** | An optional client-provided identifier for the order. |  [optional] |
|**stopLossPrice** | **String** | Stop loss price |  [optional] |
|**takeProfitPrice** | **String** | Take profit price |  [optional] |



