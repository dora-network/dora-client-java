# PLAsset

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**symbol** | **Object** | The symbol of the asset | 
**side** | **Object** | The side of the position (LONG or SHORT) | 
**avgEntryPrice** | **Object** | The average entry price of the position | 
**markPrice** | **Object** | The current mark price for the asset to calculate daily PL. This is usually the close price of the previous day | 
**liquidationPrice** | **Object** | The liquidation price of the position | 
**available** | **Object** | The available quantity in units of the asset | 
**borrowed** | **Object** | The borrowed quantity in units of the asset | 
**margin** | [**Margin**](Margin.md) |  | 
**unrealizedPl** | **Object** | The unrealized profit or loss of the position | 
**leverageLimit** | **Object** | The leverage limit for the position | 
**tp** | **Object** | The take profit price set for the position, if any |  [optional]
**sl** | **Object** | The stop loss price set for the position, if any |  [optional]
**initialCapital** | **Object** | The initial capital of the position | 
**impendingBorrows** | **Object** | The impending borrows of the position |  [optional]
**locked** | **Object** | The locked amount of the position | 
**unusedCollateral** | **Object** | The unused collateral of the position | 
