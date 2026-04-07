

# UpdateUserConfigRequest

Request body for PUT /user/{id}/config: update a user changeable details only. Other properties can only be changed by an admin following a manual request by the user.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**photoUrl** | [**UpdateFieldString**](UpdateFieldString.md) | Optional: URL of the user&#39;s profile photo, optional. |  [optional] |
|**timezone** | [**UpdateFieldString**](UpdateFieldString.md) | User&#39;s timezone, e.g., &#39;America/New_York&#39;, or an offset. |  |
|**showTutorialCards** | [**UpdateFieldBoolean**](UpdateFieldBoolean.md) | Optional: Whether to show the tutorial. |  [optional] |
|**notificationsEnabled** | [**UpdateFieldBoolean**](UpdateFieldBoolean.md) | Optional: Whether to show the notifications. |  [optional] |
|**allowEmailNotifications** | [**UpdateFieldBoolean**](UpdateFieldBoolean.md) | Optional: Whether to allow email notifications. |  [optional] |
|**allowLiquidationsNotifications** | [**UpdateFieldBoolean**](UpdateFieldBoolean.md) | Optional: Whether to allow liquidations notifications. |  [optional] |
|**allowDepositWithdrawalNotifications** | [**UpdateFieldBoolean**](UpdateFieldBoolean.md) | Optional: Whether to allow deposit/withdrawal notifications. |  [optional] |
|**allowOrdersNotifications** | [**UpdateFieldBoolean**](UpdateFieldBoolean.md) | Optional: Whether to allow orders notifications. |  [optional] |



