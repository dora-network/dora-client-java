# ValidateSubmitOrderRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **Object** |  | 
**tick** | **Object** | Minimum tradable increment for the selected order book | 
**kind** | [**OrderKind**](OrderKind.md) | Must be LIMIT or MARKET | 
**side** | [**Side**](Side.md) | Must be BUY or SELL |  [optional]
**price** | **Object** | If kind is LIMIT, must be &gt; 0; if MARKET it must be 0 or omitted | 
**goodTillDate** | **Object** |  |  [optional]
**inverseLeverage** | **Object** |  | 
**userBalance** | **Object** | User balance used to ensure they can afford the requested quantity | 
**baseAssetId** | **Object** | base asset of orderbook |  [optional]
**quoteAssetId** | **Object** | quote asset of orderbook |  [optional]
**clientOrderId** | **Object** | An optional client-provided identifier for the order. |  [optional]
**positionAssets** | **Object** | Full list of assets in the position with their price and collateral weight, required when inverse_leverage &lt; 1 for leverage health checks |  [optional]
**assetsConfig** | **Object** | Configuration for the assets in the order |  [optional]
