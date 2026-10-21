

# PromoLinkBatchSummary


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**sourceType** | **PromoSourceType** |  |  |
|**sourceId** | **String** |  |  |
|**sourceName** | **String** |  |  |
|**allocation** | **Integer** |  |  [optional] |
|**issued** | **Long** |  |  [optional] |
|**claimed** | **Long** |  |  [optional] |
|**revoked** | **Long** |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  |
|**linkType** | [**LinkTypeEnum**](#LinkTypeEnum) | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. |  [optional] |
|**affiliateProgramId** | **UUID** |  |  [optional] |
|**affiliateMemberId** | **UUID** | Existing affiliate referrer/member ID, not user ID. |  [optional] |
|**referralCode** | **String** | An existing code belonging to the selected member. Required with both IDs for reusable links; bound on the server and revalidated at claim time. |  [optional] |
|**campaignId** | **UUID** |  |  [optional] |
|**signups** | **Long** | Successful signups; reusable links omit allocation/issued/claimed/revoked counts. |  [optional] |



## Enum: LinkTypeEnum

| Name | Value |
|---- | -----|
| SINGLE_USE | &quot;SINGLE_USE&quot; |
| REUSABLE | &quot;REUSABLE&quot; |



