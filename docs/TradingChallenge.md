

# TradingChallenge


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**name** | **String** | Trading challenge name |  [optional] |
|**tenantId** | **String** |  |  |
|**type** | **TradingChallengeType** |  |  |
|**status** | **TradingChallengeStatus** |  |  |
|**maxUsers** | **Integer** |  |  |
|**startAt** | **OffsetDateTime** |  |  |
|**endAt** | **OffsetDateTime** |  |  |
|**initialUserBalance** | **String** |  |  |
|**goldPrizeQuantity** | **String** |  |  |
|**silverPrizeQuantity** | **String** |  |  |
|**bronzePrizeQuantity** | **String** |  |  |
|**pnlCondition** | **String** |  |  |
|**totalVolumeCondition** | **String** |  |  |
|**avgDailyVolumeCondition** | **String** |  |  |
|**minimumEquityPercentageCondition** | **Integer** |  |  |
|**createdAt** | **OffsetDateTime** |  |  |
|**lastProcessedAt** | **OffsetDateTime** |  |  [optional] |
|**users** | **List&lt;UUID&gt;** |  |  [optional] |
|**usersCount** | **Integer** |  |  |
|**qr** | [**TradingChallengeQR**](TradingChallengeQR.md) |  |  [optional] |
|**worstCaseExposure** | **String** | For QR_PROMO, max_users multiplied by initial_user_balance plus max_reward_amount. |  [optional] |



