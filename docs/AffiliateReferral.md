

# AffiliateReferral

User profile and affiliate activity. Trade metrics, realized PnL and cash-flow counts/dates include only events at or after attributed_at. Signup and KYC fields describe the user profile.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**userId** | **UUID** |  |  |
|**programId** | **UUID** |  |  |
|**referrerId** | **UUID** |  |  |
|**referrerUserId** | **UUID** |  |  |
|**signupSource** | **String** | Client-reported signup hostname. Empty means unknown. |  |
|**firstName** | **String** |  |  |
|**lastName** | **String** |  |  |
|**email** | **String** |  |  |
|**signedUpAt** | **OffsetDateTime** |  |  |
|**kycCompleted** | **Boolean** |  |  |
|**kycCompletedAt** | **OffsetDateTime** |  |  |
|**discordStatus** | [**DiscordStatusEnum**](#DiscordStatusEnum) | No Discord membership integration is currently available. Unknown must not be interpreted as not joined. |  |
|**depositCount** | **Long** |  |  |
|**withdrawalCount** | **Long** |  |  |
|**hasTraded** | **Boolean** |  |  |
|**firstDepositAt** | **OffsetDateTime** |  |  |
|**lastDepositAt** | **OffsetDateTime** |  |  |
|**firstWithdrawalAt** | **OffsetDateTime** |  |  |
|**lastWithdrawalAt** | **OffsetDateTime** |  |  |
|**dailyVolumeUsd** | **String** | Sum of absolute executed FILL quantity1 on USD-quoted trades during the selected UTC day. Both buy and sell executions count, once per user-side fill. |  |
|**monthlyVolumeUsd** | **String** | Same executed USD quote-notional definition for the calendar month containing date. |  |
|**dailyRealizedPnlUsd** | **String** | Sum of realized_pnl_settlements.realized_usd created during the selected UTC day, matching the existing PnL ranking convention. Excludes unrealized PnL; this is not total account equity change. |  |
|**attributedAt** | **OffsetDateTime** | Immutable referral assignment time. Earlier activity is excluded from affiliate metrics and cash flows. |  |
|**monthlyRealizedPnlUsd** | **String** | Realized PnL for the UTC calendar month containing date, including only settlements at or after attributed_at. |  |



## Enum: DiscordStatusEnum

| Name | Value |
|---- | -----|
| UNKNOWN | &quot;unknown&quot; |



