

# PromoLinkAdmin


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**tokenPrefix** | **String** |  |  |
|**url** | **URI** | Only present when reveal&#x3D;true. Private; do not log or cache. |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) | Reusable links use ACTIVE or REVOKED and have no single claimant. |  |
|**expiresAt** | **OffsetDateTime** |  |  |
|**claimedAt** | **OffsetDateTime** |  |  [optional] |
|**claimedEmail** | **String** | Masked as the first character, three asterisks, and domain. |  [optional] |
|**userId** | **UUID** |  |  [optional] |
|**linkType** | [**LinkTypeEnum**](#LinkTypeEnum) | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ISSUED | &quot;ISSUED&quot; |
| CLAIMED | &quot;CLAIMED&quot; |
| REVOKED | &quot;REVOKED&quot; |
| ACTIVE | &quot;ACTIVE&quot; |



## Enum: LinkTypeEnum

| Name | Value |
|---- | -----|
| SINGLE_USE | &quot;SINGLE_USE&quot; |
| REUSABLE | &quot;REUSABLE&quot; |



