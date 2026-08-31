

# UserDeactivation

An admin-requested account deactivation. A non-REACTIVATED request blocks the user's trading, funding, and transfers.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**deactivationId** | **UUID** |  |  |
|**userId** | **UUID** |  |  |
|**requestedBy** | **UUID** | Admin that requested the deactivation. |  |
|**reason** | **String** |  |  |
|**status** | [**StatusEnum**](#StatusEnum) | PENDING: wind-down in progress. FAILED: wind-down gave up; admin can re-trigger. COMPLETED: account deactivated. REACTIVATED: blocks lifted. |  |
|**attempts** | **Integer** | Wind-down attempts performed so far. |  |
|**result** | **String** | Latest wind-down outcome or error summary. |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  |
|**updatedAt** | **OffsetDateTime** |  |  |
|**completedAt** | **OffsetDateTime** |  |  [optional] |
|**reactivatedBy** | **UUID** |  |  [optional] |
|**reactivatedAt** | **OffsetDateTime** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| PENDING | &quot;PENDING&quot; |
| FAILED | &quot;FAILED&quot; |
| COMPLETED | &quot;COMPLETED&quot; |
| REACTIVATED | &quot;REACTIVATED&quot; |



