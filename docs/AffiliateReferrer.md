

# AffiliateReferrer


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** |  |  |
|**programId** | **UUID** |  |  |
|**tenantId** | **String** | Owning tenant for administration. This does not define a referral destination. |  |
|**userId** | **UUID** |  |  |
|**referralCode** | **String** | Current code to share; previously issued codes remain valid. Stored uppercase and unique across all programs and tenants. |  |
|**createdAt** | **OffsetDateTime** |  |  |
|**customizedAt** | **OffsetDateTime** | When the owner used their one code change; null until then. |  |



