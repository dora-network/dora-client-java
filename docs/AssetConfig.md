

# AssetConfig


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**assetId** | **UUID** |  |  |
|**price** | **String** | if an asset is a CURRENCY, set 1 USD price,If an asset is a BOND and the price isn&#39;t found, set to 0 USD   You can find price details on /price/asset/{asset_id} route |  |
|**moduleAvailable** | **String** | Optional leverage module available balance for this asset, from /v1/ledger/module/{asset_id}. If provided, validation rejects orders that need to borrow more than the module can supply. |  [optional] |
|**moduleSupplied** | **String** | Optional leverage module total supplied balance for this asset, from /v1/ledger/module/{asset_id}. Required with module_available when the asset has max_utilization. |  [optional] |
|**moduleBorrowed** | **String** | Optional leverage module borrowed balance for this asset, from /v1/ledger/module/{asset_id}. Required with module_available when the asset has max_utilization. |  [optional] |



