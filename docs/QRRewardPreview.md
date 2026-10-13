

# QRRewardPreview


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**tradingChallengeId** | **UUID** |  |  |
|**state** | [**StateEnum**](#StateEnum) |  |  |
|**currentEquity** | **String** |  |  [optional] |
|**promoCredit** | **String** |  |  |
|**eligibleProfit** | **String** |  |  [optional] |
|**projectedReward** | **String** |  |  [optional] |
|**rewardAmount** | **String** |  |  [optional] |
|**minRewardAmount** | **String** |  |  |
|**maxRewardAmount** | **String** |  |  |
|**rewardDeadlineAt** | **OffsetDateTime** |  |  |
|**kycCompleted** | **Boolean** |  |  |
|**kycUrl** | **URI** |  |  [optional] |
|**blockers** | [**List&lt;BlockersEnum&gt;**](#List&lt;BlockersEnum&gt;) |  |  |



## Enum: StateEnum

| Name | Value |
|---- | -----|
| NOT_ELIGIBLE | &quot;NOT_ELIGIBLE&quot; |
| ELIGIBLE | &quot;ELIGIBLE&quot; |
| PENDING_KYC | &quot;PENDING_KYC&quot; |
| PAID | &quot;PAID&quot; |
| LAPSED | &quot;LAPSED&quot; |



## Enum: List&lt;BlockersEnum&gt;

| Name | Value |
|---- | -----|
| BELOW_MINIMUM_PAYOUT | &quot;BELOW_MINIMUM_PAYOUT&quot; |
| BUSTED | &quot;BUSTED&quot; |
| OTHER_CHALLENGE_FUNDED | &quot;OTHER_CHALLENGE_FUNDED&quot; |
| REWARD_DEADLINE_PASSED | &quot;REWARD_DEADLINE_PASSED&quot; |
| CHALLENGE_NOT_STARTED | &quot;CHALLENGE_NOT_STARTED&quot; |
| ALREADY_REQUESTED | &quot;ALREADY_REQUESTED&quot; |
| KYC_URL_UNAVAILABLE | &quot;KYC_URL_UNAVAILABLE&quot; |



