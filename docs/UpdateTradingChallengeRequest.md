

# UpdateTradingChallengeRequest

Request body for PUT /v1/trading_challenges/{trading_challenge_id}: partially update a trading challenge. A field that is omitted, or sent as null, is left unchanged. Each field accepts either the {update, value} object or the bare value on its own. PENDING challenges accept every field; ACTIVE challenges accept only name, max_users, end and the prize quantities; COMPLETED challenges accept none. tenant_id and status are never updatable, and the participant list is managed by add_users and remove_users.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**name** | [**UpdateFieldString**](UpdateFieldString.md) | Trading challenge name. |  [optional] |
|**type** | [**UpdateFieldString**](UpdateFieldString.md) | CASH or TOURNAMENT. Only updatable while the challenge is PENDING. |  [optional] |
|**maxUsers** | [**UpdateFieldInteger**](UpdateFieldInteger.md) | Must be &gt; 0 and cannot be lowered below the number of users already registered. |  [optional] |
|**start** | [**UpdateFieldDateTime**](UpdateFieldDateTime.md) | Only updatable while the challenge is PENDING. |  [optional] |
|**end** | [**UpdateFieldDateTime**](UpdateFieldDateTime.md) | Must be after start and in the future. |  [optional] |
|**initialUserBalance** | [**UpdateFieldDecimal**](UpdateFieldDecimal.md) | Must be &gt; 0. Only updatable while the challenge is PENDING. |  [optional] |
|**goldPrizeQuantity** | [**UpdateFieldDecimal**](UpdateFieldDecimal.md) | Must be &gt; 0 for a TOURNAMENT challenge. |  [optional] |
|**silverPrizeQuantity** | [**UpdateFieldDecimal**](UpdateFieldDecimal.md) | Must be &gt;&#x3D; 0. |  [optional] |
|**bronzePrizeQuantity** | [**UpdateFieldDecimal**](UpdateFieldDecimal.md) | Must be &gt;&#x3D; 0. |  [optional] |
|**pnlCondition** | [**UpdateFieldDecimal**](UpdateFieldDecimal.md) | Must be &gt;&#x3D; 0. Only updatable while the challenge is PENDING. |  [optional] |
|**totalVolumeCondition** | [**UpdateFieldDecimal**](UpdateFieldDecimal.md) | Must be &gt;&#x3D; 0. Only updatable while the challenge is PENDING. |  [optional] |
|**avgDailyVolumeCondition** | [**UpdateFieldDecimal**](UpdateFieldDecimal.md) | Must be &gt;&#x3D; 0. Only updatable while the challenge is PENDING. |  [optional] |
|**minimumEquityPercentageCondition** | [**UpdateFieldInteger**](UpdateFieldInteger.md) | In the range [0,100). Only updatable while the challenge is PENDING. |  [optional] |



