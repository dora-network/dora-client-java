

# PermitTypedData

An EIP-712 typed-data message in the exact shape expected by eth_signTypedData_v4. The user signs it to authorize the vault as a USDC spender via EIP-2612 permit.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**types** | **Map&lt;String, List&lt;TypedDataField&gt;&gt;** | EIP-712 type definitions, keyed by type name (&#39;EIP712Domain&#39; and &#39;Permit&#39;). |  |
|**primaryType** | **String** | Always &#39;Permit&#39;. |  |
|**domain** | [**PermitDomain**](PermitDomain.md) |  |  |
|**message** | [**PermitMessage**](PermitMessage.md) |  |  |



