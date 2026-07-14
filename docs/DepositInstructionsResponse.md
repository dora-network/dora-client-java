

# DepositInstructionsResponse

Per-chain instructions for depositing USDC into the Dora vault via EIP-2612 permit.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**userId** | **UUID** | The authenticated user the instructions are issued for. |  |
|**ownerAddress** | **String** | The wallet address the instructions were issued for, echoed from the request. |  |
|**quantity** | **String** | Human-decimal USDC deposit quantity, echoed from the request. |  |
|**chains** | [**List&lt;DepositInstructionForChain&gt;**](DepositInstructionForChain.md) |  |  |



