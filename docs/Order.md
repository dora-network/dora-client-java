# Order

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orderId** | **Object** |  |  [optional]
**orderBookId** | **Object** |  |  [optional]
**kind** | [**OrderKind**](OrderKind.md) |  |  [optional]
**originalPrice** | **Object** | If Kind is LIMIT, this is the original limit price. If Kind is MARKET, this may be 0 or omitted. |  [optional]
**avgFillPrice** | **Object** |  |  [optional]
**cancelledQuantity** | **Object** | Quantity that was cancelled, if any. |  [optional]
**openQuantity** | **Object** | Quantity that is still open, i.e., not filled or cancelled. |  [optional]
**originalQuantity** | **Object** | The original quantity of the order when it was created. |  [optional]
**filledQuantity** | **Object** | Quantity that has been filled so far. |  [optional]
**filledNotional** | **Object** | Quote quantity that has been filled so far. |  [optional]
**lastUpdateAt** | **Object** |  |  [optional]
**openedAt** | **Object** |  |  [optional]
**inverseLeverage** | **Object** |  |  [optional]
**side** | [**Side**](Side.md) |  |  [optional]
**status** | [**OrderStatus**](OrderStatus.md) |  |  [optional]
**userId** | **Object** |  |  [optional]
**orderModifiers** | **Object** |  |  [optional]
**positionId** | **Object** |  |  [optional]
**orderInfo** | **Object** |  |  [optional]
**goodTillDate** | **Object** |  |  [optional]
**triggerPrice** | **Object** |  |  [optional]
**triggerType** | [**TriggerType**](TriggerType.md) |  |  [optional]
