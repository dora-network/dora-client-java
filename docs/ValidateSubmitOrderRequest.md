# ValidateSubmitOrderRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **String** |  | 
**tick** | **String** | Minimum tradable increment for the selected order book | 
**kind** | [**OrderKind**](OrderKind.md) |  | 
**side** | [**Side**](Side.md) |  |  [optional]
**price** | **String** | If kind is LIMIT, must be &gt; 0; if MARKET it must be 0 or omitted | 
**goodTillDate** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**inverseLeverage** | **String** |  | 
**userBalance** | **String** | User balance used to ensure they can afford the requested quantity | 
