

# DepositResponse

A single USDC deposit observed on-chain.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**networkChainId** | **Integer** | Internal numeric identifier of the chain. |  |
|**networkName** | **String** | Human-readable network name. |  |
|**chainId** | **String** | EVM chain ID. |  |
|**txHash** | **String** | Transaction hash as a 0x-prefixed hex string. |  |
|**logIndex** | **Integer** | Index of the log within the transaction. |  |
|**blockNumber** | **Long** |  |  |
|**blockTime** | **OffsetDateTime** |  |  |
|**contractAddress** | **String** | Vault contract address as a 0x-prefixed hex string. |  |
|**depositorAddress** | **String** | Address that made the deposit, as a 0x-prefixed hex string. |  |
|**userId** | **UUID** |  |  |
|**quantity** | **String** | Human-decimal USDC value (base units divided by 10^6). |  |
|**clientReferenceId** | **String** | Optional client-supplied reference, as a 0x-prefixed hex string. |  [optional] |
|**status** | **Web3EventStatus** |  |  |
|**transactionId** | **UUID** | Internal transaction ID, present once the deposit has been credited. |  [optional] |
|**observedAt** | **OffsetDateTime** |  |  |



