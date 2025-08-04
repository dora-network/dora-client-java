# CreateOrderRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **String** |  | 
**inverseLeverage** | [**BigDecimal**](BigDecimal.md) | Required: Inverse leverage for the order, must be between 0 and 1 (inclusive) | 
**price** | **String** |  | 
**kind** | [**OrderKind**](OrderKind.md) |  | 
**side** | [**Side**](Side.md) |  | 
**orderBookId** | [**UUID**](UUID.md) | Required: the order book to submit the order to | 
**userText** | **String** | Optional: User-defined text for the order, e.g., &#x27;buying dips&#x27; |  [optional]
**orderModifiers** | [**List&lt;OrderModifierKind&gt;**](OrderModifierKind.md) |  |  [optional]
