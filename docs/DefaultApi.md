# DefaultApi

All URIs are relative to *https://staging.dora.co*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**approveLedgerWithdrawRequest**](DefaultApi.md#approveLedgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/{withdrawal_id}/approve | Approve a pending withdrawal request |
| [**cancelAllOpenOrders**](DefaultApi.md#cancelAllOpenOrders) | **DELETE** /v1/orders | Cancel all open orders, if user passes orderbook or account_id on query params it will cancel all orders on specific orderbook or account, admin can cancel user&#39;s orders on specific orderbook |
| [**cancelLedgerWithdrawRequest**](DefaultApi.md#cancelLedgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/{withdrawal_id}/cancel | Cancel a pending withdrawal request |
| [**cancelOrderById**](DefaultApi.md#cancelOrderById) | **DELETE** /v1/orders/{order_id} | Cancel an order by ID |
| [**claimLeverageGetAccruedInterest**](DefaultApi.md#claimLeverageGetAccruedInterest) | **POST** /v1/leverage/accrued_interest/claim | Claim current accrued leverage interest for a specific user |
| [**closeIsolatedAccountV2**](DefaultApi.md#closeIsolatedAccountV2) | **POST** /v2/accounts/close | Close an isolated account, repaying the borrowed |
| [**closeIsolatedPosition**](DefaultApi.md#closeIsolatedPosition) | **POST** /v1/positions/close | Close isolated positions, repaying the borrowed |
| [**createAPIKeyForUser**](DefaultApi.md#createAPIKeyForUser) | **POST** /v1/user/apikey | Create apikey for a user |
| [**createAPIKeyForUserID**](DefaultApi.md#createAPIKeyForUserID) | **POST** /v1/user/{user_id}/apikey | Create apikey for a user |
| [**createConditionalOrder**](DefaultApi.md#createConditionalOrder) | **POST** /v1/orders/conditional | Create a new conditional orders |
| [**createNewIsolatedAccountV2**](DefaultApi.md#createNewIsolatedAccountV2) | **POST** /v2/accounts/new_isolated | Create a new isolated account for a user transferring available assets into the account |
| [**createOrder**](DefaultApi.md#createOrder) | **POST** /v1/orders | Create a new order |
| [**createUser**](DefaultApi.md#createUser) | **POST** /v1/integrators/user | Create a new user |
| [**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /v1/user/{user_id} | Delete user by ID |
| [**getAPIKeysForUserID**](DefaultApi.md#getAPIKeysForUserID) | **GET** /v1/user/{user_id}/apikey | Get user&#39;s api keys: admin or integrator only |
| [**getAllAssetPrices**](DefaultApi.md#getAllAssetPrices) | **GET** /v1/price | Get the current price of all assets |
| [**getAllPositions**](DefaultApi.md#getAllPositions) | **GET** /v1/ledger/positions | Get all users&#39; positions |
| [**getAllWithdrawalRequests**](DefaultApi.md#getAllWithdrawalRequests) | **GET** /v1/ledger/withdraw/requests | Get all withdrawal requests |
| [**getAssetById**](DefaultApi.md#getAssetById) | **GET** /v1/assets/{asset_id} | Get asset by ID |
| [**getAssetPrice**](DefaultApi.md#getAssetPrice) | **GET** /v1/price/asset/{asset_id} | Get the current price of an asset |
| [**getAssetYTMById**](DefaultApi.md#getAssetYTMById) | **GET** /v1/assets/{asset_id}/ytm | Get annualized yield to maturity for a bond asset |
| [**getAssetsStream**](DefaultApi.md#getAssetsStream) | **GET** /v1/assets/stream | Get all inserts or updates for assets |
| [**getCandleData**](DefaultApi.md#getCandleData) | **GET** /v1/charts/{order_book_id}/candle | Get candlestick data for an orderbook |
| [**getCouponPaymentsByAssetId**](DefaultApi.md#getCouponPaymentsByAssetId) | **GET** /v1/assets/{asset_id}/coupon_payments | Get coupon payments for a bond asset |
| [**getL1Depth**](DefaultApi.md#getL1Depth) | **GET** /v1/orderbooks/{order_book_id}/L1 | Get the top price levels for a specific orderbook (L1 market depth) |
| [**getL2Depth**](DefaultApi.md#getL2Depth) | **GET** /v1/orderbooks/{order_book_id}/L2 | Get the aggregated price levels for a specific orderbook (L2 market depth) |
| [**getL3Depth**](DefaultApi.md#getL3Depth) | **GET** /v1/orderbooks/{order_book_id}/L3 | Get all open orders for a specific orderbook (L3 market depth) |
| [**getLedgerAccountsSelfV2**](DefaultApi.md#getLedgerAccountsSelfV2) | **GET** /v2/ledger/accounts/self | Get your own accounts |
| [**getLedgerBalancesSelf**](DefaultApi.md#getLedgerBalancesSelf) | **GET** /v1/ledger/balances/self | Get your own available, locked, and borrowed assets |
| [**getLedgerInterestSelf**](DefaultApi.md#getLedgerInterestSelf) | **GET** /v1/ledger/interest/self | Get your own interest |
| [**getLedgerModule**](DefaultApi.md#getLedgerModule) | **GET** /v1/ledger/module | Get the entire module object, including unborrowed leverage assets and total leverage trackers |
| [**getLedgerModuleByAsset**](DefaultApi.md#getLedgerModuleByAsset) | **GET** /v1/ledger/module/{asset_id} | Get the module object for a single asset ID |
| [**getLedgerPositionsSelf**](DefaultApi.md#getLedgerPositionsSelf) | **GET** /v1/ledger/positions/self | Get your own positions |
| [**getLedgerValueSelf**](DefaultApi.md#getLedgerValueSelf) | **GET** /v1/ledger/value/self | Get your own available, locked, and borrowed USD value; and realized and unrealized PnL |
| [**getLedgerWithdrawRequestsBySelf**](DefaultApi.md#getLedgerWithdrawRequestsBySelf) | **GET** /v1/ledger/withdraw/requests/self | Get all pending withdrawal requests for the logged in user |
| [**getLedgerWithdrawRequestsByUserID**](DefaultApi.md#getLedgerWithdrawRequestsByUserID) | **GET** /v1/ledger/withdraw/requests/{user_id} | Get all pending withdrawal requests for this user |
| [**getOrderById**](DefaultApi.md#getOrderById) | **GET** /v1/orders/{order_id} | Get order by ID |
| [**getOrderbookById**](DefaultApi.md#getOrderbookById) | **GET** /v1/orderbooks/{order_book_id} | Get orderbook by ID |
| [**getOrderbookDepth**](DefaultApi.md#getOrderbookDepth) | **GET** /v1/orderbooks/{order_book_id}/depth | Get the aggregated price levels for a specific orderbook (L2 market depth) |
| [**getOrderbookOrders**](DefaultApi.md#getOrderbookOrders) | **GET** /v1/orderbooks/{order_book_id}/orders | Get all open orders for a specific orderbook (L3 market depth) |
| [**getOrderbookStats**](DefaultApi.md#getOrderbookStats) | **GET** /v1/orderbooks/{order_book_id}/stats | Get orderbook stats |
| [**getOrderbookStatsStream**](DefaultApi.md#getOrderbookStatsStream) | **GET** /v1/orderbooks/{order_book_id}/stats/stream | Orderbook stats stream |
| [**getOrderbookSummary**](DefaultApi.md#getOrderbookSummary) | **GET** /v1/orderbooks/{order_book_id}/summary | Get summary of an orderbook |
| [**getOrderbookTop**](DefaultApi.md#getOrderbookTop) | **GET** /v1/orderbooks/{order_book_id}/top | Get the top price levels for a specific orderbook (L1 market depth) |
| [**getPLForSelfByAccount**](DefaultApi.md#getPLForSelfByAccount) | **GET** /v1/pl/self | Get account-by-account PL breakdown for the logged in user |
| [**getPoolPrice**](DefaultApi.md#getPoolPrice) | **GET** /v1/price/pool/{pool_id} | Get the current price of a pool |
| [**getRealizedPnlSettlements**](DefaultApi.md#getRealizedPnlSettlements) | **GET** /v1/realized_pnl_settlements | Get realized P&amp;L settlements with filters |
| [**getTradeById**](DefaultApi.md#getTradeById) | **GET** /v1/trades/{trade_id} | Get a trade by ID |
| [**getTrades**](DefaultApi.md#getTrades) | **GET** /v1/trades | Get a filtered, paginated list of trades |
| [**getTransactionById**](DefaultApi.md#getTransactionById) | **GET** /v1/transactions/{transaction_id} | Get a transaction by ID |
| [**getTransactions**](DefaultApi.md#getTransactions) | **GET** /v1/transactions | Get a filtered, paginated list of transactions |
| [**getTransactionsSettlements**](DefaultApi.md#getTransactionsSettlements) | **GET** /v1/transactions/settlements | Get transactions settlements with filters |
| [**getTransactionsStream**](DefaultApi.md#getTransactionsStream) | **GET** /v1/transactions/stream | Get transactions since a specific time, and open a stream for further updates |
| [**getUserById**](DefaultApi.md#getUserById) | **GET** /v1/user/{user_id} | Get user by ID (admin only) |
| [**getUserCouponPaymentsStream**](DefaultApi.md#getUserCouponPaymentsStream) | **GET** /v1/user/{user_id}/coupon_payments/stream | Stream user&#39;s coupon payment accruals in real time |
| [**getUserLedgerStream**](DefaultApi.md#getUserLedgerStream) | **GET** /v1/user/{user_id}/ledger/stream | Get a snapshot of user&#39;s ledger updates since a specific time, and opens a stream for further updates |
| [**getUserLeverageAccruedInterestStream**](DefaultApi.md#getUserLeverageAccruedInterestStream) | **GET** /v1/user/{user_id}/leverage/accrued_interest/stream | Stream user&#39;s current leverage accrued interest in real time |
| [**getUserOrderUpdatesStream**](DefaultApi.md#getUserOrderUpdatesStream) | **GET** /v1/user/{user_id}/orders/{order_book_id}/updates/stream | Get a snapshot of user&#39;s order updates for the given order book since a specific time, and opens a stream for further updates |
| [**getUserOrdersUpdatesStreamAll**](DefaultApi.md#getUserOrdersUpdatesStreamAll) | **GET** /v1/user/{user_id}/orders/all/updates/stream | Get a snapshot of user&#39;s order updates across all order books since a specific time, and opens a stream for further updates |
| [**getUserSelf**](DefaultApi.md#getUserSelf) | **GET** /v1/user/self | Get user details for the authenticated user |
| [**getUserTransactionsStream**](DefaultApi.md#getUserTransactionsStream) | **GET** /v1/user/{user_id}/transactions/stream | Get a snapshot of user&#39;s executed transactions since a specific time, and opens a stream for further updates |
| [**getUsers**](DefaultApi.md#getUsers) | **GET** /v1/user | Get all users (admin only) |
| [**getUsersAPIKeys**](DefaultApi.md#getUsersAPIKeys) | **GET** /v1/user/apikey | Get user&#39;s api keys |
| [**ledgerDeposit**](DefaultApi.md#ledgerDeposit) | **POST** /v1/ledger/deposit/{user_id} | Deposit assets into this user&#39;s account from the outside world |
| [**ledgerWithdraw**](DefaultApi.md#ledgerWithdraw) | **POST** /v1/ledger/withdraw/{user_id} | Withdraw assets from this user to the outside world |
| [**ledgerWithdrawRequest**](DefaultApi.md#ledgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/{user_id} | Initiate a withdrawal request for this user to the outside world |
| [**ledgerWithdrawRequestSelf**](DefaultApi.md#ledgerWithdrawRequestSelf) | **POST** /v1/ledger/withdraw/requests/self | Initiate a withdrawal request for the logged in user to the outside world |
| [**leverageGetAccruedInterestByUser**](DefaultApi.md#leverageGetAccruedInterestByUser) | **GET** /v1/leverage/accrued_interest/self | Get current accrued leverage interest for the user |
| [**leverageGetHistoricalInterestRates**](DefaultApi.md#leverageGetHistoricalInterestRates) | **GET** /v1/leverage/interest_rate/{asset_id}/historical | Get historical leverage interest rates for a specific asset |
| [**leverageGetInterestRate**](DefaultApi.md#leverageGetInterestRate) | **GET** /v1/leverage/interest_rate/{asset_id} | Get leverage interest rate for a specific asset |
| [**leverageIsolateCollateral**](DefaultApi.md#leverageIsolateCollateral) | **POST** /v1/leverage/isolate_collateral | Create an isolated position by transferring collateral to the position from the user&#39;s global collateral |
| [**leverageSupply**](DefaultApi.md#leverageSupply) | **POST** /v1/leverage/supply | Supply leverage for a specific asset |
| [**leverageUnite**](DefaultApi.md#leverageUnite) | **POST** /v1/leverage/unite | Combines all isolated positions into a single global position |
| [**leverageWithdraw**](DefaultApi.md#leverageWithdraw) | **POST** /v1/leverage/withdraw | Withdraw leverage for a specific asset |
| [**liquidityAdd**](DefaultApi.md#liquidityAdd) | **POST** /v1/liquidity/pool/{pool_id}/add | Add liquidity to a pool |
| [**liquiditySubtract**](DefaultApi.md#liquiditySubtract) | **POST** /v1/liquidity/pool/{pool_id}/remove | Subtract liquidity from a pool |
| [**listAccountsSelfV2**](DefaultApi.md#listAccountsSelfV2) | **GET** /v2/user/self/accounts | List all accounts for the authenticated user |
| [**listAssets**](DefaultApi.md#listAssets) | **GET** /v1/assets | List assets |
| [**listOrderBooks**](DefaultApi.md#listOrderBooks) | **GET** /v1/orderbooks | List order books |
| [**listOrders**](DefaultApi.md#listOrders) | **GET** /v1/orders | List all orders |
| [**listPositionAccountsSelf**](DefaultApi.md#listPositionAccountsSelf) | **GET** /v1/user/self/position_accounts | List all position accounts for the authenticated user |
| [**payLeverageGetAccruedInterest**](DefaultApi.md#payLeverageGetAccruedInterest) | **POST** /v1/leverage/accrued_interest/pay | Pay current accrued leverage interest for a specific user |
| [**rejectLedgerWithdrawRequest**](DefaultApi.md#rejectLedgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/{withdrawal_id}/reject | Reject a pending withdrawal request |
| [**revokeAPIKeyForUser**](DefaultApi.md#revokeAPIKeyForUser) | **PUT** /v1/user/apikey/{key_id}/revoke | Revoke apikey for a user |
| [**revokeAPIKeyForUserID**](DefaultApi.md#revokeAPIKeyForUserID) | **PUT** /v1/user/{user_id}/apikey/{key_id}/revoke | Revoke apikey for a user: admin or integrator only |
| [**settleLeverageAccruedInterest**](DefaultApi.md#settleLeverageAccruedInterest) | **POST** /v1/leverage/accrued_interest/settle | Settle current accrued leverage interest for a specific user |
| [**settleRealizedPnlRecord**](DefaultApi.md#settleRealizedPnlRecord) | **PUT** /v1/realized_pnl_settlements/{settlement_id} | Mark a realized P&amp;L settlement as settled |
| [**settleTransactionsSettlements**](DefaultApi.md#settleTransactionsSettlements) | **PUT** /v1/transactions/settlements | Settle multiple transactions settlements in batch |
| [**streamAssetPrices**](DefaultApi.md#streamAssetPrices) | **GET** /v1/prices/stream | Stream real-time asset prices as map objects |
| [**streamCandleData**](DefaultApi.md#streamCandleData) | **GET** /v1/charts/{order_book_id}/candle/stream | Get a snapshot of candlestick data from date provided, and open a stream for real-time updates |
| [**streamOrderBookBalances**](DefaultApi.md#streamOrderBookBalances) | **GET** /v1/orderbooks/{order_book_id}/balances/stream | Get a snapshot of base and quote balances for an order book and open a stream for real-time updates |
| [**streamOrderbookOpenOrders**](DefaultApi.md#streamOrderbookOpenOrders) | **GET** /v1/orderbooks/{order_book_id}/open/stream | Get a snapshot of open orders in an order book and open a stream for real-time updates |
| [**streamTrades**](DefaultApi.md#streamTrades) | **GET** /v1/trades/{order_book_id}/stream | Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates |
| [**transferAccountBalancesV2**](DefaultApi.md#transferAccountBalancesV2) | **POST** /v2/accounts/transfer_balances | Transfer available balance between a user&#39;s accounts |
| [**transferAvailableBalances**](DefaultApi.md#transferAvailableBalances) | **POST** /v1/positions/transfer_balances | Transfer available balance between a user&#39;s accounts (e.g. global to isolated position) |
| [**updateUserConfig**](DefaultApi.md#updateUserConfig) | **PUT** /v1/user/{user_id}/config | Update user configuration by ID |
| [**updateUserConfigSelf**](DefaultApi.md#updateUserConfigSelf) | **PUT** /v1/user/config/self | Update user configuration for the authenticated user |
| [**validateSubmitOrder**](DefaultApi.md#validateSubmitOrder) | **POST** /v1/orders/validate | Validate submit order request data |
| [**verifyUser**](DefaultApi.md#verifyUser) | **PUT** /v1/user/{user_id}/verify | Verify a user by ID |


<a id="approveLedgerWithdrawRequest"></a>
# **approveLedgerWithdrawRequest**
> WithdrawalInitiationResponseEnvelope approveLedgerWithdrawRequest(withdrawalId, withdrawalRequestReason)

Approve a pending withdrawal request

Approve a pending withdrawal request, allowing the transfer of assets to the outside world to proceed. Note that this does not interact with any external systems; it simply updates the status of the withdrawal request in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID withdrawalId = UUID.randomUUID(); // UUID | 
    WithdrawalRequestReason withdrawalRequestReason = new WithdrawalRequestReason(); // WithdrawalRequestReason | 
    try {
      WithdrawalInitiationResponseEnvelope result = apiInstance.approveLedgerWithdrawRequest(withdrawalId, withdrawalRequestReason);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#approveLedgerWithdrawRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **withdrawalId** | **UUID**|  | |
| **withdrawalRequestReason** | [**WithdrawalRequestReason**](WithdrawalRequestReason.md)|  | [optional] |

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Withdrawal request approved successfully |  -  |
| **400** | Bad request, e.g. invalid withdrawal ID format or request is not in a pending state |  -  |
| **404** | Withdrawal request not found |  -  |
| **403** | Forbidden, user does not have permission to approve this withdrawal request |  -  |
| **500** | Internal server error |  -  |

<a id="cancelAllOpenOrders"></a>
# **cancelAllOpenOrders**
> ListOrdersResponseEnvelope cancelAllOpenOrders(orderBookId, userId, accountId, orderKind)

Cancel all open orders, if user passes orderbook or account_id on query params it will cancel all orders on specific orderbook or account, admin can cancel user&#39;s orders on specific orderbook

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String orderBookId = "orderBookId_example"; // String | 
    UUID userId = UUID.randomUUID(); // UUID | 
    UUID accountId = UUID.randomUUID(); // UUID | 
    OrderKind orderKind = OrderKind.fromValue("LIMIT"); // OrderKind | 
    try {
      ListOrdersResponseEnvelope result = apiInstance.cancelAllOpenOrders(orderBookId, userId, accountId, orderKind);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#cancelAllOpenOrders");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **String**|  | [optional] |
| **userId** | **UUID**|  | [optional] |
| **accountId** | **UUID**|  | [optional] |
| **orderKind** | [**OrderKind**](.md)|  | [optional] [enum: LIMIT, MARKET] |

### Return type

[**ListOrdersResponseEnvelope**](ListOrdersResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | All open orders have been cancelled |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **500** | Internal server error |  -  |

<a id="cancelLedgerWithdrawRequest"></a>
# **cancelLedgerWithdrawRequest**
> WithdrawalInitiationResponseEnvelope cancelLedgerWithdrawRequest(withdrawalId, withdrawalRequestReason)

Cancel a pending withdrawal request

Cancel a pending withdrawal request, providing an optional reason for the cancellation.

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID withdrawalId = UUID.randomUUID(); // UUID | 
    WithdrawalRequestReason withdrawalRequestReason = new WithdrawalRequestReason(); // WithdrawalRequestReason | 
    try {
      WithdrawalInitiationResponseEnvelope result = apiInstance.cancelLedgerWithdrawRequest(withdrawalId, withdrawalRequestReason);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#cancelLedgerWithdrawRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **withdrawalId** | **UUID**|  | |
| **withdrawalRequestReason** | [**WithdrawalRequestReason**](WithdrawalRequestReason.md)|  | [optional] |

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Withdrawal request cancelled successfully |  -  |
| **400** | Bad request, e.g. invalid withdrawal ID format or request is not in a pending state |  -  |
| **404** | Withdrawal request not found |  -  |
| **403** | Forbidden, user does not have permission to cancel this withdrawal request |  -  |
| **500** | Internal server error |  -  |

<a id="cancelOrderById"></a>
# **cancelOrderById**
> CancelOrderResponseEnvelope cancelOrderById(orderId)

Cancel an order by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderId = UUID.randomUUID(); // UUID | 
    try {
      CancelOrderResponseEnvelope result = apiInstance.cancelOrderById(orderId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#cancelOrderById");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderId** | **UUID**|  | |

### Return type

[**CancelOrderResponseEnvelope**](CancelOrderResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order cancelled successfully |  -  |
| **400** | Bad request, e.g. invalid order ID format |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this order |  -  |
| **404** | Order not found |  -  |
| **500** | Internal server error |  -  |

<a id="claimLeverageGetAccruedInterest"></a>
# **claimLeverageGetAccruedInterest**
> ClaimLeverageAccruedInterestResponseEnvelope claimLeverageGetAccruedInterest(claimLeverageAccruedInterestRequest)

Claim current accrued leverage interest for a specific user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    ClaimLeverageAccruedInterestRequest claimLeverageAccruedInterestRequest = new ClaimLeverageAccruedInterestRequest(); // ClaimLeverageAccruedInterestRequest | 
    try {
      ClaimLeverageAccruedInterestResponseEnvelope result = apiInstance.claimLeverageGetAccruedInterest(claimLeverageAccruedInterestRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#claimLeverageGetAccruedInterest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **claimLeverageAccruedInterestRequest** | [**ClaimLeverageAccruedInterestRequest**](ClaimLeverageAccruedInterestRequest.md)|  | |

### Return type

[**ClaimLeverageAccruedInterestResponseEnvelope**](ClaimLeverageAccruedInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Current leverage accrued interest claimed successfully |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **500** | Internal server error |  -  |

<a id="closeIsolatedAccountV2"></a>
# **closeIsolatedAccountV2**
> ClosePositionResponseEnvelope closeIsolatedAccountV2(closeAccountRequest)

Close an isolated account, repaying the borrowed

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    CloseAccountRequest closeAccountRequest = new CloseAccountRequest(); // CloseAccountRequest | 
    try {
      ClosePositionResponseEnvelope result = apiInstance.closeIsolatedAccountV2(closeAccountRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#closeIsolatedAccountV2");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **closeAccountRequest** | [**CloseAccountRequest**](CloseAccountRequest.md)|  | |

### Return type

[**ClosePositionResponseEnvelope**](ClosePositionResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Isolated account closed |  -  |
| **400** | Bad request, e.g. missing required fields |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this route |  -  |
| **404** | Not found, e.g. order_book or account not found |  -  |
| **500** | Internal server error |  -  |

<a id="closeIsolatedPosition"></a>
# **closeIsolatedPosition**
> ClosePositionResponseEnvelope closeIsolatedPosition(closePositionRequest)

Close isolated positions, repaying the borrowed

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    ClosePositionRequest closePositionRequest = new ClosePositionRequest(); // ClosePositionRequest | 
    try {
      ClosePositionResponseEnvelope result = apiInstance.closeIsolatedPosition(closePositionRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#closeIsolatedPosition");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **closePositionRequest** | [**ClosePositionRequest**](ClosePositionRequest.md)|  | |

### Return type

[**ClosePositionResponseEnvelope**](ClosePositionResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Isolated Position Closed |  -  |
| **400** | Bad request, e.g. missing required fields |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this route |  -  |
| **404** | Not found, e.g. order_book or position not found |  -  |
| **500** | Internal server error |  -  |

<a id="createAPIKeyForUser"></a>
# **createAPIKeyForUser**
> CreateAPIKeyResponseEnvelope createAPIKeyForUser(createAPIKeyRequest)

Create apikey for a user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    CreateAPIKeyRequest createAPIKeyRequest = new CreateAPIKeyRequest(); // CreateAPIKeyRequest | 
    try {
      CreateAPIKeyResponseEnvelope result = apiInstance.createAPIKeyForUser(createAPIKeyRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createAPIKeyForUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **createAPIKeyRequest** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  | |

### Return type

[**CreateAPIKeyResponseEnvelope**](CreateAPIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | APIKey created |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="createAPIKeyForUserID"></a>
# **createAPIKeyForUserID**
> CreateAPIKeyResponseEnvelope createAPIKeyForUserID(userId, createAPIKeyRequest)

Create apikey for a user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String userId = "userId_example"; // String | 
    CreateAPIKeyRequest createAPIKeyRequest = new CreateAPIKeyRequest(); // CreateAPIKeyRequest | 
    try {
      CreateAPIKeyResponseEnvelope result = apiInstance.createAPIKeyForUserID(userId, createAPIKeyRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createAPIKeyForUserID");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **String**|  | |
| **createAPIKeyRequest** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  | |

### Return type

[**CreateAPIKeyResponseEnvelope**](CreateAPIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | APIKey created |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="createConditionalOrder"></a>
# **createConditionalOrder**
> CreateConditionalOrderResponseEnvelope createConditionalOrder(createConditionalOrderRequest)

Create a new conditional orders

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    CreateConditionalOrderRequest createConditionalOrderRequest = new CreateConditionalOrderRequest(); // CreateConditionalOrderRequest | 
    try {
      CreateConditionalOrderResponseEnvelope result = apiInstance.createConditionalOrder(createConditionalOrderRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createConditionalOrder");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **createConditionalOrderRequest** | [**CreateConditionalOrderRequest**](CreateConditionalOrderRequest.md)|  | |

### Return type

[**CreateConditionalOrderResponseEnvelope**](CreateConditionalOrderResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Conditional orders are created |  -  |
| **400** | Bad request, e.g. missing required fields |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **500** | Internal server error |  -  |

<a id="createNewIsolatedAccountV2"></a>
# **createNewIsolatedAccountV2**
> NewIsolatedAccountResponseV2Envelope createNewIsolatedAccountV2(newIsolatedAccountRequestV2)

Create a new isolated account for a user transferring available assets into the account

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    NewIsolatedAccountRequestV2 newIsolatedAccountRequestV2 = new NewIsolatedAccountRequestV2(); // NewIsolatedAccountRequestV2 | 
    try {
      NewIsolatedAccountResponseV2Envelope result = apiInstance.createNewIsolatedAccountV2(newIsolatedAccountRequestV2);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createNewIsolatedAccountV2");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **newIsolatedAccountRequestV2** | [**NewIsolatedAccountRequestV2**](NewIsolatedAccountRequestV2.md)|  | |

### Return type

[**NewIsolatedAccountResponseV2Envelope**](NewIsolatedAccountResponseV2Envelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Isolated account created |  -  |
| **400** | Bad request, e.g. missing required fields |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **409** | Conflict, e.g. the requested amount is not available to transfer |  -  |
| **500** | Internal server error |  -  |

<a id="createOrder"></a>
# **createOrder**
> CreateOrderResponseEnvelope createOrder(createOrderRequest)

Create a new order

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    CreateOrderRequest createOrderRequest = new CreateOrderRequest(); // CreateOrderRequest | 
    try {
      CreateOrderResponseEnvelope result = apiInstance.createOrder(createOrderRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createOrder");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **createOrderRequest** | [**CreateOrderRequest**](CreateOrderRequest.md)|  | |

### Return type

[**CreateOrderResponseEnvelope**](CreateOrderResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Order created |  -  |
| **400** | Bad request, e.g. missing required fields |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **500** | Internal server error |  -  |

<a id="createUser"></a>
# **createUser**
> UserCreatedResponseEnvelope createUser(createIntegratorUserRequest)

Create a new user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    CreateIntegratorUserRequest createIntegratorUserRequest = new CreateIntegratorUserRequest(); // CreateIntegratorUserRequest | 
    try {
      UserCreatedResponseEnvelope result = apiInstance.createUser(createIntegratorUserRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **createIntegratorUserRequest** | [**CreateIntegratorUserRequest**](CreateIntegratorUserRequest.md)|  | |

### Return type

[**UserCreatedResponseEnvelope**](UserCreatedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | User created |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **500** | Internal server error |  -  |

<a id="deleteUser"></a>
# **deleteUser**
> UserDeletedResponseEnvelope deleteUser(userId)

Delete user by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    try {
      UserDeletedResponseEnvelope result = apiInstance.deleteUser(userId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#deleteUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |

### Return type

[**UserDeletedResponseEnvelope**](UserDeletedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User deleted |  -  |
| **401** | Unauthorized, only admin can delete users |  -  |
| **403** | Forbidden, only admin can delete users |  -  |
| **404** | User not found |  -  |

<a id="getAPIKeysForUserID"></a>
# **getAPIKeysForUserID**
> APIKeyResponseEnvelope getAPIKeysForUserID(userId)

Get user&#39;s api keys: admin or integrator only

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String userId = "userId_example"; // String | 
    try {
      APIKeyResponseEnvelope result = apiInstance.getAPIKeysForUserID(userId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getAPIKeysForUserID");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **String**|  | |

### Return type

[**APIKeyResponseEnvelope**](APIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A list of existing api-keys |  -  |
| **400** | Bad request, e.g. invalid path parameters |  -  |
| **500** | Internal server error |  -  |

<a id="getAllAssetPrices"></a>
# **getAllAssetPrices**
> ListAssetPriceResponseEnvelope getAllAssetPrices()

Get the current price of all assets

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      ListAssetPriceResponseEnvelope result = apiInstance.getAllAssetPrices();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getAllAssetPrices");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListAssetPriceResponseEnvelope**](ListAssetPriceResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Current prices of all assets |  -  |
| **500** | Internal server error |  -  |

<a id="getAllPositions"></a>
# **getAllPositions**
> AllPositionsResponseEnvelope getAllPositions()

Get all users&#39; positions

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      AllPositionsResponseEnvelope result = apiInstance.getAllPositions();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getAllPositions");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AllPositionsResponseEnvelope**](AllPositionsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User positions |  -  |
| **500** | Internal server error |  -  |

<a id="getAllWithdrawalRequests"></a>
# **getAllWithdrawalRequests**
> AllWithdrawalInitiationsResponseEnvelope getAllWithdrawalRequests(status)

Get all withdrawal requests

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String status = "status_example"; // String | 
    try {
      AllWithdrawalInitiationsResponseEnvelope result = apiInstance.getAllWithdrawalRequests(status);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getAllWithdrawalRequests");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **status** | **String**|  | [optional] |

### Return type

[**AllWithdrawalInitiationsResponseEnvelope**](AllWithdrawalInitiationsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of withdrawal requests |  -  |
| **500** | Internal server error |  -  |

<a id="getAssetById"></a>
# **getAssetById**
> GetAssetByIDResponseEnvelope getAssetById(assetId)

Get asset by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID assetId = UUID.randomUUID(); // UUID | 
    try {
      GetAssetByIDResponseEnvelope result = apiInstance.getAssetById(assetId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getAssetById");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **assetId** | **UUID**|  | |

### Return type

[**GetAssetByIDResponseEnvelope**](GetAssetByIDResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Asset details |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Asset not found |  -  |

<a id="getAssetPrice"></a>
# **getAssetPrice**
> AssetPriceResponseEnvelope getAssetPrice(assetId)

Get the current price of an asset

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID assetId = UUID.randomUUID(); // UUID | 
    try {
      AssetPriceResponseEnvelope result = apiInstance.getAssetPrice(assetId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getAssetPrice");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **assetId** | **UUID**|  | |

### Return type

[**AssetPriceResponseEnvelope**](AssetPriceResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Current price of the asset |  -  |
| **400** | Bad request, e.g. invalid ID format |  -  |
| **404** | Asset not found |  -  |
| **500** | Internal server error |  -  |

<a id="getAssetYTMById"></a>
# **getAssetYTMById**
> GetAssetYTMByIDResponseEnvelope getAssetYTMById(assetId)

Get annualized yield to maturity for a bond asset

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID assetId = UUID.randomUUID(); // UUID | 
    try {
      GetAssetYTMByIDResponseEnvelope result = apiInstance.getAssetYTMById(assetId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getAssetYTMById");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **assetId** | **UUID**|  | |

### Return type

[**GetAssetYTMByIDResponseEnvelope**](GetAssetYTMByIDResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Asset YTM details |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Asset not found |  -  |

<a id="getAssetsStream"></a>
# **getAssetsStream**
> List&lt;StreamAssetsEntry&gt; getAssetsStream(since, until)

Get all inserts or updates for assets

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime until = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      List<StreamAssetsEntry> result = apiInstance.getAssetsStream(since, until);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getAssetsStream");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **since** | **OffsetDateTime**|  | [optional] |
| **until** | **OffsetDateTime**|  | [optional] |

### Return type

[**List&lt;StreamAssetsEntry&gt;**](StreamAssetsEntry.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Asset&#39;s stream |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this route |  -  |
| **500** | Internal server error |  -  |

<a id="getCandleData"></a>
# **getCandleData**
> ListCandlesResponseEnvelope getCandleData(orderBookId, start, end, resolution)

Get candlestick data for an orderbook

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String orderBookId = "orderBookId_example"; // String | 
    OffsetDateTime start = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime end = OffsetDateTime.now(); // OffsetDateTime | 
    CandleResolution resolution = CandleResolution.fromValue("1m"); // CandleResolution | 
    try {
      ListCandlesResponseEnvelope result = apiInstance.getCandleData(orderBookId, start, end, resolution);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getCandleData");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **String**|  | |
| **start** | **OffsetDateTime**|  | |
| **end** | **OffsetDateTime**|  | |
| **resolution** | [**CandleResolution**](.md)|  | [optional] [enum: 1m, 5m, 15m, 1h, 4h, 1d] |

### Return type

[**ListCandlesResponseEnvelope**](ListCandlesResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Candlestick data |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getCouponPaymentsByAssetId"></a>
# **getCouponPaymentsByAssetId**
> ListCouponPaymentsResponseEnvelope getCouponPaymentsByAssetId(assetId)

Get coupon payments for a bond asset

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID assetId = UUID.randomUUID(); // UUID | 
    try {
      ListCouponPaymentsResponseEnvelope result = apiInstance.getCouponPaymentsByAssetId(assetId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getCouponPaymentsByAssetId");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **assetId** | **UUID**|  | |

### Return type

[**ListCouponPaymentsResponseEnvelope**](ListCouponPaymentsResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of coupon payments |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Asset not found or no coupon payments available |  -  |

<a id="getL1Depth"></a>
# **getL1Depth**
> GetTopOfBookResponseEnvelope getL1Depth(orderBookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      GetTopOfBookResponseEnvelope result = apiInstance.getL1Depth(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getL1Depth");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**GetTopOfBookResponseEnvelope**](GetTopOfBookResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Top price levels data |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getL2Depth"></a>
# **getL2Depth**
> ListOrderBookDepthResponseEnvelope getL2Depth(orderBookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      ListOrderBookDepthResponseEnvelope result = apiInstance.getL2Depth(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getL2Depth");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**ListOrderBookDepthResponseEnvelope**](ListOrderBookDepthResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order book depth data |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getL3Depth"></a>
# **getL3Depth**
> ListOrdersResponseEnvelope getL3Depth(orderBookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      ListOrdersResponseEnvelope result = apiInstance.getL3Depth(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getL3Depth");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**ListOrdersResponseEnvelope**](ListOrdersResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of orders for the orderbook |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerAccountsSelfV2"></a>
# **getLedgerAccountsSelfV2**
> LedgerAccountsResponseV2Envelope getLedgerAccountsSelfV2()

Get your own accounts

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      LedgerAccountsResponseV2Envelope result = apiInstance.getLedgerAccountsSelfV2();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerAccountsSelfV2");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**LedgerAccountsResponseV2Envelope**](LedgerAccountsResponseV2Envelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User accounts |  -  |
| **400** | Bad request, e.g. invalid user ID format |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerBalancesSelf"></a>
# **getLedgerBalancesSelf**
> UserBalanceResponseEnvelope getLedgerBalancesSelf()

Get your own available, locked, and borrowed assets

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      UserBalanceResponseEnvelope result = apiInstance.getLedgerBalancesSelf();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerBalancesSelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserBalanceResponseEnvelope**](UserBalanceResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User balances |  -  |
| **400** | Bad request, e.g. invalid user ID format |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerInterestSelf"></a>
# **getLedgerInterestSelf**
> UserInterestResponseEnvelope getLedgerInterestSelf()

Get your own interest

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      UserInterestResponseEnvelope result = apiInstance.getLedgerInterestSelf();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerInterestSelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserInterestResponseEnvelope**](UserInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User interest |  -  |
| **400** | Bad request, e.g. invalid user ID format |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerModule"></a>
# **getLedgerModule**
> LedgerModuleResponseEnvelope getLedgerModule()

Get the entire module object, including unborrowed leverage assets and total leverage trackers

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      LedgerModuleResponseEnvelope result = apiInstance.getLedgerModule();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerModule");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**LedgerModuleResponseEnvelope**](LedgerModuleResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Leverage module object |  -  |
| **404** | Module not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerModuleByAsset"></a>
# **getLedgerModuleByAsset**
> LedgerModuleByAssetResponseEnvelope getLedgerModuleByAsset(assetId)

Get the module object for a single asset ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID assetId = UUID.randomUUID(); // UUID | 
    try {
      LedgerModuleByAssetResponseEnvelope result = apiInstance.getLedgerModuleByAsset(assetId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerModuleByAsset");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **assetId** | **UUID**|  | |

### Return type

[**LedgerModuleByAssetResponseEnvelope**](LedgerModuleByAssetResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Leverage module balance for asset |  -  |
| **400** | Bad request, e.g. invalid asset ID format |  -  |
| **404** | Asset not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerPositionsSelf"></a>
# **getLedgerPositionsSelf**
> UserPositionResponseEnvelope getLedgerPositionsSelf()

Get your own positions

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      UserPositionResponseEnvelope result = apiInstance.getLedgerPositionsSelf();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerPositionsSelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserPositionResponseEnvelope**](UserPositionResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User positions |  -  |
| **400** | Bad request, e.g. invalid user ID format |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerValueSelf"></a>
# **getLedgerValueSelf**
> UserValueResponseEnvelope getLedgerValueSelf()

Get your own available, locked, and borrowed USD value; and realized and unrealized PnL

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      UserValueResponseEnvelope result = apiInstance.getLedgerValueSelf();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerValueSelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserValueResponseEnvelope**](UserValueResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User value |  -  |
| **400** | Bad request, e.g. invalid user ID format |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerWithdrawRequestsBySelf"></a>
# **getLedgerWithdrawRequestsBySelf**
> AllWithdrawalInitiationsResponseEnvelope getLedgerWithdrawRequestsBySelf(status)

Get all pending withdrawal requests for the logged in user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String status = "status_example"; // String | 
    try {
      AllWithdrawalInitiationsResponseEnvelope result = apiInstance.getLedgerWithdrawRequestsBySelf(status);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerWithdrawRequestsBySelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **status** | **String**|  | [optional] |

### Return type

[**AllWithdrawalInitiationsResponseEnvelope**](AllWithdrawalInitiationsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of pending withdrawal requests for the logged in user |  -  |
| **400** | Bad request, e.g. invalid user ID format |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getLedgerWithdrawRequestsByUserID"></a>
# **getLedgerWithdrawRequestsByUserID**
> AllWithdrawalInitiationsResponseEnvelope getLedgerWithdrawRequestsByUserID(userId, status)

Get all pending withdrawal requests for this user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    String status = "status_example"; // String | 
    try {
      AllWithdrawalInitiationsResponseEnvelope result = apiInstance.getLedgerWithdrawRequestsByUserID(userId, status);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getLedgerWithdrawRequestsByUserID");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **status** | **String**|  | [optional] |

### Return type

[**AllWithdrawalInitiationsResponseEnvelope**](AllWithdrawalInitiationsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of pending withdrawal requests for this user |  -  |
| **400** | Bad request, e.g. invalid user ID format |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getOrderById"></a>
# **getOrderById**
> OrderResponseEnvelope getOrderById(orderId)

Get order by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderId = UUID.randomUUID(); // UUID | 
    try {
      OrderResponseEnvelope result = apiInstance.getOrderById(orderId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getOrderById");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderId** | **UUID**|  | |

### Return type

[**OrderResponseEnvelope**](OrderResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order details |  -  |
| **400** | Bad request, e.g. invalid order ID format |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this order |  -  |
| **404** | Order not found |  -  |
| **500** | Internal server error |  -  |

<a id="getOrderbookById"></a>
# **getOrderbookById**
> OrderBookResponseEnvelope getOrderbookById(orderBookId)

Get orderbook by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      OrderBookResponseEnvelope result = apiInstance.getOrderbookById(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getOrderbookById");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**OrderBookResponseEnvelope**](OrderBookResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Orderbook details |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Orderbook not found |  -  |

<a id="getOrderbookDepth"></a>
# **getOrderbookDepth**
> ListOrderBookDepthResponseEnvelope getOrderbookDepth(orderBookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      ListOrderBookDepthResponseEnvelope result = apiInstance.getOrderbookDepth(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getOrderbookDepth");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**ListOrderBookDepthResponseEnvelope**](ListOrderBookDepthResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Order book depth data |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getOrderbookOrders"></a>
# **getOrderbookOrders**
> ListOrdersResponseEnvelope getOrderbookOrders(orderBookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      ListOrdersResponseEnvelope result = apiInstance.getOrderbookOrders(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getOrderbookOrders");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**ListOrdersResponseEnvelope**](ListOrdersResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of orders for the orderbook |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getOrderbookStats"></a>
# **getOrderbookStats**
> OrderbookStatsResponseEnvelope getOrderbookStats(orderBookId)

Get orderbook stats

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      OrderbookStatsResponseEnvelope result = apiInstance.getOrderbookStats(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getOrderbookStats");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**OrderbookStatsResponseEnvelope**](OrderbookStatsResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Orderbook stats details |  -  |
| **204** | No Content |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Orderbook not found |  -  |

<a id="getOrderbookStatsStream"></a>
# **getOrderbookStatsStream**
> OrderbookStats getOrderbookStatsStream(orderBookId)

Orderbook stats stream

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      OrderbookStats result = apiInstance.getOrderbookStatsStream(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getOrderbookStatsStream");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**OrderbookStats**](OrderbookStats.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Orderbook stats stream |  -  |
| **204** | No Content |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getOrderbookSummary"></a>
# **getOrderbookSummary**
> OrderBookSummaryResponseEnvelope getOrderbookSummary(orderBookId)

Get summary of an orderbook

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      OrderBookSummaryResponseEnvelope result = apiInstance.getOrderbookSummary(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getOrderbookSummary");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**OrderBookSummaryResponseEnvelope**](OrderBookSummaryResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Orderbook summary data |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getOrderbookTop"></a>
# **getOrderbookTop**
> GetTopOfBookResponseEnvelope getOrderbookTop(orderBookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    try {
      GetTopOfBookResponseEnvelope result = apiInstance.getOrderbookTop(orderBookId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getOrderbookTop");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |

### Return type

[**GetTopOfBookResponseEnvelope**](GetTopOfBookResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Top price levels data |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="getPLForSelfByAccount"></a>
# **getPLForSelfByAccount**
> PLResponseEnvelope getPLForSelfByAccount()

Get account-by-account PL breakdown for the logged in user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      PLResponseEnvelope result = apiInstance.getPLForSelfByAccount();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getPLForSelfByAccount");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PLResponseEnvelope**](PLResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of user accounts with a PL breakdown by asset and summary |  -  |
| **401** | Unauthorized, user is not logged in |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getPoolPrice"></a>
# **getPoolPrice**
> PoolPriceResponseEnvelope getPoolPrice(poolId)

Get the current price of a pool

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID poolId = UUID.randomUUID(); // UUID | 
    try {
      PoolPriceResponseEnvelope result = apiInstance.getPoolPrice(poolId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getPoolPrice");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **poolId** | **UUID**|  | |

### Return type

[**PoolPriceResponseEnvelope**](PoolPriceResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Current price of the pool |  -  |
| **400** | Bad request, e.g. invalid ID format |  -  |
| **404** | Pool not found |  -  |
| **500** | Internal server error |  -  |

<a id="getRealizedPnlSettlements"></a>
# **getRealizedPnlSettlements**
> GetRealizedPnlSettlementsResponseEnvelope getRealizedPnlSettlements(userId, tenantId, positionId, createdAfter, createdBefore, settledAfter, settledBefore, isSettled)

Get realized P&amp;L settlements with filters

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    UUID tenantId = UUID.randomUUID(); // UUID | 
    UUID positionId = UUID.randomUUID(); // UUID | 
    OffsetDateTime createdAfter = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime createdBefore = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime settledAfter = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime settledBefore = OffsetDateTime.now(); // OffsetDateTime | 
    Boolean isSettled = true; // Boolean | 
    try {
      GetRealizedPnlSettlementsResponseEnvelope result = apiInstance.getRealizedPnlSettlements(userId, tenantId, positionId, createdAfter, createdBefore, settledAfter, settledBefore, isSettled);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getRealizedPnlSettlements");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | [optional] |
| **tenantId** | **UUID**|  | [optional] |
| **positionId** | **UUID**|  | [optional] |
| **createdAfter** | **OffsetDateTime**|  | [optional] |
| **createdBefore** | **OffsetDateTime**|  | [optional] |
| **settledAfter** | **OffsetDateTime**|  | [optional] |
| **settledBefore** | **OffsetDateTime**|  | [optional] |
| **isSettled** | **Boolean**|  | [optional] |

### Return type

[**GetRealizedPnlSettlementsResponseEnvelope**](GetRealizedPnlSettlementsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of realized P&amp;L settlements with filters applied |  -  |
| **401** | Unauthorized, user is not logged in |  -  |
| **403** | Forbidden, user does not have access |  -  |
| **500** | Internal server error |  -  |

<a id="getTradeById"></a>
# **getTradeById**
> TradeResponseEnvelope getTradeById(tradeId)

Get a trade by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID tradeId = UUID.randomUUID(); // UUID | 
    try {
      TradeResponseEnvelope result = apiInstance.getTradeById(tradeId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getTradeById");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tradeId** | **UUID**|  | |

### Return type

[**TradeResponseEnvelope**](TradeResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Trade details |  -  |
| **400** | Bad request, e.g. invalid ID format |  -  |
| **404** | Trade not found |  -  |
| **500** | Internal server error |  -  |

<a id="getTrades"></a>
# **getTrades**
> ListTradeResponseEnvelope getTrades(orderBookIds, userIds, start, end, page, limit)

Get a filtered, paginated list of trades

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    List<String> orderBookIds = Arrays.asList(); // List<String> | 
    List<UUID> userIds = Arrays.asList(); // List<UUID> | 
    OffsetDateTime start = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime end = OffsetDateTime.now(); // OffsetDateTime | 
    Integer page = 1; // Integer | 
    Integer limit = 100; // Integer | 
    try {
      ListTradeResponseEnvelope result = apiInstance.getTrades(orderBookIds, userIds, start, end, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getTrades");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookIds** | [**List&lt;String&gt;**](String.md)|  | [optional] |
| **userIds** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional] |
| **start** | **OffsetDateTime**|  | [optional] |
| **end** | **OffsetDateTime**|  | [optional] |
| **page** | **Integer**|  | [optional] [default to 1] |
| **limit** | **Integer**|  | [optional] [default to 100] |

### Return type

[**ListTradeResponseEnvelope**](ListTradeResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of trades |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **404** | No trades found |  -  |
| **500** | Internal server error |  -  |

<a id="getTransactionById"></a>
# **getTransactionById**
> TransactionResponseEnvelope getTransactionById(transactionId)

Get a transaction by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID transactionId = UUID.randomUUID(); // UUID | 
    try {
      TransactionResponseEnvelope result = apiInstance.getTransactionById(transactionId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getTransactionById");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **transactionId** | **UUID**|  | |

### Return type

[**TransactionResponseEnvelope**](TransactionResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Transaction details |  -  |
| **400** | Bad request, e.g. invalid ID format |  -  |
| **404** | Transaction not found |  -  |
| **500** | Internal server error |  -  |

<a id="getTransactions"></a>
# **getTransactions**
> ListTransactionsResponseEnvelope getTransactions(pools, userIds, txKinds, start, end, tenantId, page, limit)

Get a filtered, paginated list of transactions

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    List<String> pools = Arrays.asList(); // List<String> | 
    List<UUID> userIds = Arrays.asList(); // List<UUID> | 
    List<TransactionKind> txKinds = Arrays.asList(); // List<TransactionKind> | 
    OffsetDateTime start = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime end = OffsetDateTime.now(); // OffsetDateTime | 
    UUID tenantId = UUID.randomUUID(); // UUID | 
    Integer page = 1; // Integer | 
    Integer limit = 100; // Integer | 
    try {
      ListTransactionsResponseEnvelope result = apiInstance.getTransactions(pools, userIds, txKinds, start, end, tenantId, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getTransactions");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **pools** | [**List&lt;String&gt;**](String.md)|  | [optional] |
| **userIds** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional] |
| **txKinds** | [**List&lt;TransactionKind&gt;**](TransactionKind.md)|  | [optional] |
| **start** | **OffsetDateTime**|  | [optional] |
| **end** | **OffsetDateTime**|  | [optional] |
| **tenantId** | **UUID**|  | [optional] |
| **page** | **Integer**|  | [optional] [default to 1] |
| **limit** | **Integer**|  | [optional] [default to 100] |

### Return type

[**ListTransactionsResponseEnvelope**](ListTransactionsResponseEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of transactions |  -  |
| **400** | Bad request, e.g. insufficient funds or invalid parameters |  -  |
| **500** | Internal server error |  -  |

<a id="getTransactionsSettlements"></a>
# **getTransactionsSettlements**
> TransactionsSettlementsResponseEnvelope getTransactionsSettlements(tenantId, userId, positionId, txKind, createdAfter, createdBefore, settledAfter, settledBefore, isSettled)

Get transactions settlements with filters

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String tenantId = "tenantId_example"; // String | Tenant ID to filter settlements
    UUID userId = UUID.randomUUID(); // UUID | User ID to filter settlements
    UUID positionId = UUID.randomUUID(); // UUID | Position ID to filter settlements
    String txKind = "txKind_example"; // String | Transaction kind to filter settlements
    OffsetDateTime createdAfter = OffsetDateTime.now(); // OffsetDateTime | Filter settlements created after this time
    OffsetDateTime createdBefore = OffsetDateTime.now(); // OffsetDateTime | Filter settlements created before this time
    OffsetDateTime settledAfter = OffsetDateTime.now(); // OffsetDateTime | Filter settlements settled after this time
    OffsetDateTime settledBefore = OffsetDateTime.now(); // OffsetDateTime | Filter settlements settled before this time
    Boolean isSettled = true; // Boolean | Filter settlements by settlement status
    try {
      TransactionsSettlementsResponseEnvelope result = apiInstance.getTransactionsSettlements(tenantId, userId, positionId, txKind, createdAfter, createdBefore, settledAfter, settledBefore, isSettled);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getTransactionsSettlements");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **tenantId** | **String**| Tenant ID to filter settlements | [optional] |
| **userId** | **UUID**| User ID to filter settlements | [optional] |
| **positionId** | **UUID**| Position ID to filter settlements | [optional] |
| **txKind** | **String**| Transaction kind to filter settlements | [optional] |
| **createdAfter** | **OffsetDateTime**| Filter settlements created after this time | [optional] |
| **createdBefore** | **OffsetDateTime**| Filter settlements created before this time | [optional] |
| **settledAfter** | **OffsetDateTime**| Filter settlements settled after this time | [optional] |
| **settledBefore** | **OffsetDateTime**| Filter settlements settled before this time | [optional] |
| **isSettled** | **Boolean**| Filter settlements by settlement status | [optional] |

### Return type

[**TransactionsSettlementsResponseEnvelope**](TransactionsSettlementsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A list of transaction settlements |  -  |
| **400** | Bad request |  -  |
| **404** | No settlements found |  -  |
| **500** | Internal server error |  -  |

<a id="getTransactionsStream"></a>
# **getTransactionsStream**
> List&lt;StreamTransactionsEntry&gt; getTransactionsStream(since)

Get transactions since a specific time, and open a stream for further updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthQuery
    ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
    apiKeyAuthQuery.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthQuery.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      List<StreamTransactionsEntry> result = apiInstance.getTransactionsStream(since);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getTransactionsStream");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **since** | **OffsetDateTime**|  | [optional] |

### Return type

[**List&lt;StreamTransactionsEntry&gt;**](StreamTransactionsEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Transactions stream |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to these transactions |  -  |
| **500** | Internal server error |  -  |

<a id="getUserById"></a>
# **getUserById**
> UserEnvelope getUserById(userId)

Get user by ID (admin only)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    try {
      UserEnvelope result = apiInstance.getUserById(userId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserById");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |

### Return type

[**UserEnvelope**](UserEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User details |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getUserCouponPaymentsStream"></a>
# **getUserCouponPaymentsStream**
> StreamUserCouponPaymentsResponse getUserCouponPaymentsStream(userId)

Stream user&#39;s coupon payment accruals in real time

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthQuery
    ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
    apiKeyAuthQuery.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthQuery.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    try {
      StreamUserCouponPaymentsResponse result = apiInstance.getUserCouponPaymentsStream(userId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserCouponPaymentsStream");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |

### Return type

[**StreamUserCouponPaymentsResponse**](StreamUserCouponPaymentsResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User&#39;s coupon payments stream |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this data |  -  |
| **404** | User not found or no coupon payments available |  -  |
| **500** | Internal server error |  -  |

<a id="getUserLedgerStream"></a>
# **getUserLedgerStream**
> List&lt;StreamPositionsEntry&gt; getUserLedgerStream(userId)

Get a snapshot of user&#39;s ledger updates since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthQuery
    ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
    apiKeyAuthQuery.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthQuery.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    try {
      List<StreamPositionsEntry> result = apiInstance.getUserLedgerStream(userId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserLedgerStream");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |

### Return type

[**List&lt;StreamPositionsEntry&gt;**](StreamPositionsEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User&#39;s ledger stream |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this ledger |  -  |
| **404** | User not found or no ledger entries available |  -  |
| **500** | Internal server error |  -  |

<a id="getUserLeverageAccruedInterestStream"></a>
# **getUserLeverageAccruedInterestStream**
> StreamCurrentLeverageAccruedInterestResponse getUserLeverageAccruedInterestStream(userId)

Stream user&#39;s current leverage accrued interest in real time

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthQuery
    ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
    apiKeyAuthQuery.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthQuery.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    try {
      StreamCurrentLeverageAccruedInterestResponse result = apiInstance.getUserLeverageAccruedInterestStream(userId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserLeverageAccruedInterestStream");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |

### Return type

[**StreamCurrentLeverageAccruedInterestResponse**](StreamCurrentLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User&#39;s leverage accrued interest stream |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this data |  -  |
| **404** | User not found or no leverage accrued interest available |  -  |
| **500** | Internal server error |  -  |

<a id="getUserOrderUpdatesStream"></a>
# **getUserOrderUpdatesStream**
> List&lt;StreamOrderUpdatesEntry&gt; getUserOrderUpdatesStream(userId, orderBookId, since)

Get a snapshot of user&#39;s order updates for the given order book since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthQuery
    ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
    apiKeyAuthQuery.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthQuery.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      List<StreamOrderUpdatesEntry> result = apiInstance.getUserOrderUpdatesStream(userId, orderBookId, since);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserOrderUpdatesStream");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **orderBookId** | **UUID**|  | |
| **since** | **OffsetDateTime**|  | [optional] |

### Return type

[**List&lt;StreamOrderUpdatesEntry&gt;**](StreamOrderUpdatesEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User&#39;s orders stream |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **404** | User not found or no orders available |  -  |
| **500** | Internal server error |  -  |

<a id="getUserOrdersUpdatesStreamAll"></a>
# **getUserOrdersUpdatesStreamAll**
> List&lt;StreamOrderUpdatesEntry&gt; getUserOrdersUpdatesStreamAll(userId, since)

Get a snapshot of user&#39;s order updates across all order books since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthQuery
    ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
    apiKeyAuthQuery.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthQuery.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      List<StreamOrderUpdatesEntry> result = apiInstance.getUserOrdersUpdatesStreamAll(userId, since);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserOrdersUpdatesStreamAll");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **since** | **OffsetDateTime**|  | [optional] |

### Return type

[**List&lt;StreamOrderUpdatesEntry&gt;**](StreamOrderUpdatesEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User&#39;s orders stream |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **404** | User not found or no orders available |  -  |
| **500** | Internal server error |  -  |

<a id="getUserSelf"></a>
# **getUserSelf**
> UserEnvelope getUserSelf()

Get user details for the authenticated user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      UserEnvelope result = apiInstance.getUserSelf();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserSelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserEnvelope**](UserEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User details |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="getUserTransactionsStream"></a>
# **getUserTransactionsStream**
> List&lt;StreamTransactionsEntry&gt; getUserTransactionsStream(userId, since)

Get a snapshot of user&#39;s executed transactions since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthQuery
    ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
    apiKeyAuthQuery.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthQuery.setApiKeyPrefix("Token");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      List<StreamTransactionsEntry> result = apiInstance.getUserTransactionsStream(userId, since);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserTransactionsStream");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **since** | **OffsetDateTime**|  | [optional] |

### Return type

[**List&lt;StreamTransactionsEntry&gt;**](StreamTransactionsEntry.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User&#39;s transactions stream |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this transactions |  -  |
| **404** | User not found or no transactions available |  -  |
| **500** | Internal server error |  -  |

<a id="getUsers"></a>
# **getUsers**
> ListUsersResponseEnvelope getUsers(id, limit, offset, email, firstName, lastName, countryOfDomicile)

Get all users (admin only)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID id = UUID.randomUUID(); // UUID | 
    Integer limit = 100; // Integer | 
    Integer offset = 0; // Integer | 
    String email = "email_example"; // String | 
    String firstName = "firstName_example"; // String | 
    String lastName = "lastName_example"; // String | 
    CountryCode countryOfDomicile = CountryCode.fromValue("AF"); // CountryCode | 
    try {
      ListUsersResponseEnvelope result = apiInstance.getUsers(id, limit, offset, email, firstName, lastName, countryOfDomicile);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUsers");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **UUID**|  | [optional] |
| **limit** | **Integer**|  | [optional] [default to 100] |
| **offset** | **Integer**|  | [optional] [default to 0] |
| **email** | **String**|  | [optional] |
| **firstName** | **String**|  | [optional] |
| **lastName** | **String**|  | [optional] |
| **countryOfDomicile** | [**CountryCode**](.md)|  | [optional] [enum: AF, AX, AL, DZ, AS, AD, AO, AI, AQ, AG, AR, AM, AW, AU, AT, AZ, BS, BH, BD, BB, BY, BE, BZ, BJ, BM, BT, BO, BQ, BA, BW, BV, BR, IO, BN, BG, BF, BI, CV, KH, CM, CA, KY, CF, TD, CL, CN, CX, CC, CO, KM, CG, CD, CK, CR, CI, HR, CU, CW, CY, CZ, DK, DJ, DM, DO, EC, EG, SV, GQ, ER, EE, SZ, ET, FK, FO, FJ, FI, FR, GF, PF, TF, GA, GM, GE, DE, GH, GI, GR, GL, GD, GP, GU, GT, GG, GN, GW, GY, HT, HM, VA, HN, HK, HU, IS, IN, ID, IR, IQ, IE, IM, IL, IT, JM, JP, JE, JO, KZ, KE, KI, KP, KR, KW, KG, LA, LV, LB, LS, LR, LY, LI, LT, LU, MO, MG, MW, MY, MV, ML, MT, MH, MQ, MR, MU, YT, MX, FM, MD, MC, MN, ME, MS, MA, MZ, MM, NA, NR, NP, NL, NC, NZ, NI, NE, NG, NU, NF, MK, MP, NO, OM, PK, PW, PS, PA, PG, PY, PE, PH, PN, PL, PT, PR, QA, RE, RO, RU, RW, BL, SH, KN, LC, MF, PM, VC, WS, SM, ST, SA, SN, RS, SC, SL, SG, SX, SK, SI, SB, SO, ZA, GS, SS, ES, LK, SD, SR, SJ, SE, CH, SY, TW, TJ, TZ, TH, TL, TG, TK, TO, TT, TN, TR, TM, TC, TV, UG, UA, AE, GB, US, UM, UY, UZ, VU, VE, VN, VG, VI, WF, EH, YE, ZM, ZW] |

### Return type

[**ListUsersResponseEnvelope**](ListUsersResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A list of users |  -  |
| **500** | Internal server error |  -  |

<a id="getUsersAPIKeys"></a>
# **getUsersAPIKeys**
> APIKeyResponseEnvelope getUsersAPIKeys()

Get user&#39;s api keys

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      APIKeyResponseEnvelope result = apiInstance.getUsersAPIKeys();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUsersAPIKeys");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**APIKeyResponseEnvelope**](APIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A list of existing api-keys |  -  |
| **400** | Bad request, e.g. invalid path parameters |  -  |
| **500** | Internal server error |  -  |

<a id="ledgerDeposit"></a>
# **ledgerDeposit**
> FundUserResponseEnvelope ledgerDeposit(userId, fundUserRequest)

Deposit assets into this user&#39;s account from the outside world

Deposit assets into this user&#39;s account from the outside world. Note that this does not interact with any external systems; it simply adds the amount to the user&#39;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    FundUserRequest fundUserRequest = new FundUserRequest(); // FundUserRequest | 
    try {
      FundUserResponseEnvelope result = apiInstance.ledgerDeposit(userId, fundUserRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#ledgerDeposit");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **fundUserRequest** | [**FundUserRequest**](FundUserRequest.md)|  | |

### Return type

[**FundUserResponseEnvelope**](FundUserResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Deposit successful |  -  |
| **400** | Bad request, e.g. invalid parameters or insufficient funds |  -  |
| **500** | Internal server error |  -  |

<a id="ledgerWithdraw"></a>
# **ledgerWithdraw**
> FundUserResponseEnvelope ledgerWithdraw(userId, defundUserRequest, status)

Withdraw assets from this user to the outside world

Withdraw assets from this user&#39;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#39;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    DefundUserRequest defundUserRequest = new DefundUserRequest(); // DefundUserRequest | 
    String status = "status_example"; // String | 
    try {
      FundUserResponseEnvelope result = apiInstance.ledgerWithdraw(userId, defundUserRequest, status);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#ledgerWithdraw");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **defundUserRequest** | [**DefundUserRequest**](DefundUserRequest.md)|  | |
| **status** | **String**|  | [optional] |

### Return type

[**FundUserResponseEnvelope**](FundUserResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Withdraw successful |  -  |
| **400** | Bad request, e.g. invalid parameters or insufficient funds |  -  |
| **500** | Internal server error |  -  |

<a id="ledgerWithdrawRequest"></a>
# **ledgerWithdrawRequest**
> WithdrawalInitiationResponseEnvelope ledgerWithdrawRequest(userId, defundUserRequest)

Initiate a withdrawal request for this user to the outside world

Withdraw assets from this user&#39;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#39;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    DefundUserRequest defundUserRequest = new DefundUserRequest(); // DefundUserRequest | 
    try {
      WithdrawalInitiationResponseEnvelope result = apiInstance.ledgerWithdrawRequest(userId, defundUserRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#ledgerWithdrawRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **defundUserRequest** | [**DefundUserRequest**](DefundUserRequest.md)|  | |

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Withdraw request initiation successful |  -  |
| **400** | Bad request, e.g. invalid parameters or insufficient funds |  -  |
| **500** | Internal server error |  -  |

<a id="ledgerWithdrawRequestSelf"></a>
# **ledgerWithdrawRequestSelf**
> WithdrawalInitiationResponseEnvelope ledgerWithdrawRequestSelf(userId, defundUserRequest)

Initiate a withdrawal request for the logged in user to the outside world

Withdraw assets from the logged in user&#39;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#39;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    DefundUserRequest defundUserRequest = new DefundUserRequest(); // DefundUserRequest | 
    try {
      WithdrawalInitiationResponseEnvelope result = apiInstance.ledgerWithdrawRequestSelf(userId, defundUserRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#ledgerWithdrawRequestSelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **defundUserRequest** | [**DefundUserRequest**](DefundUserRequest.md)|  | |

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Withdraw request initiation successful |  -  |
| **400** | Bad request, e.g. invalid parameters or insufficient funds |  -  |
| **500** | Internal server error |  -  |

<a id="leverageGetAccruedInterestByUser"></a>
# **leverageGetAccruedInterestByUser**
> CurrentLeverageAccruedInterestResponseEnvelope leverageGetAccruedInterestByUser(positionId, assetId)

Get current accrued leverage interest for the user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID positionId = UUID.randomUUID(); // UUID | 
    UUID assetId = UUID.randomUUID(); // UUID | 
    try {
      CurrentLeverageAccruedInterestResponseEnvelope result = apiInstance.leverageGetAccruedInterestByUser(positionId, assetId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#leverageGetAccruedInterestByUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **positionId** | **UUID**|  | [optional] |
| **assetId** | **UUID**|  | [optional] |

### Return type

[**CurrentLeverageAccruedInterestResponseEnvelope**](CurrentLeverageAccruedInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Current leverage accrued interest retrieved successfully |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **500** | Internal server error |  -  |

<a id="leverageGetHistoricalInterestRates"></a>
# **leverageGetHistoricalInterestRates**
> HistoricalLeverageInterestRatesResponseEnvelope leverageGetHistoricalInterestRates(assetId, start, end)

Get historical leverage interest rates for a specific asset

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID assetId = UUID.randomUUID(); // UUID | 
    OffsetDateTime start = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime end = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      HistoricalLeverageInterestRatesResponseEnvelope result = apiInstance.leverageGetHistoricalInterestRates(assetId, start, end);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#leverageGetHistoricalInterestRates");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **assetId** | **UUID**|  | |
| **start** | **OffsetDateTime**|  | [optional] |
| **end** | **OffsetDateTime**|  | [optional] |

### Return type

[**HistoricalLeverageInterestRatesResponseEnvelope**](HistoricalLeverageInterestRatesResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Historical leverage interest rates retrieved successfully |  -  |
| **400** | Bad request, e.g. invalid time parameter or end before/equal start |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **500** | Internal server error |  -  |

<a id="leverageGetInterestRate"></a>
# **leverageGetInterestRate**
> LeverageInterestRateResponseEnvelope leverageGetInterestRate(assetId, start, end)

Get leverage interest rate for a specific asset

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID assetId = UUID.randomUUID(); // UUID | 
    OffsetDateTime start = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime end = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      LeverageInterestRateResponseEnvelope result = apiInstance.leverageGetInterestRate(assetId, start, end);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#leverageGetInterestRate");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **assetId** | **UUID**|  | |
| **start** | **OffsetDateTime**|  | [optional] |
| **end** | **OffsetDateTime**|  | [optional] |

### Return type

[**LeverageInterestRateResponseEnvelope**](LeverageInterestRateResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Leverage interest rate retrieved successfully |  -  |
| **400** | Bad request, e.g. invalid/mismatched time parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **404** | No utilization data found for the selected window or asset not found |  -  |
| **500** | Internal server error |  -  |

<a id="leverageIsolateCollateral"></a>
# **leverageIsolateCollateral**
> IsolateCollateralResponse leverageIsolateCollateral(isolateCollateralRequest)

Create an isolated position by transferring collateral to the position from the user&#39;s global collateral

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    IsolateCollateralRequest isolateCollateralRequest = new IsolateCollateralRequest(); // IsolateCollateralRequest | 
    try {
      IsolateCollateralResponse result = apiInstance.leverageIsolateCollateral(isolateCollateralRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#leverageIsolateCollateral");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **isolateCollateralRequest** | [**IsolateCollateralRequest**](IsolateCollateralRequest.md)|  | |

### Return type

[**IsolateCollateralResponse**](IsolateCollateralResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Leverage position isolated |  -  |
| **400** | Bad request, e.g. insufficient collateral or invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **404** | Leverage position not found |  -  |
| **409** | Conflict, e.g. the requested amount is not available to transfer |  -  |
| **500** | Internal server error |  -  |

<a id="leverageSupply"></a>
# **leverageSupply**
> SupplyResponseEnvelope leverageSupply(supplyRequest)

Supply leverage for a specific asset

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    SupplyRequest supplyRequest = new SupplyRequest(); // SupplyRequest | 
    try {
      SupplyResponseEnvelope result = apiInstance.leverageSupply(supplyRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#leverageSupply");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **supplyRequest** | [**SupplyRequest**](SupplyRequest.md)|  | |

### Return type

[**SupplyResponseEnvelope**](SupplyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Supply successful |  -  |
| **400** | Bad request, e.g. insufficient collateral or invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **500** | Internal server error |  -  |

<a id="leverageUnite"></a>
# **leverageUnite**
> UnitePositionResponseEnvelope leverageUnite(unitePositionRequest)

Combines all isolated positions into a single global position

Combines all isolated positions into a single global position

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UnitePositionRequest unitePositionRequest = new UnitePositionRequest(); // UnitePositionRequest | 
    try {
      UnitePositionResponseEnvelope result = apiInstance.leverageUnite(unitePositionRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#leverageUnite");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **unitePositionRequest** | [**UnitePositionRequest**](UnitePositionRequest.md)|  | |

### Return type

[**UnitePositionResponseEnvelope**](UnitePositionResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Leverage position combined |  -  |
| **400** | Bad request, e.g. insufficient collateral or invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **404** | Leverage position not found |  -  |
| **409** | Conflict, e.g. the requested amount is not available to transfer |  -  |
| **500** | Internal server error |  -  |

<a id="leverageWithdraw"></a>
# **leverageWithdraw**
> WithdrawResponseEnvelope leverageWithdraw(withdrawRequest)

Withdraw leverage for a specific asset

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    WithdrawRequest withdrawRequest = new WithdrawRequest(); // WithdrawRequest | 
    try {
      WithdrawResponseEnvelope result = apiInstance.leverageWithdraw(withdrawRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#leverageWithdraw");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **withdrawRequest** | [**WithdrawRequest**](WithdrawRequest.md)|  | |

### Return type

[**WithdrawResponseEnvelope**](WithdrawResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Withdraw successful |  -  |
| **400** | Bad request, e.g. insufficient collateral or invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **500** | Internal server error |  -  |

<a id="liquidityAdd"></a>
# **liquidityAdd**
> LiquidityResponseEnvelope liquidityAdd(poolId, liquidityRequest)

Add liquidity to a pool

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID poolId = UUID.randomUUID(); // UUID | 
    LiquidityRequest liquidityRequest = new LiquidityRequest(); // LiquidityRequest | 
    try {
      LiquidityResponseEnvelope result = apiInstance.liquidityAdd(poolId, liquidityRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#liquidityAdd");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **poolId** | **UUID**|  | |
| **liquidityRequest** | [**LiquidityRequest**](LiquidityRequest.md)|  | |

### Return type

[**LiquidityResponseEnvelope**](LiquidityResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Liquidity added |  -  |
| **400** | Bad request, e.g. insufficient funds or invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **404** | Pool not found |  -  |
| **409** | Conflict, e.g. the requested amount is not available to transfer |  -  |
| **500** | Internal server error |  -  |

<a id="liquiditySubtract"></a>
# **liquiditySubtract**
> LiquidityResponseEnvelope liquiditySubtract(poolId, liquidityRequest)

Subtract liquidity from a pool

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID poolId = UUID.randomUUID(); // UUID | 
    LiquidityRequest liquidityRequest = new LiquidityRequest(); // LiquidityRequest | 
    try {
      LiquidityResponseEnvelope result = apiInstance.liquiditySubtract(poolId, liquidityRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#liquiditySubtract");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **poolId** | **UUID**|  | |
| **liquidityRequest** | [**LiquidityRequest**](LiquidityRequest.md)|  | |

### Return type

[**LiquidityResponseEnvelope**](LiquidityResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Liquidity subtracted |  -  |
| **400** | Bad request, e.g. insufficient funds or invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **404** | Pool not found |  -  |
| **409** | Conflict, e.g. the requested amount is not available to transfer |  -  |
| **500** | Internal server error |  -  |

<a id="listAccountsSelfV2"></a>
# **listAccountsSelfV2**
> ListAccountsResponseV2Envelope listAccountsSelfV2()

List all accounts for the authenticated user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      ListAccountsResponseV2Envelope result = apiInstance.listAccountsSelfV2();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#listAccountsSelfV2");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListAccountsResponseV2Envelope**](ListAccountsResponseV2Envelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of accounts including the account id, the account name, and global account indicator |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="listAssets"></a>
# **listAssets**
> ResponseEnvelopeOfListAssets listAssets(createdAfter, createdBefore, assetKind, canAddLiquidity, canDirectBorrow, canOnboard, canTrade, canVirtualBorrow, page, limit)

List assets

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    OffsetDateTime createdAfter = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime createdBefore = OffsetDateTime.now(); // OffsetDateTime | 
    AssetKind assetKind = AssetKind.fromValue("BOND"); // AssetKind | Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE)
    Boolean canAddLiquidity = true; // Boolean | 
    Boolean canDirectBorrow = true; // Boolean | 
    Boolean canOnboard = true; // Boolean | 
    Boolean canTrade = true; // Boolean | 
    Boolean canVirtualBorrow = true; // Boolean | 
    Integer page = 1; // Integer | 
    Integer limit = 100; // Integer | 
    try {
      ResponseEnvelopeOfListAssets result = apiInstance.listAssets(createdAfter, createdBefore, assetKind, canAddLiquidity, canDirectBorrow, canOnboard, canTrade, canVirtualBorrow, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#listAssets");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **createdAfter** | **OffsetDateTime**|  | [optional] |
| **createdBefore** | **OffsetDateTime**|  | [optional] |
| **assetKind** | [**AssetKind**](.md)| Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE) | [optional] [enum: BOND, CURRENCY, INTEREST, POOL_SHARE] |
| **canAddLiquidity** | **Boolean**|  | [optional] |
| **canDirectBorrow** | **Boolean**|  | [optional] |
| **canOnboard** | **Boolean**|  | [optional] |
| **canTrade** | **Boolean**|  | [optional] |
| **canVirtualBorrow** | **Boolean**|  | [optional] |
| **page** | **Integer**|  | [optional] [default to 1] |
| **limit** | **Integer**|  | [optional] [default to 100] |

### Return type

[**ResponseEnvelopeOfListAssets**](ResponseEnvelopeOfListAssets.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A list of assets |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **500** | Internal server error |  -  |

<a id="listOrderBooks"></a>
# **listOrderBooks**
> ListOrderbookResponseEnvelope listOrderBooks(status, baseAssetId, quoteAssetId, page, limit)

List order books

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    OrderBookStatus status = OrderBookStatus.fromValue("CLOSED"); // OrderBookStatus | 
    UUID baseAssetId = UUID.randomUUID(); // UUID | 
    UUID quoteAssetId = UUID.randomUUID(); // UUID | 
    Integer page = 1; // Integer | 
    Integer limit = 100; // Integer | 
    try {
      ListOrderbookResponseEnvelope result = apiInstance.listOrderBooks(status, baseAssetId, quoteAssetId, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#listOrderBooks");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **status** | [**OrderBookStatus**](.md)|  | [optional] [enum: CLOSED, OPEN, SUSPENDED] |
| **baseAssetId** | **UUID**|  | [optional] |
| **quoteAssetId** | **UUID**|  | [optional] |
| **page** | **Integer**|  | [optional] [default to 1] |
| **limit** | **Integer**|  | [optional] [default to 100] |

### Return type

[**ListOrderbookResponseEnvelope**](ListOrderbookResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A list of orderbooks |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | No orderbooks found |  -  |
| **500** | Internal server error |  -  |

<a id="listOrders"></a>
# **listOrders**
> ListOrdersResponseEnvelope listOrders(orderBookId, kind, status, side, from, to, page, limit)

List all orders

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    List<UUID> orderBookId = Arrays.asList(); // List<UUID> | 
    List<OrderKind> kind = Arrays.asList(); // List<OrderKind> | 
    List<OrderStatus> status = Arrays.asList(); // List<OrderStatus> | 
    Side side = Side.fromValue("BUY"); // Side | 
    OffsetDateTime from = OffsetDateTime.now(); // OffsetDateTime | 
    OffsetDateTime to = OffsetDateTime.now(); // OffsetDateTime | 
    Integer page = 1; // Integer | 
    Integer limit = 100; // Integer | 
    try {
      ListOrdersResponseEnvelope result = apiInstance.listOrders(orderBookId, kind, status, side, from, to, page, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#listOrders");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional] |
| **kind** | [**List&lt;OrderKind&gt;**](OrderKind.md)|  | [optional] |
| **status** | [**List&lt;OrderStatus&gt;**](OrderStatus.md)|  | [optional] |
| **side** | [**Side**](.md)|  | [optional] [enum: BUY, SELL] |
| **from** | **OffsetDateTime**|  | [optional] |
| **to** | **OffsetDateTime**|  | [optional] |
| **page** | **Integer**|  | [optional] [default to 1] |
| **limit** | **Integer**|  | [optional] [default to 100] |

### Return type

[**ListOrdersResponseEnvelope**](ListOrdersResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A list of orders |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **404** | No orders found |  -  |
| **500** | Internal server error |  -  |

<a id="listPositionAccountsSelf"></a>
# **listPositionAccountsSelf**
> ListPositionAccountsResponseEnvelope listPositionAccountsSelf()

List all position accounts for the authenticated user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      ListPositionAccountsResponseEnvelope result = apiInstance.listPositionAccountsSelf();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#listPositionAccountsSelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListPositionAccountsResponseEnvelope**](ListPositionAccountsResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of position accounts including the position id, the position name, and global account indicator |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="payLeverageGetAccruedInterest"></a>
# **payLeverageGetAccruedInterest**
> PayLeverageAccruedInterestResponseEnvelope payLeverageGetAccruedInterest(payLeverageAccruedInterestRequest)

Pay current accrued leverage interest for a specific user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    PayLeverageAccruedInterestRequest payLeverageAccruedInterestRequest = new PayLeverageAccruedInterestRequest(); // PayLeverageAccruedInterestRequest | 
    try {
      PayLeverageAccruedInterestResponseEnvelope result = apiInstance.payLeverageGetAccruedInterest(payLeverageAccruedInterestRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#payLeverageGetAccruedInterest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **payLeverageAccruedInterestRequest** | [**PayLeverageAccruedInterestRequest**](PayLeverageAccruedInterestRequest.md)|  | |

### Return type

[**PayLeverageAccruedInterestResponseEnvelope**](PayLeverageAccruedInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Current leverage accrued interest paid successfully |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **500** | Internal server error |  -  |

<a id="rejectLedgerWithdrawRequest"></a>
# **rejectLedgerWithdrawRequest**
> WithdrawalInitiationResponseEnvelope rejectLedgerWithdrawRequest(withdrawalId, withdrawalRequestReason)

Reject a pending withdrawal request

Reject a pending withdrawal request, providing a reason for the rejection. Note that this does not interact with any external systems; it simply updates the status of the withdrawal request in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID withdrawalId = UUID.randomUUID(); // UUID | 
    WithdrawalRequestReason withdrawalRequestReason = new WithdrawalRequestReason(); // WithdrawalRequestReason | 
    try {
      WithdrawalInitiationResponseEnvelope result = apiInstance.rejectLedgerWithdrawRequest(withdrawalId, withdrawalRequestReason);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#rejectLedgerWithdrawRequest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **withdrawalId** | **UUID**|  | |
| **withdrawalRequestReason** | [**WithdrawalRequestReason**](WithdrawalRequestReason.md)|  | |

### Return type

[**WithdrawalInitiationResponseEnvelope**](WithdrawalInitiationResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Withdrawal request rejected successfully |  -  |
| **400** | Bad request, e.g. invalid withdrawal ID format or request is not in a pending state |  -  |
| **404** | Withdrawal request not found |  -  |
| **403** | Forbidden, user does not have permission to reject this withdrawal request |  -  |
| **500** | Internal server error |  -  |

<a id="revokeAPIKeyForUser"></a>
# **revokeAPIKeyForUser**
> RevokeAPIKeyResponseEnvelope revokeAPIKeyForUser(keyId)

Revoke apikey for a user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String keyId = "keyId_example"; // String | 
    try {
      RevokeAPIKeyResponseEnvelope result = apiInstance.revokeAPIKeyForUser(keyId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#revokeAPIKeyForUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **keyId** | **String**|  | |

### Return type

[**RevokeAPIKeyResponseEnvelope**](RevokeAPIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | APIKey revoked |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="revokeAPIKeyForUserID"></a>
# **revokeAPIKeyForUserID**
> RevokeAPIKeyResponseEnvelope revokeAPIKeyForUserID(userId, keyId)

Revoke apikey for a user: admin or integrator only

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String userId = "userId_example"; // String | 
    String keyId = "keyId_example"; // String | 
    try {
      RevokeAPIKeyResponseEnvelope result = apiInstance.revokeAPIKeyForUserID(userId, keyId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#revokeAPIKeyForUserID");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **String**|  | |
| **keyId** | **String**|  | |

### Return type

[**RevokeAPIKeyResponseEnvelope**](RevokeAPIKeyResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | APIKey revoked |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="settleLeverageAccruedInterest"></a>
# **settleLeverageAccruedInterest**
> SettleLeverageAccruedInterestResponseEnvelope settleLeverageAccruedInterest(settleLeverageAccruedInterestRequest)

Settle current accrued leverage interest for a specific user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    SettleLeverageAccruedInterestRequest settleLeverageAccruedInterestRequest = new SettleLeverageAccruedInterestRequest(); // SettleLeverageAccruedInterestRequest | 
    try {
      SettleLeverageAccruedInterestResponseEnvelope result = apiInstance.settleLeverageAccruedInterest(settleLeverageAccruedInterestRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#settleLeverageAccruedInterest");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **settleLeverageAccruedInterestRequest** | [**SettleLeverageAccruedInterestRequest**](SettleLeverageAccruedInterestRequest.md)|  | |

### Return type

[**SettleLeverageAccruedInterestResponseEnvelope**](SettleLeverageAccruedInterestResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Current leverage accrued interest settled successfully |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **401** | Unauthorized, e.g. user not logged in or invalid credentials |  -  |
| **500** | Internal server error |  -  |

<a id="settleRealizedPnlRecord"></a>
# **settleRealizedPnlRecord**
> SettleRealizedPnlRecordResponseEnvelope settleRealizedPnlRecord(settlementId)

Mark a realized P&amp;L settlement as settled

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID settlementId = UUID.randomUUID(); // UUID | 
    try {
      SettleRealizedPnlRecordResponseEnvelope result = apiInstance.settleRealizedPnlRecord(settlementId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#settleRealizedPnlRecord");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **settlementId** | **UUID**|  | |

### Return type

[**SettleRealizedPnlRecordResponseEnvelope**](SettleRealizedPnlRecordResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | The realized P&amp;L settlement record has been marked as settled |  -  |
| **401** | Unauthorized, user is not logged in |  -  |
| **403** | Forbidden, user does not have access |  -  |
| **500** | Internal server error |  -  |

<a id="settleTransactionsSettlements"></a>
# **settleTransactionsSettlements**
> TransactionsSettlementsResponse settleTransactionsSettlements(transactionsSettlementRequest)

Settle multiple transactions settlements in batch

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    TransactionsSettlementRequest transactionsSettlementRequest = new TransactionsSettlementRequest(); // TransactionsSettlementRequest | 
    try {
      TransactionsSettlementsResponse result = apiInstance.settleTransactionsSettlements(transactionsSettlementRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#settleTransactionsSettlements");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **transactionsSettlementRequest** | [**TransactionsSettlementRequest**](TransactionsSettlementRequest.md)|  | |

### Return type

[**TransactionsSettlementsResponse**](TransactionsSettlementsResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Settlements updated |  -  |
| **400** | Bad request |  -  |
| **404** | No transactions for settlement found |  -  |
| **500** | Internal server error |  -  |

<a id="streamAssetPrices"></a>
# **streamAssetPrices**
> Map&lt;String, AssetPrice&gt; streamAssetPrices(since, assetId)

Stream real-time asset prices as map objects

Opens a WebSocket stream for real-time asset price updates. First message contains all current prices, subsequent messages contain only changed prices. Data is sent as JSON objects keyed by asset ID.

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    UUID assetId = UUID.randomUUID(); // UUID | 
    try {
      Map<String, AssetPrice> result = apiInstance.streamAssetPrices(since, assetId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#streamAssetPrices");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **since** | **OffsetDateTime**|  | [optional] |
| **assetId** | **UUID**|  | [optional] |

### Return type

[**Map&lt;String, AssetPrice&gt;**](AssetPrice.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Real-time stream of asset prices. First message: all current prices. Subsequent messages: only changed prices. |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **500** | Internal server error |  -  |

<a id="streamCandleData"></a>
# **streamCandleData**
> List&lt;StreamCandlesEntry&gt; streamCandleData(orderBookId, since, resolution)

Get a snapshot of candlestick data from date provided, and open a stream for real-time updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String orderBookId = "orderBookId_example"; // String | 
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    CandleResolution resolution = CandleResolution.fromValue("1m"); // CandleResolution | 
    try {
      List<StreamCandlesEntry> result = apiInstance.streamCandleData(orderBookId, since, resolution);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#streamCandleData");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **String**|  | |
| **since** | **OffsetDateTime**|  | [optional] |
| **resolution** | [**CandleResolution**](.md)|  | [optional] [enum: 1m, 5m, 15m, 1h, 4h, 1d] |

### Return type

[**List&lt;StreamCandlesEntry&gt;**](StreamCandlesEntry.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Stream opened successfully |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="streamOrderBookBalances"></a>
# **streamOrderBookBalances**
> List&lt;StreamOrderBookBalanceEntry&gt; streamOrderBookBalances(orderBookId, since)

Get a snapshot of base and quote balances for an order book and open a stream for real-time updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      List<StreamOrderBookBalanceEntry> result = apiInstance.streamOrderBookBalances(orderBookId, since);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#streamOrderBookBalances");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |
| **since** | **OffsetDateTime**|  | [optional] |

### Return type

[**List&lt;StreamOrderBookBalanceEntry&gt;**](StreamOrderBookBalanceEntry.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Stream opened successfully |  -  |
| **400** | Bad request, e.g. invalid order book ID format |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="streamOrderbookOpenOrders"></a>
# **streamOrderbookOpenOrders**
> LiveOrderbook streamOrderbookOpenOrders(orderBookId, since)

Get a snapshot of open orders in an order book and open a stream for real-time updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      LiveOrderbook result = apiInstance.streamOrderbookOpenOrders(orderBookId, since);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#streamOrderbookOpenOrders");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |
| **since** | **OffsetDateTime**|  | [optional] |

### Return type

[**LiveOrderbook**](LiveOrderbook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Stream opened successfully |  -  |
| **400** | Bad request, e.g. invalid order book ID format |  -  |
| **404** | Orderbook not found |  -  |
| **500** | Internal server error |  -  |

<a id="streamTrades"></a>
# **streamTrades**
> List&lt;StreamTradesEntry&gt; streamTrades(orderBookId, since)

Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID orderBookId = UUID.randomUUID(); // UUID | 
    OffsetDateTime since = OffsetDateTime.now(); // OffsetDateTime | 
    try {
      List<StreamTradesEntry> result = apiInstance.streamTrades(orderBookId, since);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#streamTrades");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **orderBookId** | **UUID**|  | |
| **since** | **OffsetDateTime**|  | [optional] |

### Return type

[**List&lt;StreamTradesEntry&gt;**](StreamTradesEntry.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Real-time trade updates |  -  |
| **400** | Bad request, e.g. invalid parameters |  -  |
| **500** | Internal server error |  -  |

<a id="transferAccountBalancesV2"></a>
# **transferAccountBalancesV2**
> TransferAccountBalancesResponseEnvelope transferAccountBalancesV2(transferAccountBalancesRequest)

Transfer available balance between a user&#39;s accounts

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    TransferAccountBalancesRequest transferAccountBalancesRequest = new TransferAccountBalancesRequest(); // TransferAccountBalancesRequest | 
    try {
      TransferAccountBalancesResponseEnvelope result = apiInstance.transferAccountBalancesV2(transferAccountBalancesRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#transferAccountBalancesV2");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **transferAccountBalancesRequest** | [**TransferAccountBalancesRequest**](TransferAccountBalancesRequest.md)|  | |

### Return type

[**TransferAccountBalancesResponseEnvelope**](TransferAccountBalancesResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Isolated account created |  -  |
| **400** | Bad request, e.g. missing required fields |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **409** | Conflict, e.g. the requested amount is not available to transfer |  -  |
| **500** | Internal server error |  -  |

<a id="transferAvailableBalances"></a>
# **transferAvailableBalances**
> TransferBalancesResponseEnvelope transferAvailableBalances(transferBalancesRequest)

Transfer available balance between a user&#39;s accounts (e.g. global to isolated position)

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    TransferBalancesRequest transferBalancesRequest = new TransferBalancesRequest(); // TransferBalancesRequest | 
    try {
      TransferBalancesResponseEnvelope result = apiInstance.transferAvailableBalances(transferBalancesRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#transferAvailableBalances");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **transferBalancesRequest** | [**TransferBalancesRequest**](TransferBalancesRequest.md)|  | |

### Return type

[**TransferBalancesResponseEnvelope**](TransferBalancesResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Isolated Position Created |  -  |
| **400** | Bad request, e.g. missing required fields |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **409** | Conflict, e.g. the requested amount is not available to transfer |  -  |
| **500** | Internal server error |  -  |

<a id="updateUserConfig"></a>
# **updateUserConfig**
> UserUpdatedResponseEnvelope updateUserConfig(userId, updateUserConfigRequest)

Update user configuration by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    UpdateUserConfigRequest updateUserConfigRequest = new UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
    try {
      UserUpdatedResponseEnvelope result = apiInstance.updateUserConfig(userId, updateUserConfigRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#updateUserConfig");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |
| **updateUserConfigRequest** | [**UpdateUserConfigRequest**](UpdateUserConfigRequest.md)|  | |

### Return type

[**UserUpdatedResponseEnvelope**](UserUpdatedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User configuration updated |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="updateUserConfigSelf"></a>
# **updateUserConfigSelf**
> UserUpdatedResponseEnvelope updateUserConfigSelf(updateUserConfigRequest)

Update user configuration for the authenticated user

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UpdateUserConfigRequest updateUserConfigRequest = new UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
    try {
      UserUpdatedResponseEnvelope result = apiInstance.updateUserConfigSelf(updateUserConfigRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#updateUserConfigSelf");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **updateUserConfigRequest** | [**UpdateUserConfigRequest**](UpdateUserConfigRequest.md)|  | |

### Return type

[**UserUpdatedResponseEnvelope**](UserUpdatedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User configuration updated |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

<a id="validateSubmitOrder"></a>
# **validateSubmitOrder**
> ValidateSubmitOrderResponse validateSubmitOrder(validateSubmitOrderRequest)

Validate submit order request data

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    ValidateSubmitOrderRequest validateSubmitOrderRequest = new ValidateSubmitOrderRequest(); // ValidateSubmitOrderRequest | 
    try {
      ValidateSubmitOrderResponse result = apiInstance.validateSubmitOrder(validateSubmitOrderRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#validateSubmitOrder");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **validateSubmitOrderRequest** | [**ValidateSubmitOrderRequest**](ValidateSubmitOrderRequest.md)|  | |

### Return type

[**ValidateSubmitOrderResponse**](ValidateSubmitOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Validated submit order request |  -  |
| **400** | Bad request, e.g. missing required fields |  -  |
| **401** | Unauthorized, user not logged in or does not have access to this orderbook |  -  |
| **500** | Internal server error |  -  |

<a id="verifyUser"></a>
# **verifyUser**
> UserUpdatedResponseEnvelope verifyUser(userId)

Verify a user by ID

### Example
```java
// Import classes:
import tech.dora.ApiClient;
import tech.dora.ApiException;
import tech.dora.Configuration;
import tech.dora.auth.*;
import tech.dora.models.*;
import tech.dora.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://staging.dora.co");
    
    // Configure API key authorization: apiKeyAuthHeader
    ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
    apiKeyAuthHeader.setApiKey("YOUR API KEY");
    // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
    //apiKeyAuthHeader.setApiKeyPrefix("Token");

    // Configure HTTP bearer authorization: bearerAuth
    HttpBearerAuth bearerAuth = (HttpBearerAuth) defaultClient.getAuthentication("bearerAuth");
    bearerAuth.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    UUID userId = UUID.randomUUID(); // UUID | 
    try {
      UserUpdatedResponseEnvelope result = apiInstance.verifyUser(userId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#verifyUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **UUID**|  | |

### Return type

[**UserUpdatedResponseEnvelope**](UserUpdatedResponseEnvelope.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | User verified |  -  |
| **400** | Bad request, e.g. invalid query parameters |  -  |
| **404** | User not found |  -  |
| **500** | Internal server error |  -  |

