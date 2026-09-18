

# TenantGuaranteeFundRow


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**tenantId** | **String** |  |  |
|**seq** | **Long** |  |  |
|**available** | **String** |  |  |
|**txKind** | [**TxKindEnum**](#TxKindEnum) |  |  |
|**updatedAt** | **OffsetDateTime** |  |  |



## Enum: TxKindEnum

| Name | Value |
|---- | -----|
| DEPOSIT | &quot;DEPOSIT&quot; |
| WITHDRAWAL | &quot;WITHDRAWAL&quot; |
| SETTLEMENT | &quot;SETTLEMENT&quot; |



