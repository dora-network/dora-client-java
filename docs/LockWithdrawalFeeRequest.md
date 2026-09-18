

# LockWithdrawalFeeRequest

Request to lock the network fee for an approved USDC withdrawal. The withdrawal is named by the path, and the fee itself is not part of the body: it is read from the signed quote token, so a client cannot choose what its own withdrawal costs.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**quoteToken** | **String** | The signed quote token returned by GET /v1/web3/withdrawals/fee-quote. It must still be within its TTL and must have been issued for this withdrawal&#39;s destination, quantity, and chain. |  |



