# Order

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**orderId** | **Object** |  | 
**orderBookId** | **Object** |  | 
**kind** | [**OrderKind**](OrderKind.md) |  | 
**originalPrice** | **Object** | If Kind is LIMIT, this is the original limit price. If Kind is MARKET, this may be 0 or omitted. | 
**avgFillPrice** | **Object** |  | 
**cancelledQuantity** | **Object** | Quantity that was cancelled, if any. | 
**openQuantity** | **Object** | Quantity that is still open, i.e., not filled or cancelled. | 
**originalQuantity** | **Object** | The original quantity of the order when it was created. | 
**filledQuantity** | **Object** | Quantity that has been filled so far. | 
**filledNotional** | **Object** | Quote quantity that has been filled so far. | 
**lastUpdateAt** | **Object** |  |  [optional]
**openedAt** | **Object** |  | 
**inverseLeverage** | **Object** |  | 
**side** | [**Side**](Side.md) |  | 
**status** | [**OrderStatus**](OrderStatus.md) |  | 
**userId** | **Object** |  | 
**orderModifiers** | **Object** |  |  [optional]
**positionId** | **Object** |  | 
**orderInfo** | **Object** |  |  [optional]
**goodTillDate** | **Object** |  |  [optional]
**triggerPrice** | **Object** |  |  [optional]
**triggerType** | [**TriggerType**](TriggerType.md) |  |  [optional]
**clientOrderId** | **Object** | An optional client-provided identifier for the order. |  [optional]
