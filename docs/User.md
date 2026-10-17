

# User


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**closedAt** | **OffsetDateTime** |  |  [optional] |
|**disabledAt** | **OffsetDateTime** |  |  [optional] |
|**email** | **String** |  |  |
|**firstName** | **String** |  |  |
|**lastName** | **String** |  |  |
|**userName** | **String** |  |  |
|**countryOfDomicile** | **CountryCode** |  |  |
|**nativeAssetId** | **UUID** |  |  |
|**photoUrl** | **String** |  |  [optional] |
|**provider** | **String** |  |  [optional] |
|**providerId** | **UUID** |  |  [optional] |
|**roles** | **List&lt;UserRole&gt;** |  |  |
|**managedCompetitionIds** | **List&lt;UUID&gt;** | Competition IDs this user is explicitly allowed to manage when they have COMPETITION_MANAGER role. Empty means no competition-management access. |  [optional] |
|**managedAffiliateProgramIds** | **List&lt;UUID&gt;** | Affiliate program IDs this user is explicitly allowed to manage when they have AFFILIATE_MANAGER role. Empty means no affiliate-management access. |  [optional] |
|**timezone** | **String** | User&#39;s timezone, e.g., &#39;America/New_York&#39;, or an offset. |  [optional] |
|**timezoneOffset** | **Integer** | timezone offset in seconds |  [optional] |
|**verifiedAt** | **OffsetDateTime** |  |  [optional] |
|**showTutorialCards** | **Boolean** |  |  |
|**notificationsEnabled** | **Boolean** |  |  |
|**tenantId** | **String** |  |  |
|**usedReferralCode** | **String** | Exact affiliate code this user applied at signup or later. Empty when no code has been applied; distinct from codes the user owns. |  |
|**allowEmailNotifications** | **Boolean** |  |  |
|**allowLiquidationsNotifications** | **Boolean** |  |  |
|**allowDepositWithdrawalNotifications** | **Boolean** |  |  |
|**allowOrdersNotifications** | **Boolean** |  |  |
|**allowCopyTrading** | **Boolean** |  |  |
|**kycCompletedAt** | **OffsetDateTime** | When the user completed KYC. Omitted/null if KYC has not been completed. Set via POST /v1/integrators/user/{user_id}/kyc. |  [optional] |
|**tag** | **List&lt;UsersTag&gt;** | Tags assigned to the user by an admin. Set via PUT /v1/users/{user_id}/tag. |  [optional] |



