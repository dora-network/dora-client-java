# CreateOrderRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **String** |  | 
**inverseLeverage** | **String** |  | 
**price** | **String** |  |  [optional]
**kind** | [**OrderKind**](OrderKind.md) |  | 
**side** | [**Side**](Side.md) |  | 
**positionId** | [**UUID**](UUID.md) | position ID to use for the order. required. | 
**orderBookId** | [**UUID**](UUID.md) | Required: the order book to submit the order to | 
**orderModifiers** | [**List&lt;OrderModifierKind&gt;**](OrderModifierKind.md) |  |  [optional]
**goodTillDate** | [**OffsetDateTime**](OffsetDateTime.md) |  |  [optional]
**triggerPrice** | **String** |  |  [optional]
