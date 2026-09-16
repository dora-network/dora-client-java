

# PromoLinkAdmin


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**tokenPrefix** | **String** |  |  |
|**url** | **URI** | Only present when reveal&#x3D;true. Private; do not log or cache. |  [optional] |
|**status** | **PromoLinkStatus** |  |  |
|**expiresAt** | **OffsetDateTime** |  |  |
|**claimedAt** | **OffsetDateTime** |  |  [optional] |
|**claimedEmail** | **String** | Masked as the first character, three asterisks, and domain. |  [optional] |
|**userId** | **UUID** |  |  [optional] |



