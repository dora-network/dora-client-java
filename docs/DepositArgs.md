

# DepositArgs

The non-signature arguments to the vault deposit() call. The remaining (v, r, s) arguments come from the permit signature the client obtains by signing the approval.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**quantity** | **String** | Deposit quantity in USDC base units (10^-6 USDC), as a decimal string. Matches the permit&#39;s value. |  |
|**userId** | **String** | The caller&#39;s user ID as 16 bytes, 0x-prefixed hex. Stored on-chain with the deposit and mapped back to the user by the indexer. |  |
|**clientReferenceId** | **String** | The bytes32 client reference as a 0x-prefixed hex string. All zero bytes when not supplied. |  |
|**deadline** | **String** | Unix timestamp (seconds), as a decimal string. Matches the permit&#39;s deadline exactly. |  |



