

# IssuePromoLinkBatchRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**sourceType** | **PromoSourceType** |  |  |
|**sourceId** | **String** |  |  |
|**sourceName** | **String** |  |  [optional] |
|**allocation** | **Integer** | Cannot exceed the configured max_links_per_batch or remaining campaign capacity. |  |
|**note** | **String** |  |  [optional] |
|**expiresAt** | **OffsetDateTime** | Defaults to challenge end and must fall between challenge start and end in the future. |  [optional] |



