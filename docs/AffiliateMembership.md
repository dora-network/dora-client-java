

# AffiliateMembership


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**programId** | **UUID** |  |  |
|**tenantId** | **String** | Owning tenant for administration. This does not define a referral destination. |  |
|**userId** | **UUID** |  |  |
|**referralCode** | **String** | Current code to share; previously issued codes remain valid. |  |
|**createdAt** | **OffsetDateTime** |  |  |
|**programName** | **String** |  |  |
|**isActive** | **Boolean** |  |  |
|**customizedAt** | **OffsetDateTime** |  |  |
|**canCustomize** | **Boolean** | True when this membership has not used its one-time code change, including while the program is inactive. |  |



