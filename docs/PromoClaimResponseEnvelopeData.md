

# PromoClaimResponseEnvelopeData


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**state** | **PromoClaimState** |  |  |
|**email** | **String** |  |  [optional] |
|**campaignName** | **String** |  |  [optional] |
|**promoCredit** | **String** |  |  [optional] |
|**minRewardAmount** | **String** |  |  [optional] |
|**maxRewardAmount** | **String** |  |  [optional] |
|**targetEquity** | **String** |  |  [optional] |
|**expiresAt** | **OffsetDateTime** |  |  [optional] |
|**sourceName** | **String** |  |  [optional] |
|**linkType** | [**LinkTypeEnum**](#LinkTypeEnum) | Defaults to SINGLE_USE for existing clients. REUSABLE creates one tracked link without a quantity. |  [optional] |
|**affiliateProgramId** | **UUID** |  |  [optional] |
|**affiliateMemberId** | **UUID** | Existing affiliate referrer/member ID, not user ID. |  [optional] |
|**referralCode** | **String** | An existing code belonging to the selected member. Required with both IDs for reusable links; bound on the server and revalidated at claim time. |  [optional] |
|**campaignId** | **UUID** |  |  [optional] |
|**linkId** | **UUID** |  |  [optional] |
|**sourceId** | **String** |  |  [optional] |



## Enum: LinkTypeEnum

| Name | Value |
|---- | -----|
| SINGLE_USE | &quot;SINGLE_USE&quot; |
| REUSABLE | &quot;REUSABLE&quot; |



