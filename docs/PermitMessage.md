

# PermitMessage

The EIP-2612 Permit struct the user signs. The uint256 fields are decimal strings to avoid JSON number precision loss.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**owner** | **String** | The user&#39;s wallet address (permit owner), as a 0x-prefixed hex string. |  |
|**spender** | **String** | The vault contract address granted the allowance, as a 0x-prefixed hex string. |  |
|**value** | **String** | Approved quantity in USDC base units (10^-6 USDC), as a decimal string. |  |
|**nonce** | **String** | The owner&#39;s current USDC permit nonce on this chain, as a decimal string. |  |
|**deadline** | **String** | Unix timestamp (seconds) at which the permit expires, as a decimal string. One hour from issuance. |  |



