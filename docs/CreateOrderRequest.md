# CreateOrderRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **String** |  |  [optional]
**inverseLeverage** | [**BigDecimal**](BigDecimal.md) | Required: Inverse leverage for the order, must be between 0 and 1 (inclusive) |  [optional]
**price** | **String** |  |  [optional]
**kind** | [**KindEnum**](#KindEnum) |  |  [optional]
**side** | **String** | Required: Must be either &#x27;BUY&#x27; or &#x27;SELL&#x27; |  [optional]
**orderBookId** | [**UUID**](UUID.md) | Required: the order book to submit the order to |  [optional]
**userText** | **String** | Optional: User-defined text for the order, e.g., &#x27;buying dips&#x27; |  [optional]
**orderModifiers** | [**List&lt;OrderModifiersEnum&gt;**](#List&lt;OrderModifiersEnum&gt;) |  |  [optional]

<a name="KindEnum"></a>
## Enum: KindEnum
Name | Value
---- | -----
MARKET | &quot;MARKET&quot;
LIMIT | &quot;LIMIT&quot;

<a name="List<OrderModifiersEnum>"></a>
## Enum: List&lt;OrderModifiersEnum&gt;
Name | Value
---- | -----
MAX_BUY | &quot;MAX_BUY&quot;
