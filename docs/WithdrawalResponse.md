

# WithdrawalResponse

A single USDC withdrawal request.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**withdrawalId** | **UUID** |  |  [optional] |
|**networkChainId** | **Integer** | Internal numeric identifier of the chain. |  [optional] |
|**networkName** | **String** | Human-readable network name. |  [optional] |
|**chainId** | **String** | EVM chain ID. |  [optional] |
|**userId** | **UUID** |  |  [optional] |
|**accountId** | **UUID** |  |  [optional] |
|**toAddress** | **String** | Destination wallet address as a 0x-prefixed hex string. |  [optional] |
|**quantity** | **String** | Human-decimal USDC quantity to withdraw (base units divided by 10^6). |  [optional] |
|**fee** | **String** | Human-decimal USDC network fee (base units divided by 10^6). 0 until the requester locks a quoted fee as part of approval. |  [optional] |
|**status** | **Web3WithdrawalStatus** |  |  [optional] |
|**txHash** | **String** | Broadcast withdraw() transaction hash as a 0x-prefixed hex string. Present from &#x60;BROADCAST&#x60; onward. |  [optional] |
|**failureReason** | **String** | Reason the withdrawal was rejected or failed. Present for REJECTED/FAILED. |  [optional] |
|**approvedBy** | **UUID** | Admin who approved the withdrawal. Present once approved. |  [optional] |
|**approvedAt** | **OffsetDateTime** | When the withdrawal was approved. Present once approved. |  [optional] |
|**settlementTransactionId** | **UUID** | Ledger settlement transaction. Present once confirmed. |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**updatedAt** | **OffsetDateTime** |  |  [optional] |



