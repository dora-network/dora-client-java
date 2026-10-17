

# AffiliateAttribution


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**referredUserId** | **UUID** |  |  |
|**programId** | **UUID** |  |  |
|**referrerId** | **UUID** |  |  |
|**referrerUserId** | **UUID** |  |  |
|**tenantId** | **String** | Tenant that owns the referrer and the program. A referrer in a global tenant may refer users of any tenant. |  |
|**referredTenantId** | **String** | Tenant that owns the referred user. Differs from tenant_id only when a global tenant&#39;s referrer referred the user. |  |
|**signupSource** | **String** | Signup hostname when assigned at signup; empty for an assignment made later. |  |
|**createdAt** | **OffsetDateTime** | Immutable assignment time; activity begins counting from this timestamp. |  |
|**referralCode** | **String** | Exact code the user entered, retained when the referrer changes their primary code. |  |



