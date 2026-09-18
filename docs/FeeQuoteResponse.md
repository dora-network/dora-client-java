

# FeeQuoteResponse

The estimated network fee for one approved USDC withdrawal, alongside a signed, TTL-bound quote token bound to that withdrawal. Submit the token to PUT /v1/web3/withdrawals/{withdrawal_id} to reserve the quoted fee.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**withdrawalId** | **UUID** | The withdrawal this quote was issued for. The quote token is bound to it and cannot be redeemed against any other withdrawal. |  |
|**to** | **String** | The withdrawal destination address, read from the withdrawal row. |  |
|**quantity** | **String** | Human-decimal USDC withdrawal quantity, read from the withdrawal row. |  |
|**fee** | **String** | The estimated network fee, in human USDC. |  |
|**feeBaseUnits** | **String** | The estimated network fee, in micro-USDC base units. |  |
|**chainId** | **String** | EVM chain ID the quote was computed for. |  |
|**quoteToken** | **String** | Signed, TTL-bound quote token to submit to PUT /v1/web3/withdrawals/{withdrawal_id} so the server can validate the fee it quoted. It names the withdrawal it was issued for. |  |
|**expiresAt** | **OffsetDateTime** | When the quote token expires. |  |



