

# IssuePromoLinkBatchResponseData


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**batchId** | **UUID** |  |  |
|**sourceId** | **String** |  |  |
|**allocation** | **Integer** |  |  [optional] |
|**links** | [**List&lt;IssuedPromoLink&gt;**](IssuedPromoLink.md) |  |  |
|**linkType** | [**LinkTypeEnum**](#LinkTypeEnum) | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. |  [optional] |
|**affiliateProgramId** | **UUID** |  |  [optional] |
|**affiliateMemberId** | **UUID** | Existing affiliate referrer/member ID, not user ID. |  [optional] |
|**referralCode** | **String** | An existing code belonging to the selected member. Required with both IDs for reusable links; bound on the server and revalidated at claim time. |  [optional] |



## Enum: LinkTypeEnum

| Name | Value |
|---- | -----|
| SINGLE_USE | &quot;SINGLE_USE&quot; |
| REUSABLE | &quot;REUSABLE&quot; |



