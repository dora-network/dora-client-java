

# IssuePromoLinkBatchRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**sourceType** | **PromoSourceType** |  |  |
|**sourceId** | **String** |  |  |
|**sourceName** | **String** |  |  [optional] |
|**allocation** | **Integer** | Required for SINGLE_USE; omit for REUSABLE. Bounded by max_links_per_batch. Minting reserves no campaign place. |  [optional] |
|**note** | **String** |  |  [optional] |
|**expiresAt** | **OffsetDateTime** | Defaults to challenge end and must fall between challenge start and end in the future. |  [optional] |
|**linkType** | [**LinkTypeEnum**](#LinkTypeEnum) | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. |  [optional] |
|**affiliateProgramId** | **UUID** |  |  [optional] |
|**affiliateMemberId** | **UUID** | Existing affiliate referrer/member ID, not user ID. |  [optional] |
|**referralCode** | **String** | An existing code belonging to the selected member. Required with both IDs for reusable links; bound on the server and revalidated at claim time. |  [optional] |



## Enum: LinkTypeEnum

| Name | Value |
|---- | -----|
| SINGLE_USE | &quot;SINGLE_USE&quot; |
| REUSABLE | &quot;REUSABLE&quot; |



