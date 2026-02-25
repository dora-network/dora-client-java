# CreateOrderRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **Object** |  | 
**inverseLeverage** | **Object** |  | 
**price** | **Object** |  |  [optional]
**kind** | [**OrderKind**](OrderKind.md) |  | 
**side** | [**Side**](Side.md) | Required: Must be either &#x27;BUY&#x27; or &#x27;SELL&#x27; | 
**fromGlobalPosition** | **Object** | use global position for the order or isolated. required. | 
**orderBookId** | **Object** | Required: the order book to submit the order to | 
**orderModifiers** | **Object** |  |  [optional]
**goodTillDate** | **Object** |  |  [optional]
**clientOrderId** | **Object** | An optional client-provided identifier for the order. |  [optional]
**stopLossPrice** | **Object** | Stop loss price |  [optional]
**takeProfitPrice** | **Object** | Take profit price |  [optional]
