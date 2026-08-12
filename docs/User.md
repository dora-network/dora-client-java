

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
|**timezone** | **String** | User&#39;s timezone, e.g., &#39;America/New_York&#39;, or an offset. |  [optional] |
|**timezoneOffset** | **Integer** | timezone offset in seconds |  [optional] |
|**verifiedAt** | **OffsetDateTime** |  |  [optional] |
|**showTutorialCards** | **Boolean** |  |  |
|**notificationsEnabled** | **Boolean** |  |  |
|**tenantId** | **String** |  |  |
|**allowEmailNotifications** | **Boolean** |  |  |
|**allowLiquidationsNotifications** | **Boolean** |  |  |
|**allowDepositWithdrawalNotifications** | **Boolean** |  |  |
|**allowOrdersNotifications** | **Boolean** |  |  |
|**allowCopyTrading** | **Boolean** |  |  |
|**kycCompletedAt** | **OffsetDateTime** | When the user completed KYC. Omitted/null if KYC has not been completed. Set via POST /v1/integrators/user/{user_id}/kyc. |  [optional] |



