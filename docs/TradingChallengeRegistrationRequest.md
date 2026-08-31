

# TradingChallengeRegistrationRequest

A user's request to take part in a trading challenge, raised at sign-up and settled by an admin, the tenant's integrator or one of the challenge's managers. Approving it enrols the user; the row is kept after the decision as an audit trail.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**tradingChallengeId** | **UUID** |  |  |
|**tradingChallengeName** | **String** |  |  [optional] |
|**tradingChallengeType** | [**TradingChallengeTypeEnum**](#TradingChallengeTypeEnum) |  |  [optional] |
|**tradingChallengeStatus** | [**TradingChallengeStatusEnum**](#TradingChallengeStatusEnum) |  |  [optional] |
|**userId** | **UUID** |  |  |
|**userEmail** | **String** |  |  [optional] |
|**userName** | **String** |  |  [optional] |
|**tenantId** | **String** |  |  |
|**status** | [**StatusEnum**](#StatusEnum) |  |  |
|**reviewedBy** | **UUID** | Who settled the request. Absent while it is PENDING. |  [optional] |
|**reviewedAt** | **OffsetDateTime** | When it was settled. Absent while it is PENDING. |  [optional] |
|**reviewReason** | **String** | Free-text note kept for the audit trail. Optional on both decisions. |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  |
|**updatedAt** | **OffsetDateTime** |  |  |



## Enum: TradingChallengeTypeEnum

| Name | Value |
|---- | -----|
| TOURNAMENT | &quot;TOURNAMENT&quot; |
| CASH | &quot;CASH&quot; |



## Enum: TradingChallengeStatusEnum

| Name | Value |
|---- | -----|
| PENDING | &quot;PENDING&quot; |
| ACTIVE | &quot;ACTIVE&quot; |
| COMPLETED | &quot;COMPLETED&quot; |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| PENDING | &quot;PENDING&quot; |
| APPROVED | &quot;APPROVED&quot; |
| REJECTED | &quot;REJECTED&quot; |



