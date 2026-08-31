

# CreateIntegratorUserRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**email** | **String** |  |  [optional] |
|**firstName** | **String** |  |  [optional] |
|**lastName** | **String** |  |  [optional] |
|**userName** | **String** |  |  [optional] |
|**countryOfDomicile** | **CountryCode** |  |  [optional] |
|**nativeAssetId** | **UUID** | Optional: the user&#39;s native asset ID. Must be a CURRENCY asset; defaults to USD. The USDC asset is never allowed for integrator-created users. |  [optional] |
|**photoUrl** | **String** |  |  [optional] |
|**provider** | **String** |  |  [optional] |
|**providerId** | **UUID** |  |  [optional] |
|**timezone** | **String** |  |  [optional] |
|**challengeId** | **UUID** | Optional: sign the new user up for this trading challenge. This creates a PENDING registration request that an admin, the tenant&#39;s integrator or one of the challenge&#39;s managers must approve before the user is actually enrolled. The challenge must belong to the new user&#39;s tenant and still be open for entries, otherwise the whole sign-up fails. |  [optional] |



