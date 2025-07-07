# ModuleBalance

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assetId** | [**UUID**](UUID.md) |  |  [optional]
**seq** | **Integer** |  |  [optional]
**available** | **String** | The available balance in the module for this asset |  [optional]
**supplied** | **String** | The total amount supplied to the module for this asset |  [optional]
**suppliedCollateral** | **String** | The amount supplied as collateral from user balances in the module for this asset |  [optional]
**virtual** | **String** | Assets minted by virtual-borrowing, but not yet repaid |  [optional]
**borrowed** | **String** | The total amount borrowed from the supplied but not yet repaid |  [optional]
