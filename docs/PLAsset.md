# PLAsset

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**symbol** | **Object** | The symbol of the asset |  [optional]
**side** | **Object** | The side of the position (LONG or SHORT) |  [optional]
**avgEntryPrice** | **Object** | The average entry price of the position |  [optional]
**markPrice** | **Object** | The current mark price for the asset to calculate daily PL. This is usually the close price of the previous day |  [optional]
**liquidationPrice** | **Object** | The liquidation price of the position |  [optional]
**available** | **Object** | The available quantity in units of the asset |  [optional]
**borrowed** | **Object** | The borrowed quantity in units of the asset |  [optional]
**margin** | [**Margin**](Margin.md) |  |  [optional]
**unrealizedPl** | **Object** | The unrealized profit or loss of the position |  [optional]
**leverageLimit** | **Object** | The leverage limit for the position |  [optional]
**tp** | **Object** | The take profit price set for the position, if any |  [optional]
**sl** | **Object** | The stop loss price set for the position, if any |  [optional]
**initialCapital** | **Object** | The initial capital of the position |  [optional]
**impendingBorrows** | **Object** | The impending borrows of the position |  [optional]
**locked** | **Object** | The locked amount of the position |  [optional]
**unusedCollateral** | **Object** | The unused collateral of the position |  [optional]
