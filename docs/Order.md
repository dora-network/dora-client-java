

# Order


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**orderId** | **UUID** |  |  |
|**orderBookId** | **UUID** |  |  |
|**kind** | **OrderKind** |  |  |
|**originalPrice** | **String** | If Kind is LIMIT, this is the original limit price. If Kind is MARKET, this may be 0 or omitted. |  |
|**avgFillPrice** | **String** |  |  |
|**cancelledQuantity** | **String** | Quantity that was cancelled, if any. |  |
|**openQuantity** | **String** | Quantity that is still open, i.e., not filled or cancelled. |  |
|**originalQuantity** | **String** | The original quantity of the order when it was created. |  |
|**filledQuantity** | **String** | Quantity that has been filled so far. |  |
|**filledNotional** | **String** | Quote quantity that has been filled so far. |  |
|**lockedQuantity** | **String** | Balance locked to ensure limit buy orders have sufficient balance to be fulfilled |  |
|**impendingBorrowsQuantity** | **String** | Borrows locked from the liquidity pool to ensure limit short sell orders have sufficient balance to be fulfilled |  |
|**lastUpdateAt** | **OffsetDateTime** |  |  |
|**openedAt** | **OffsetDateTime** |  |  |
|**inverseLeverage** | **String** |  |  |
|**side** | **Side** |  |  |
|**status** | **OrderStatus** |  |  |
|**userId** | **UUID** |  |  |
|**orderModifiers** | **List&lt;OrderModifierKind&gt;** |  |  [optional] |
|**positionId** | **UUID** |  |  |
|**orderInfo** | **String** |  |  [optional] |
|**goodTillDate** | **OffsetDateTime** |  |  [optional] |
|**triggerPrice** | **String** |  |  [optional] |
|**triggerType** | **TriggerType** |  |  [optional] |
|**clientOrderId** | **String** | An optional client-provided identifier for the order. |  [optional] |
|**parentOrderId** | **UUID** |  |  [optional] |



