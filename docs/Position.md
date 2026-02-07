# Position

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **Object** | The unique identifier for the position. Used, for example, when creating an order from a position, or deciding collateral should be transferred from position A to position B. | 
**assetId** | **Object** |  | 
**seq** | **Object** |  | 
**isGlobal** | **Object** |  |  [optional]
**available** | **Object** | The available balance in the position for this asset that are not locked, supplied, or used as collateral | 
**locked** | **Object** | The balance that has been reserved for a current order. If spent by the order, they are removed. If the order is cancelled, they are returned to the position&#x27;s available balance. | 
**supplied** | **Object** | The balance that user has supplied to the leverage module. The user remains entitled to these assets and can withdraw them into their available balance. | 
**borrowed** | **Object** | The total amount of debt outstanding for this position. This position cannot be closed until all debt is fully repaid, i.e. borrowed &#x3D; 0. | 
**impendingBorrows** | **Object** | The equivalent of locked balances, but for leveraged orders. If a user has an active order that would borrow assets as part of its input, then their borrow limit must be reduced until the order is executed or cancelled. | 
**avgEntryPrice** | **Object** | average cost per unit quantity that was paid (long positions) or received (short positions) for this asset. | 
**borrowLimit** | **Object** | The borrow limit | 
**liquidationThreshold** | **Object** | The borrow limit | 
**createdAt** | **Object** |  | 
**positionName** | **Object** |  | 
