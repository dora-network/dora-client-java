

# DepositCall

Descriptor of the vault deposit() transaction the client builds after signing the permit. The client splits the permit signature into v/r/s and ABI-encodes function_signature with args plus (v, r, s) to produce the calldata sent to 'to'.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**to** | **String** | The vault contract address, as a 0x-prefixed hex string. |  |
|**chainId** | **Long** | EVM chain ID, as a JSON number. |  |
|**value** | **String** | Native currency value to send with the transaction. Always &#39;0&#39;. |  |
|**functionSignature** | **String** | Canonical Solidity signature of the vault&#39;s permit-aware deposit function: deposit(uint256,bytes16,bytes32,uint256,uint8,bytes32,bytes32). |  |
|**selector** | **String** | The 4-byte ABI call selector of function_signature, as a 0x-prefixed hex string. |  |
|**args** | [**DepositArgs**](DepositArgs.md) |  |  |



