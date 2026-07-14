

# DepositInstructionForChain

Everything the caller needs to deposit USDC into the Dora vault on a single chain with one signature and one transaction.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**networkName** | **String** | Human-readable network name, e.g. &#39;Ethereum Mainnet&#39;. |  |
|**chainId** | **String** | EVM chain ID. |  |
|**contractAddress** | **String** | The DoraUSDCVault contract address for this chain, as a 0x-prefixed hex string. |  |
|**usdcAddress** | **String** | The ERC-20 USDC token contract on this chain, as a 0x-prefixed hex string. It is the verifying contract of the permit; the spender granted by the permit is contract_address (the vault). |  |
|**approval** | [**PermitTypedData**](PermitTypedData.md) |  |  |
|**deposit** | [**DepositCall**](DepositCall.md) |  |  |



