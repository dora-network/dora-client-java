

# FeeQuoteResponse

The estimated network fee to withdraw USDC via web3, alongside a signed, TTL-bound quote token the client submits with a later withdrawal so the server can validate the fee it was quoted.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**to** | **String** | The withdrawal destination address, echoed from the request. |  |
|**quantity** | **String** | Human-decimal USDC withdrawal quantity, echoed from the request. |  |
|**fee** | **String** | The estimated network fee, in human USDC. |  |
|**feeBaseUnits** | **String** | The estimated network fee, in micro-USDC base units. |  |
|**chainId** | **String** | EVM chain ID the quote was computed for. |  |
|**quoteToken** | **String** | Signed, TTL-bound quote token to submit with a later withdrawal so the server can validate the fee it was quoted. |  |
|**expiresAt** | **OffsetDateTime** | When the quote token expires. |  |



