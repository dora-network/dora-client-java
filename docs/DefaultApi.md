# DefaultApi

All URIs are relative to *https://localhost:8084*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelAllOpenOrders**](DefaultApi.md#cancelAllOpenOrders) | **DELETE** /v1/orders | Cancel all open orders, if user passes orderbook on query param it will cancel all orders on specific orderbook, admin can cancel user&#x27;s orders on specific orderbook
[**cancelOrderById**](DefaultApi.md#cancelOrderById) | **DELETE** /v1/orders/{order_id} | Cancel an order by ID
[**checkUserEmailExists**](DefaultApi.md#checkUserEmailExists) | **GET** /v1/user/exists | Check whether a user email exists
[**claimLeverageGetAccruedInterest**](DefaultApi.md#claimLeverageGetAccruedInterest) | **POST** /v1/leverage/accrued_interest/claim | Claim current accrued leverage interest for a specific user
[**closeIsolatedPosition**](DefaultApi.md#closeIsolatedPosition) | **POST** /v1/positions/close | Close isolated positions, repaying the borrowed
[**createAPIKeyForUser**](DefaultApi.md#createAPIKeyForUser) | **POST** /v1/user/apikey | Create apikey for a user
[**createAPIKeyForUserID**](DefaultApi.md#createAPIKeyForUserID) | **POST** /v1/user/{user_id}/apikey | Create apikey for a user
[**createOrder**](DefaultApi.md#createOrder) | **POST** /v1/orders | Create a new order
[**createUser**](DefaultApi.md#createUser) | **POST** /v1/integrators/user | Create a new user
[**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /v1/user/{user_id} | Delete user by ID
[**getAPIKeysForUserID**](DefaultApi.md#getAPIKeysForUserID) | **GET** /v1/user/{user_id}/apikey | Get user&#x27;s api keys: admin or integrator only
[**getAllAssetPrices**](DefaultApi.md#getAllAssetPrices) | **GET** /v1/price | Get the current price of all assets
[**getAssetById**](DefaultApi.md#getAssetById) | **GET** /v1/assets/{asset_id} | Get asset by ID
[**getAssetPrice**](DefaultApi.md#getAssetPrice) | **GET** /v1/price/asset/{asset_id} | Get the current price of an asset
[**getAssetYTMById**](DefaultApi.md#getAssetYTMById) | **GET** /v1/assets/{asset_id}/ytm | Get annualized yield to maturity for a bond asset
[**getAssetsStream**](DefaultApi.md#getAssetsStream) | **GET** /v1/assets/stream | Get all inserts or updates for assets
[**getCandleData**](DefaultApi.md#getCandleData) | **GET** /v1/charts/{order_book_id}/candle | Get candlestick data for an orderbook
[**getCouponPaymentsByAssetId**](DefaultApi.md#getCouponPaymentsByAssetId) | **GET** /v1/assets/{asset_id}/coupon_payments | Get coupon payments for a bond asset
[**getL1Depth**](DefaultApi.md#getL1Depth) | **GET** /v1/orderbooks/{order_book_id}/L1 | Get the top price levels for a specific orderbook (L1 market depth)
[**getL2Depth**](DefaultApi.md#getL2Depth) | **GET** /v1/orderbooks/{order_book_id}/L2 | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getL3Depth**](DefaultApi.md#getL3Depth) | **GET** /v1/orderbooks/{order_book_id}/L3 | Get all open orders for a specific orderbook (L3 market depth)
[**getLedgerBalancesSelf**](DefaultApi.md#getLedgerBalancesSelf) | **GET** /v1/ledger/balances/self | Get your own available, locked, and borrowed assets
[**getLedgerInterestSelf**](DefaultApi.md#getLedgerInterestSelf) | **GET** /v1/ledger/interest/self | Get your own interest
[**getLedgerModule**](DefaultApi.md#getLedgerModule) | **GET** /v1/ledger/module | Get the entire module object, including unborrowed leverage assets and total leverage trackers
[**getLedgerModuleByAsset**](DefaultApi.md#getLedgerModuleByAsset) | **GET** /v1/ledger/module/{asset_id} | Get the module object for a single asset ID
[**getLedgerPositionsSelf**](DefaultApi.md#getLedgerPositionsSelf) | **GET** /v1/ledger/positions/self | Get your own positions
[**getLedgerValueSelf**](DefaultApi.md#getLedgerValueSelf) | **GET** /v1/ledger/value/self | Get your own available, locked, and borrowed USD value; and realized and unrealized PnL
[**getLedgerWithdrawRequestsBySelf**](DefaultApi.md#getLedgerWithdrawRequestsBySelf) | **GET** /v1/ledger/withdraw/requests/self | Get all pending withdrawal requests for the logged in user
[**getOrderById**](DefaultApi.md#getOrderById) | **GET** /v1/orders/{order_id} | Get order by ID
[**getOrderbookById**](DefaultApi.md#getOrderbookById) | **GET** /v1/orderbooks/{order_book_id} | Get orderbook by ID
[**getOrderbookDepth**](DefaultApi.md#getOrderbookDepth) | **GET** /v1/orderbooks/{order_book_id}/depth | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getOrderbookOrders**](DefaultApi.md#getOrderbookOrders) | **GET** /v1/orderbooks/{order_book_id}/orders | Get all open orders for a specific orderbook (L3 market depth)
[**getOrderbookStats**](DefaultApi.md#getOrderbookStats) | **GET** /v1/orderbooks/{order_book_id}/stats | Get orderbook stats
[**getOrderbookStatsStream**](DefaultApi.md#getOrderbookStatsStream) | **GET** /v1/orderbooks/{order_book_id}/stats/stream | Orderbook stats stream
[**getOrderbookSummary**](DefaultApi.md#getOrderbookSummary) | **GET** /v1/orderbooks/{order_book_id}/summary | Get summary of an orderbook
[**getOrderbookTop**](DefaultApi.md#getOrderbookTop) | **GET** /v1/orderbooks/{order_book_id}/top | Get the top price levels for a specific orderbook (L1 market depth)
[**getPLForSelfByAccount**](DefaultApi.md#getPLForSelfByAccount) | **GET** /v1/pl/self | Get account-by-account PL breakdown for the logged in user
[**getPoolPrice**](DefaultApi.md#getPoolPrice) | **GET** /v1/price/pool/{pool_id} | Get the current price of a pool
[**getTradeById**](DefaultApi.md#getTradeById) | **GET** /v1/trades/{trade_id} | Get a trade by ID
[**getTrades**](DefaultApi.md#getTrades) | **GET** /v1/trades | Get a filtered, paginated list of trades
[**getTransactionById**](DefaultApi.md#getTransactionById) | **GET** /v1/transactions/{transaction_id} | Get a transaction by ID
[**getTransactions**](DefaultApi.md#getTransactions) | **GET** /v1/transactions | Get a filtered, paginated list of transactions
[**getUserById**](DefaultApi.md#getUserById) | **GET** /v1/user/{user_id} | Get user by ID (admin only)
[**getUserCouponPaymentsStream**](DefaultApi.md#getUserCouponPaymentsStream) | **GET** /v1/user/{user_id}/coupon_payments/stream | Stream user&#x27;s coupon payment accruals in real time
[**getUserLedgerStream**](DefaultApi.md#getUserLedgerStream) | **GET** /v1/user/{user_id}/ledger/stream | Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates
[**getUserOrderUpdatesStream**](DefaultApi.md#getUserOrderUpdatesStream) | **GET** /v1/user/{user_id}/orders/{order_book_id}/updates/stream | Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates
[**getUserOrdersUpdatesStreamAll**](DefaultApi.md#getUserOrdersUpdatesStreamAll) | **GET** /v1/user/{user_id}/orders/all/updates/stream | Get a snapshot of user&#x27;s order updates across all order books since a specific time, and opens a stream for further updates
[**getUserSelf**](DefaultApi.md#getUserSelf) | **GET** /v1/user/self | Get user details for the authenticated user
[**getUserTransactionsStream**](DefaultApi.md#getUserTransactionsStream) | **GET** /v1/user/{user_id}/transactions/stream | Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates
[**getUsersAPIKeys**](DefaultApi.md#getUsersAPIKeys) | **GET** /v1/user/apikey | Get user&#x27;s api keys
[**ledgerDeposit**](DefaultApi.md#ledgerDeposit) | **POST** /v1/ledger/deposit/{user_id} | Deposit assets into this user&#x27;s account from the outside world
[**ledgerWithdraw**](DefaultApi.md#ledgerWithdraw) | **POST** /v1/ledger/withdraw/{user_id} | Withdraw assets from this user to the outside world
[**ledgerWithdrawRequest**](DefaultApi.md#ledgerWithdrawRequest) | **POST** /v1/ledger/withdraw/requests/self | Initiate a withdrawal request for the logged in user to the outside world
[**leverageGetAccruedInterestByUser**](DefaultApi.md#leverageGetAccruedInterestByUser) | **GET** /v1/leverage/accrued_interest/self | Get current accrued leverage interest for the user
[**leverageIsolateCollateral**](DefaultApi.md#leverageIsolateCollateral) | **POST** /v1/leverage/isolate_collateral | Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral
[**leverageSupply**](DefaultApi.md#leverageSupply) | **POST** /v1/leverage/supply | Supply leverage for a specific asset
[**leverageUnite**](DefaultApi.md#leverageUnite) | **POST** /v1/leverage/unite | Combines all isolated positions into a single global position
[**leverageWithdraw**](DefaultApi.md#leverageWithdraw) | **POST** /v1/leverage/withdraw | Withdraw leverage for a specific asset
[**liquidityAdd**](DefaultApi.md#liquidityAdd) | **POST** /v1/liquidity/pool/{pool_id}/add | Add liquidity to a pool
[**liquiditySubtract**](DefaultApi.md#liquiditySubtract) | **POST** /v1/liquidity/pool/{pool_id}/remove | Subtract liquidity from a pool
[**listAssets**](DefaultApi.md#listAssets) | **GET** /v1/assets | List assets
[**listOrderBooks**](DefaultApi.md#listOrderBooks) | **GET** /v1/orderbooks | List order books
[**listOrders**](DefaultApi.md#listOrders) | **GET** /v1/orders | List all orders
[**listPositionAccountsSelf**](DefaultApi.md#listPositionAccountsSelf) | **GET** /v1/user/self/position_accounts | List all position accounts for the authenticated user
[**payLeverageGetAccruedInterest**](DefaultApi.md#payLeverageGetAccruedInterest) | **POST** /v1/leverage/accrued_interest/pay | Pay current accrued leverage interest for a specific user
[**revokeAPIKeyForUser**](DefaultApi.md#revokeAPIKeyForUser) | **PUT** /v1/user/apikey/{key_id}/revoke | Revoke apikey for a user
[**revokeAPIKeyForUserID**](DefaultApi.md#revokeAPIKeyForUserID) | **PUT** /v1/user/{user_id}/apikey/{key_id}/revoke | Revoke apikey for a user: admin or integrator only
[**settleLeverageAccruedInterest**](DefaultApi.md#settleLeverageAccruedInterest) | **POST** /v1/leverage/accrued_interest/settle | Settle current accrued leverage interest for a specific user
[**streamAssetPrices**](DefaultApi.md#streamAssetPrices) | **GET** /v1/prices/stream | Stream real-time asset prices as map objects
[**streamCandleData**](DefaultApi.md#streamCandleData) | **GET** /v1/charts/{order_book_id}/candle/stream | Get a snapshot of candlestick data from date provided, and open a stream for real-time updates
[**streamOrderBookBalances**](DefaultApi.md#streamOrderBookBalances) | **GET** /v1/orderbooks/{order_book_id}/balances/stream | Get a snapshot of base and quote balances for an order book and open a stream for real-time updates
[**streamOrderbookOpenOrders**](DefaultApi.md#streamOrderbookOpenOrders) | **GET** /v1/orderbooks/{order_book_id}/open/stream | Get a snapshot of open orders in an order book and open a stream for real-time updates
[**streamTrades**](DefaultApi.md#streamTrades) | **GET** /v1/trades/{order_book_id}/stream | Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates
[**transferAvailableBalances**](DefaultApi.md#transferAvailableBalances) | **POST** /v1/positions/transfer_balances | Transfer available balance between a user&#x27;s accounts (e.g. global to isolated position)
[**updateUserConfig**](DefaultApi.md#updateUserConfig) | **PUT** /v1/user/{user_id}/config | Update user configuration by ID
[**updateUserConfigSelf**](DefaultApi.md#updateUserConfigSelf) | **PUT** /v1/user/config/self | Update user configuration for the authenticated user
[**validateSubmitOrder**](DefaultApi.md#validateSubmitOrder) | **POST** /v1/orders/validate | Validate submit order request data
[**verifyUser**](DefaultApi.md#verifyUser) | **PUT** /v1/user/{user_id}/verify | Verify a user by ID

<a name="cancelAllOpenOrders"></a>
# **cancelAllOpenOrders**
> ListOrdersResponse cancelAllOpenOrders(orderBookId, userId, orderKind)

Cancel all open orders, if user passes orderbook on query param it will cancel all orders on specific orderbook, admin can cancel user&#x27;s orders on specific orderbook

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
Object userId = null; // Object | 
OrderKind orderKind = new OrderKind(); // OrderKind | 
try {
    ListOrdersResponse result = apiInstance.cancelAllOpenOrders(orderBookId, userId, orderKind);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#cancelAllOpenOrders");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  | [optional]
 **userId** | [**Object**](.md)|  | [optional]
 **orderKind** | [**OrderKind**](.md)|  | [optional]

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="cancelOrderById"></a>
# **cancelOrderById**
> CancelOrderResponse cancelOrderById(orderId)

Cancel an order by ID

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object orderId = null; // Object | 
try {
    CancelOrderResponse result = apiInstance.cancelOrderById(orderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#cancelOrderById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | [**Object**](.md)|  |

### Return type

[**CancelOrderResponse**](CancelOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="checkUserEmailExists"></a>
# **checkUserEmailExists**
> EmailExistsResponse checkUserEmailExists(email)

Check whether a user email exists

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object email = null; // Object | 
try {
    EmailExistsResponse result = apiInstance.checkUserEmailExists(email);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#checkUserEmailExists");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | [**Object**](.md)|  |

### Return type

[**EmailExistsResponse**](EmailExistsResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="claimLeverageGetAccruedInterest"></a>
# **claimLeverageGetAccruedInterest**
> ClaimLeverageAccruedInterestResponse claimLeverageGetAccruedInterest(body)

Claim current accrued leverage interest for a specific user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
ClaimLeverageAccruedInterestRequest body = new ClaimLeverageAccruedInterestRequest(); // ClaimLeverageAccruedInterestRequest | 
try {
    ClaimLeverageAccruedInterestResponse result = apiInstance.claimLeverageGetAccruedInterest(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#claimLeverageGetAccruedInterest");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ClaimLeverageAccruedInterestRequest**](ClaimLeverageAccruedInterestRequest.md)|  |

### Return type

[**ClaimLeverageAccruedInterestResponse**](ClaimLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="closeIsolatedPosition"></a>
# **closeIsolatedPosition**
> ClosePositionResponse closeIsolatedPosition(body)

Close isolated positions, repaying the borrowed

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
ClosePositionRequest body = new ClosePositionRequest(); // ClosePositionRequest | 
try {
    ClosePositionResponse result = apiInstance.closeIsolatedPosition(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#closeIsolatedPosition");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ClosePositionRequest**](ClosePositionRequest.md)|  |

### Return type

[**ClosePositionResponse**](ClosePositionResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createAPIKeyForUser"></a>
# **createAPIKeyForUser**
> CreateAPIKeyResponse createAPIKeyForUser(body)

Create apikey for a user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
CreateAPIKeyRequest body = new CreateAPIKeyRequest(); // CreateAPIKeyRequest | 
try {
    CreateAPIKeyResponse result = apiInstance.createAPIKeyForUser(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#createAPIKeyForUser");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  |

### Return type

[**CreateAPIKeyResponse**](CreateAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createAPIKeyForUserID"></a>
# **createAPIKeyForUserID**
> CreateAPIKeyResponse createAPIKeyForUserID(body, userId)

Create apikey for a user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
CreateAPIKeyRequest body = new CreateAPIKeyRequest(); // CreateAPIKeyRequest | 
Object userId = null; // Object | 
try {
    CreateAPIKeyResponse result = apiInstance.createAPIKeyForUserID(body, userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#createAPIKeyForUserID");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  |
 **userId** | [**Object**](.md)|  |

### Return type

[**CreateAPIKeyResponse**](CreateAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createOrder"></a>
# **createOrder**
> CreateOrderResponse createOrder(body)

Create a new order

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
CreateOrderRequest body = new CreateOrderRequest(); // CreateOrderRequest | 
try {
    CreateOrderResponse result = apiInstance.createOrder(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#createOrder");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateOrderRequest**](CreateOrderRequest.md)|  |

### Return type

[**CreateOrderResponse**](CreateOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createUser"></a>
# **createUser**
> UserCreatedResponse createUser(body)

Create a new user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
CreateIntegratorUserRequest body = new CreateIntegratorUserRequest(); // CreateIntegratorUserRequest | 
try {
    UserCreatedResponse result = apiInstance.createUser(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#createUser");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateIntegratorUserRequest**](CreateIntegratorUserRequest.md)|  |

### Return type

[**UserCreatedResponse**](UserCreatedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteUser"></a>
# **deleteUser**
> UserDeletedResponse deleteUser(userId)

Delete user by ID

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
try {
    UserDeletedResponse result = apiInstance.deleteUser(userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#deleteUser");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |

### Return type

[**UserDeletedResponse**](UserDeletedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAPIKeysForUserID"></a>
# **getAPIKeysForUserID**
> GetAPIKeyResponse getAPIKeysForUserID(userId)

Get user&#x27;s api keys: admin or integrator only

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
try {
    GetAPIKeyResponse result = apiInstance.getAPIKeysForUserID(userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAPIKeysForUserID");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |

### Return type

[**GetAPIKeyResponse**](GetAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAllAssetPrices"></a>
# **getAllAssetPrices**
> ListAssetPriceResponse getAllAssetPrices()

Get the current price of all assets

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    ListAssetPriceResponse result = apiInstance.getAllAssetPrices();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAllAssetPrices");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListAssetPriceResponse**](ListAssetPriceResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetById"></a>
# **getAssetById**
> GetAssetByIDResponse getAssetById(assetId)

Get asset by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object assetId = null; // Object | 
try {
    GetAssetByIDResponse result = apiInstance.getAssetById(assetId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAssetById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | [**Object**](.md)|  |

### Return type

[**GetAssetByIDResponse**](GetAssetByIDResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetPrice"></a>
# **getAssetPrice**
> GetAssetPriceResponse getAssetPrice(assetId)

Get the current price of an asset

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object assetId = null; // Object | 
try {
    GetAssetPriceResponse result = apiInstance.getAssetPrice(assetId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAssetPrice");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | [**Object**](.md)|  |

### Return type

[**GetAssetPriceResponse**](GetAssetPriceResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetYTMById"></a>
# **getAssetYTMById**
> GetAssetYTMByIDResponse getAssetYTMById(assetId)

Get annualized yield to maturity for a bond asset

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object assetId = null; // Object | 
try {
    GetAssetYTMByIDResponse result = apiInstance.getAssetYTMById(assetId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAssetYTMById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | [**Object**](.md)|  |

### Return type

[**GetAssetYTMByIDResponse**](GetAssetYTMByIDResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetsStream"></a>
# **getAssetsStream**
> StreamAssetsResponse getAssetsStream(since, until)

Get all inserts or updates for assets

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object since = null; // Object | 
Object until = null; // Object | 
try {
    StreamAssetsResponse result = apiInstance.getAssetsStream(since, until);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAssetsStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **since** | [**Object**](.md)|  | [optional]
 **until** | [**Object**](.md)|  | [optional]

### Return type

[**StreamAssetsResponse**](StreamAssetsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getCandleData"></a>
# **getCandleData**
> ListCandlesResponse getCandleData(orderBookId, start, end, resolution)

Get candlestick data for an orderbook

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
Object start = null; // Object | 
Object end = null; // Object | 
CandleResolution resolution = new CandleResolution(); // CandleResolution | 
try {
    ListCandlesResponse result = apiInstance.getCandleData(orderBookId, start, end, resolution);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getCandleData");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |
 **start** | [**Object**](.md)|  | [optional]
 **end** | [**Object**](.md)|  | [optional]
 **resolution** | [**CandleResolution**](.md)|  | [optional]

### Return type

[**ListCandlesResponse**](ListCandlesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getCouponPaymentsByAssetId"></a>
# **getCouponPaymentsByAssetId**
> ListCouponPaymentsResponse getCouponPaymentsByAssetId(assetId)

Get coupon payments for a bond asset

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object assetId = null; // Object | 
try {
    ListCouponPaymentsResponse result = apiInstance.getCouponPaymentsByAssetId(assetId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getCouponPaymentsByAssetId");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | [**Object**](.md)|  |

### Return type

[**ListCouponPaymentsResponse**](ListCouponPaymentsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL1Depth"></a>
# **getL1Depth**
> GetTopOfBookResponse getL1Depth(orderBookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    GetTopOfBookResponse result = apiInstance.getL1Depth(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getL1Depth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**GetTopOfBookResponse**](GetTopOfBookResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL2Depth"></a>
# **getL2Depth**
> ListOrderBookDepthResponse getL2Depth(orderBookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    ListOrderBookDepthResponse result = apiInstance.getL2Depth(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getL2Depth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**ListOrderBookDepthResponse**](ListOrderBookDepthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL3Depth"></a>
# **getL3Depth**
> ListOrdersResponse getL3Depth(orderBookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    ListOrdersResponse result = apiInstance.getL3Depth(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getL3Depth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerBalancesSelf"></a>
# **getLedgerBalancesSelf**
> UserBalanceResponse getLedgerBalancesSelf()

Get your own available, locked, and borrowed assets

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    UserBalanceResponse result = apiInstance.getLedgerBalancesSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerBalancesSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserBalanceResponse**](UserBalanceResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerInterestSelf"></a>
# **getLedgerInterestSelf**
> UserInterestResponse getLedgerInterestSelf()

Get your own interest

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    UserInterestResponse result = apiInstance.getLedgerInterestSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerInterestSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserInterestResponse**](UserInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerModule"></a>
# **getLedgerModule**
> LedgerModuleResponse getLedgerModule()

Get the entire module object, including unborrowed leverage assets and total leverage trackers

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    LedgerModuleResponse result = apiInstance.getLedgerModule();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerModule");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**LedgerModuleResponse**](LedgerModuleResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerModuleByAsset"></a>
# **getLedgerModuleByAsset**
> LedgerModuleByAssetResponse getLedgerModuleByAsset(assetId)

Get the module object for a single asset ID

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object assetId = null; // Object | 
try {
    LedgerModuleByAssetResponse result = apiInstance.getLedgerModuleByAsset(assetId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerModuleByAsset");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assetId** | [**Object**](.md)|  |

### Return type

[**LedgerModuleByAssetResponse**](LedgerModuleByAssetResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerPositionsSelf"></a>
# **getLedgerPositionsSelf**
> UserPositionResponse getLedgerPositionsSelf()

Get your own positions

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    UserPositionResponse result = apiInstance.getLedgerPositionsSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerPositionsSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserPositionResponse**](UserPositionResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerValueSelf"></a>
# **getLedgerValueSelf**
> UserValueResponse getLedgerValueSelf()

Get your own available, locked, and borrowed USD value; and realized and unrealized PnL

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    UserValueResponse result = apiInstance.getLedgerValueSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerValueSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserValueResponse**](UserValueResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerWithdrawRequestsBySelf"></a>
# **getLedgerWithdrawRequestsBySelf**
> AllWithdrawalInitiationsResponse getLedgerWithdrawRequestsBySelf()

Get all pending withdrawal requests for the logged in user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    AllWithdrawalInitiationsResponse result = apiInstance.getLedgerWithdrawRequestsBySelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerWithdrawRequestsBySelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AllWithdrawalInitiationsResponse**](AllWithdrawalInitiationsResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderById"></a>
# **getOrderById**
> GetOrderResponse getOrderById(orderId)

Get order by ID

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object orderId = null; // Object | 
try {
    GetOrderResponse result = apiInstance.getOrderById(orderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | [**Object**](.md)|  |

### Return type

[**GetOrderResponse**](GetOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookById"></a>
# **getOrderbookById**
> GetOrderBookResponse getOrderbookById(orderBookId)

Get orderbook by ID

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    GetOrderBookResponse result = apiInstance.getOrderbookById(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**GetOrderBookResponse**](GetOrderBookResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookDepth"></a>
# **getOrderbookDepth**
> ListOrderBookDepthResponse getOrderbookDepth(orderBookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    ListOrderBookDepthResponse result = apiInstance.getOrderbookDepth(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookDepth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**ListOrderBookDepthResponse**](ListOrderBookDepthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookOrders"></a>
# **getOrderbookOrders**
> ListOrdersResponse getOrderbookOrders(orderBookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    ListOrdersResponse result = apiInstance.getOrderbookOrders(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookOrders");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookStats"></a>
# **getOrderbookStats**
> GetOrderbookStatsResponse getOrderbookStats(orderBookId)

Get orderbook stats

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    GetOrderbookStatsResponse result = apiInstance.getOrderbookStats(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookStats");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**GetOrderbookStatsResponse**](GetOrderbookStatsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookStatsStream"></a>
# **getOrderbookStatsStream**
> OrderbookStats getOrderbookStatsStream(orderBookId)

Orderbook stats stream

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    OrderbookStats result = apiInstance.getOrderbookStatsStream(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookStatsStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**OrderbookStats**](OrderbookStats.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookSummary"></a>
# **getOrderbookSummary**
> GetOrderBookSummaryResponse getOrderbookSummary(orderBookId)

Get summary of an orderbook

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    GetOrderBookSummaryResponse result = apiInstance.getOrderbookSummary(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookSummary");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**GetOrderBookSummaryResponse**](GetOrderBookSummaryResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookTop"></a>
# **getOrderbookTop**
> GetTopOfBookResponse getOrderbookTop(orderBookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
try {
    GetTopOfBookResponse result = apiInstance.getOrderbookTop(orderBookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookTop");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |

### Return type

[**GetTopOfBookResponse**](GetTopOfBookResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getPLForSelfByAccount"></a>
# **getPLForSelfByAccount**
> PLResponse getPLForSelfByAccount()

Get account-by-account PL breakdown for the logged in user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    PLResponse result = apiInstance.getPLForSelfByAccount();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getPLForSelfByAccount");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PLResponse**](PLResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getPoolPrice"></a>
# **getPoolPrice**
> GetPoolPriceResponse getPoolPrice(poolId)

Get the current price of a pool

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object poolId = null; // Object | 
try {
    GetPoolPriceResponse result = apiInstance.getPoolPrice(poolId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getPoolPrice");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **poolId** | [**Object**](.md)|  |

### Return type

[**GetPoolPriceResponse**](GetPoolPriceResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTradeById"></a>
# **getTradeById**
> TradeResponse getTradeById(tradeId)

Get a trade by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object tradeId = null; // Object | 
try {
    TradeResponse result = apiInstance.getTradeById(tradeId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getTradeById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tradeId** | [**Object**](.md)|  |

### Return type

[**TradeResponse**](TradeResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTrades"></a>
# **getTrades**
> ListTradeResponse getTrades(orderBookIds, userIds, start, end, page, limit)

Get a filtered, paginated list of trades

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object orderBookIds = null; // Object | 
Object userIds = null; // Object | 
Object start = null; // Object | 
Object end = null; // Object | 
Object page = 1; // Object | 
Object limit = 100; // Object | 
try {
    ListTradeResponse result = apiInstance.getTrades(orderBookIds, userIds, start, end, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getTrades");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookIds** | [**Object**](.md)|  | [optional]
 **userIds** | [**Object**](.md)|  | [optional]
 **start** | [**Object**](.md)|  | [optional]
 **end** | [**Object**](.md)|  | [optional]
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListTradeResponse**](ListTradeResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTransactionById"></a>
# **getTransactionById**
> GetTransactionResponse getTransactionById(transactionId)

Get a transaction by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object transactionId = null; // Object | 
try {
    GetTransactionResponse result = apiInstance.getTransactionById(transactionId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getTransactionById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transactionId** | [**Object**](.md)|  |

### Return type

[**GetTransactionResponse**](GetTransactionResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTransactions"></a>
# **getTransactions**
> ListTransactionsResponse getTransactions(pools, userIds, txKinds, start, end, page, limit)

Get a filtered, paginated list of transactions

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object pools = null; // Object | 
Object userIds = null; // Object | 
Object txKinds = null; // Object | 
Object start = null; // Object | 
Object end = null; // Object | 
Object page = 1; // Object | 
Object limit = 100; // Object | 
try {
    ListTransactionsResponse result = apiInstance.getTransactions(pools, userIds, txKinds, start, end, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getTransactions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pools** | [**Object**](.md)|  | [optional]
 **userIds** | [**Object**](.md)|  | [optional]
 **txKinds** | [**Object**](.md)|  | [optional]
 **start** | [**Object**](.md)|  | [optional]
 **end** | [**Object**](.md)|  | [optional]
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListTransactionsResponse**](ListTransactionsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserById"></a>
# **getUserById**
> GetUserResponse getUserById(userId)

Get user by ID (admin only)

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
try {
    GetUserResponse result = apiInstance.getUserById(userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |

### Return type

[**GetUserResponse**](GetUserResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserCouponPaymentsStream"></a>
# **getUserCouponPaymentsStream**
> StreamUserCouponPaymentsResponse getUserCouponPaymentsStream(userId)

Stream user&#x27;s coupon payment accruals in real time

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthQuery
ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
apiKeyAuthQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.setApiKeyPrefix("Token");

DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
try {
    StreamUserCouponPaymentsResponse result = apiInstance.getUserCouponPaymentsStream(userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserCouponPaymentsStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |

### Return type

[**StreamUserCouponPaymentsResponse**](StreamUserCouponPaymentsResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserLedgerStream"></a>
# **getUserLedgerStream**
> StreamPositionsResponse getUserLedgerStream(userId)

Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthQuery
ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
apiKeyAuthQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.setApiKeyPrefix("Token");

DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
try {
    StreamPositionsResponse result = apiInstance.getUserLedgerStream(userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserLedgerStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |

### Return type

[**StreamPositionsResponse**](StreamPositionsResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserOrderUpdatesStream"></a>
# **getUserOrderUpdatesStream**
> StreamOrderUpdatesResponse getUserOrderUpdatesStream(userId, orderBookId, since)

Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthQuery
ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
apiKeyAuthQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.setApiKeyPrefix("Token");

DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
Object orderBookId = null; // Object | 
Object since = null; // Object | 
try {
    StreamOrderUpdatesResponse result = apiInstance.getUserOrderUpdatesStream(userId, orderBookId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserOrderUpdatesStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |
 **orderBookId** | [**Object**](.md)|  |
 **since** | [**Object**](.md)|  | [optional]

### Return type

[**StreamOrderUpdatesResponse**](StreamOrderUpdatesResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserOrdersUpdatesStreamAll"></a>
# **getUserOrdersUpdatesStreamAll**
> StreamOrderUpdatesResponse getUserOrdersUpdatesStreamAll(userId, since)

Get a snapshot of user&#x27;s order updates across all order books since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthQuery
ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
apiKeyAuthQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.setApiKeyPrefix("Token");

DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
Object since = null; // Object | 
try {
    StreamOrderUpdatesResponse result = apiInstance.getUserOrdersUpdatesStreamAll(userId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserOrdersUpdatesStreamAll");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |
 **since** | [**Object**](.md)|  | [optional]

### Return type

[**StreamOrderUpdatesResponse**](StreamOrderUpdatesResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserSelf"></a>
# **getUserSelf**
> GetUserResponse getUserSelf()

Get user details for the authenticated user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    GetUserResponse result = apiInstance.getUserSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GetUserResponse**](GetUserResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserTransactionsStream"></a>
# **getUserTransactionsStream**
> StreamTransactionsResponse getUserTransactionsStream(userId, since)

Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthQuery
ApiKeyAuth apiKeyAuthQuery = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthQuery");
apiKeyAuthQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthQuery.setApiKeyPrefix("Token");

DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
Object since = null; // Object | 
try {
    StreamTransactionsResponse result = apiInstance.getUserTransactionsStream(userId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserTransactionsStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |
 **since** | [**Object**](.md)|  | [optional]

### Return type

[**StreamTransactionsResponse**](StreamTransactionsResponse.md)

### Authorization

[apiKeyAuthQuery](../README.md#apiKeyAuthQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUsersAPIKeys"></a>
# **getUsersAPIKeys**
> GetAPIKeyResponse getUsersAPIKeys()

Get user&#x27;s api keys

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    GetAPIKeyResponse result = apiInstance.getUsersAPIKeys();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUsersAPIKeys");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GetAPIKeyResponse**](GetAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="ledgerDeposit"></a>
# **ledgerDeposit**
> FundUserResponse ledgerDeposit(body, userId)

Deposit assets into this user&#x27;s account from the outside world

Deposit assets into this user&#x27;s account from the outside world. Note that this does not interact with any external systems; it simply adds the amount to the user&#x27;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
FundUserRequest body = new FundUserRequest(); // FundUserRequest | 
Object userId = null; // Object | 
try {
    FundUserResponse result = apiInstance.ledgerDeposit(body, userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#ledgerDeposit");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**FundUserRequest**](FundUserRequest.md)|  |
 **userId** | [**Object**](.md)|  |

### Return type

[**FundUserResponse**](FundUserResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="ledgerWithdraw"></a>
# **ledgerWithdraw**
> FundUserResponse ledgerWithdraw(body, userId)

Withdraw assets from this user to the outside world

Withdraw assets from this user&#x27;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#x27;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
DefundUserRequest body = new DefundUserRequest(); // DefundUserRequest | 
Object userId = null; // Object | 
try {
    FundUserResponse result = apiInstance.ledgerWithdraw(body, userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#ledgerWithdraw");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DefundUserRequest**](DefundUserRequest.md)|  |
 **userId** | [**Object**](.md)|  |

### Return type

[**FundUserResponse**](FundUserResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="ledgerWithdrawRequest"></a>
# **ledgerWithdrawRequest**
> WithdrawalInitiationResponse ledgerWithdrawRequest(body, userId)

Initiate a withdrawal request for the logged in user to the outside world

Withdraw assets from the logged in user&#x27;s account to the outside world. Note that this does not interact with any external systems; it simply deducts the amount from the user&#x27;s available balance in the ledger. Actual transfer of assets must be handled separately.

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
DefundUserRequest body = new DefundUserRequest(); // DefundUserRequest | 
Object userId = null; // Object | 
try {
    WithdrawalInitiationResponse result = apiInstance.ledgerWithdrawRequest(body, userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#ledgerWithdrawRequest");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DefundUserRequest**](DefundUserRequest.md)|  |
 **userId** | [**Object**](.md)|  |

### Return type

[**WithdrawalInitiationResponse**](WithdrawalInitiationResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageGetAccruedInterestByUser"></a>
# **leverageGetAccruedInterestByUser**
> CurrentLeverageAccruedInterestResponse leverageGetAccruedInterestByUser(positionId, assetId)

Get current accrued leverage interest for the user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object positionId = null; // Object | 
Object assetId = null; // Object | 
try {
    CurrentLeverageAccruedInterestResponse result = apiInstance.leverageGetAccruedInterestByUser(positionId, assetId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageGetAccruedInterestByUser");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **positionId** | [**Object**](.md)|  | [optional]
 **assetId** | [**Object**](.md)|  | [optional]

### Return type

[**CurrentLeverageAccruedInterestResponse**](CurrentLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="leverageIsolateCollateral"></a>
# **leverageIsolateCollateral**
> IsolateCollateralResponse leverageIsolateCollateral(body)

Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
IsolateCollateralRequest body = new IsolateCollateralRequest(); // IsolateCollateralRequest | 
try {
    IsolateCollateralResponse result = apiInstance.leverageIsolateCollateral(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageIsolateCollateral");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**IsolateCollateralRequest**](IsolateCollateralRequest.md)|  |

### Return type

[**IsolateCollateralResponse**](IsolateCollateralResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageSupply"></a>
# **leverageSupply**
> SupplyResponse leverageSupply(body)

Supply leverage for a specific asset

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
SupplyRequest body = new SupplyRequest(); // SupplyRequest | 
try {
    SupplyResponse result = apiInstance.leverageSupply(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageSupply");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SupplyRequest**](SupplyRequest.md)|  |

### Return type

[**SupplyResponse**](SupplyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageUnite"></a>
# **leverageUnite**
> UnitePositionResponse leverageUnite(body)

Combines all isolated positions into a single global position

Combines all isolated positions into a single global position

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
UnitePositionRequest body = new UnitePositionRequest(); // UnitePositionRequest | 
try {
    UnitePositionResponse result = apiInstance.leverageUnite(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageUnite");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UnitePositionRequest**](UnitePositionRequest.md)|  |

### Return type

[**UnitePositionResponse**](UnitePositionResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageWithdraw"></a>
# **leverageWithdraw**
> WithdrawResponse leverageWithdraw(body)

Withdraw leverage for a specific asset

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
WithdrawRequest body = new WithdrawRequest(); // WithdrawRequest | 
try {
    WithdrawResponse result = apiInstance.leverageWithdraw(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageWithdraw");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**WithdrawRequest**](WithdrawRequest.md)|  |

### Return type

[**WithdrawResponse**](WithdrawResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquidityAdd"></a>
# **liquidityAdd**
> LiquidityResponse liquidityAdd(body, poolId)

Add liquidity to a pool

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
LiquidityRequest body = new LiquidityRequest(); // LiquidityRequest | 
Object poolId = null; // Object | 
try {
    LiquidityResponse result = apiInstance.liquidityAdd(body, poolId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#liquidityAdd");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**LiquidityRequest**](LiquidityRequest.md)|  |
 **poolId** | [**Object**](.md)|  |

### Return type

[**LiquidityResponse**](LiquidityResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquiditySubtract"></a>
# **liquiditySubtract**
> LiquidityResponse liquiditySubtract(body, poolId)

Subtract liquidity from a pool

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
LiquidityRequest body = new LiquidityRequest(); // LiquidityRequest | 
Object poolId = null; // Object | 
try {
    LiquidityResponse result = apiInstance.liquiditySubtract(body, poolId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#liquiditySubtract");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**LiquidityRequest**](LiquidityRequest.md)|  |
 **poolId** | [**Object**](.md)|  |

### Return type

[**LiquidityResponse**](LiquidityResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="listAssets"></a>
# **listAssets**
> ListAssetsResponse listAssets(createdAfter, createdBefore, assetKind, canAddLiquidity, canDirectBorrow, canOnboard, canTrade, canVirtualBorrow, page, limit)

List assets

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object createdAfter = null; // Object | 
Object createdBefore = null; // Object | 
AssetKind assetKind = new AssetKind(); // AssetKind | Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE)
Object canAddLiquidity = null; // Object | 
Object canDirectBorrow = null; // Object | 
Object canOnboard = null; // Object | 
Object canTrade = null; // Object | 
Object canVirtualBorrow = null; // Object | 
Object page = 1; // Object | 
Object limit = 100; // Object | 
try {
    ListAssetsResponse result = apiInstance.listAssets(createdAfter, createdBefore, assetKind, canAddLiquidity, canDirectBorrow, canOnboard, canTrade, canVirtualBorrow, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#listAssets");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createdAfter** | [**Object**](.md)|  | [optional]
 **createdBefore** | [**Object**](.md)|  | [optional]
 **assetKind** | [**AssetKind**](.md)| Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE) | [optional]
 **canAddLiquidity** | [**Object**](.md)|  | [optional]
 **canDirectBorrow** | [**Object**](.md)|  | [optional]
 **canOnboard** | [**Object**](.md)|  | [optional]
 **canTrade** | [**Object**](.md)|  | [optional]
 **canVirtualBorrow** | [**Object**](.md)|  | [optional]
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListAssetsResponse**](ListAssetsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrderBooks"></a>
# **listOrderBooks**
> ListOrderBooksResponse listOrderBooks(status, baseAssetId, quoteAssetId, page, limit)

List order books

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
OrderBookStatus status = new OrderBookStatus(); // OrderBookStatus | 
Object baseAssetId = null; // Object | 
Object quoteAssetId = null; // Object | 
Object page = 1; // Object | 
Object limit = 100; // Object | 
try {
    ListOrderBooksResponse result = apiInstance.listOrderBooks(status, baseAssetId, quoteAssetId, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#listOrderBooks");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | [**OrderBookStatus**](.md)|  | [optional]
 **baseAssetId** | [**Object**](.md)|  | [optional]
 **quoteAssetId** | [**Object**](.md)|  | [optional]
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListOrderBooksResponse**](ListOrderBooksResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrders"></a>
# **listOrders**
> ListOrdersResponse listOrders(orderBookId, kind, status, side, from, to, page, limit)

List all orders

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
Object kind = null; // Object | 
Object status = null; // Object | 
Side side = new Side(); // Side | 
Object from = null; // Object | 
Object to = null; // Object | 
Object page = 1; // Object | 
Object limit = 100; // Object | 
try {
    ListOrdersResponse result = apiInstance.listOrders(orderBookId, kind, status, side, from, to, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#listOrders");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  | [optional]
 **kind** | [**Object**](.md)|  | [optional]
 **status** | [**Object**](.md)|  | [optional]
 **side** | [**Side**](.md)|  | [optional]
 **from** | [**Object**](.md)|  | [optional]
 **to** | [**Object**](.md)|  | [optional]
 **page** | [**Object**](.md)|  | [optional] [default to 1]
 **limit** | [**Object**](.md)|  | [optional] [default to 100]

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listPositionAccountsSelf"></a>
# **listPositionAccountsSelf**
> ListPositionAccountsResponse listPositionAccountsSelf()

List all position accounts for the authenticated user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
try {
    ListPositionAccountsResponse result = apiInstance.listPositionAccountsSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#listPositionAccountsSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListPositionAccountsResponse**](ListPositionAccountsResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="payLeverageGetAccruedInterest"></a>
# **payLeverageGetAccruedInterest**
> PayLeverageAccruedInterestResponse payLeverageGetAccruedInterest(body)

Pay current accrued leverage interest for a specific user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
PayLeverageAccruedInterestRequest body = new PayLeverageAccruedInterestRequest(); // PayLeverageAccruedInterestRequest | 
try {
    PayLeverageAccruedInterestResponse result = apiInstance.payLeverageGetAccruedInterest(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#payLeverageGetAccruedInterest");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PayLeverageAccruedInterestRequest**](PayLeverageAccruedInterestRequest.md)|  |

### Return type

[**PayLeverageAccruedInterestResponse**](PayLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="revokeAPIKeyForUser"></a>
# **revokeAPIKeyForUser**
> RevokeAPIKeyResponse revokeAPIKeyForUser(keyId)

Revoke apikey for a user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object keyId = null; // Object | 
try {
    RevokeAPIKeyResponse result = apiInstance.revokeAPIKeyForUser(keyId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#revokeAPIKeyForUser");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **keyId** | [**Object**](.md)|  |

### Return type

[**RevokeAPIKeyResponse**](RevokeAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="revokeAPIKeyForUserID"></a>
# **revokeAPIKeyForUserID**
> RevokeAPIKeyResponse revokeAPIKeyForUserID(userId, keyId)

Revoke apikey for a user: admin or integrator only

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
Object keyId = null; // Object | 
try {
    RevokeAPIKeyResponse result = apiInstance.revokeAPIKeyForUserID(userId, keyId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#revokeAPIKeyForUserID");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |
 **keyId** | [**Object**](.md)|  |

### Return type

[**RevokeAPIKeyResponse**](RevokeAPIKeyResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="settleLeverageAccruedInterest"></a>
# **settleLeverageAccruedInterest**
> SettleLeverageAccruedInterestResponse settleLeverageAccruedInterest(body)

Settle current accrued leverage interest for a specific user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
SettleLeverageAccruedInterestRequest body = new SettleLeverageAccruedInterestRequest(); // SettleLeverageAccruedInterestRequest | 
try {
    SettleLeverageAccruedInterestResponse result = apiInstance.settleLeverageAccruedInterest(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#settleLeverageAccruedInterest");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**SettleLeverageAccruedInterestRequest**](SettleLeverageAccruedInterestRequest.md)|  |

### Return type

[**SettleLeverageAccruedInterestResponse**](SettleLeverageAccruedInterestResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="streamAssetPrices"></a>
# **streamAssetPrices**
> StreamAssetPricesResponse streamAssetPrices(since, assetId)

Stream real-time asset prices as map objects

Opens a WebSocket stream for real-time asset price updates. First message contains all current prices, subsequent messages contain only changed prices. Data is sent as JSON objects keyed by asset ID.

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object since = null; // Object | 
Object assetId = null; // Object | 
try {
    StreamAssetPricesResponse result = apiInstance.streamAssetPrices(since, assetId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamAssetPrices");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **since** | [**Object**](.md)|  | [optional]
 **assetId** | [**Object**](.md)|  | [optional]

### Return type

[**StreamAssetPricesResponse**](StreamAssetPricesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamCandleData"></a>
# **streamCandleData**
> StreamCandlesResponse streamCandleData(orderBookId, since, resolution)

Get a snapshot of candlestick data from date provided, and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
Object since = null; // Object | 
CandleResolution resolution = new CandleResolution(); // CandleResolution | 
try {
    StreamCandlesResponse result = apiInstance.streamCandleData(orderBookId, since, resolution);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamCandleData");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |
 **since** | [**Object**](.md)|  | [optional]
 **resolution** | [**CandleResolution**](.md)|  | [optional]

### Return type

[**StreamCandlesResponse**](StreamCandlesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamOrderBookBalances"></a>
# **streamOrderBookBalances**
> StreamOrderBookBalancesResponse streamOrderBookBalances(orderBookId, since)

Get a snapshot of base and quote balances for an order book and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
Object since = null; // Object | 
try {
    StreamOrderBookBalancesResponse result = apiInstance.streamOrderBookBalances(orderBookId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamOrderBookBalances");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |
 **since** | [**Object**](.md)|  | [optional]

### Return type

[**StreamOrderBookBalancesResponse**](StreamOrderBookBalancesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamOrderbookOpenOrders"></a>
# **streamOrderbookOpenOrders**
> LiveOrderbook streamOrderbookOpenOrders(orderBookId, since)

Get a snapshot of open orders in an order book and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
Object since = null; // Object | 
try {
    LiveOrderbook result = apiInstance.streamOrderbookOpenOrders(orderBookId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamOrderbookOpenOrders");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |
 **since** | [**Object**](.md)|  | [optional]

### Return type

[**LiveOrderbook**](LiveOrderbook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamTrades"></a>
# **streamTrades**
> StreamTradesResponse streamTrades(orderBookId, since)

Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object orderBookId = null; // Object | 
Object since = null; // Object | 
try {
    StreamTradesResponse result = apiInstance.streamTrades(orderBookId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamTrades");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderBookId** | [**Object**](.md)|  |
 **since** | [**Object**](.md)|  | [optional]

### Return type

[**StreamTradesResponse**](StreamTradesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="transferAvailableBalances"></a>
# **transferAvailableBalances**
> TransferBalancesResponse transferAvailableBalances(body)

Transfer available balance between a user&#x27;s accounts (e.g. global to isolated position)

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
TransferBalancesRequest body = new TransferBalancesRequest(); // TransferBalancesRequest | 
try {
    TransferBalancesResponse result = apiInstance.transferAvailableBalances(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#transferAvailableBalances");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**TransferBalancesRequest**](TransferBalancesRequest.md)|  |

### Return type

[**TransferBalancesResponse**](TransferBalancesResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateUserConfig"></a>
# **updateUserConfig**
> UserUpdatedResponse updateUserConfig(body, userId)

Update user configuration by ID

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
UpdateUserConfigRequest body = new UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
Object userId = null; // Object | 
try {
    UserUpdatedResponse result = apiInstance.updateUserConfig(body, userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#updateUserConfig");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateUserConfigRequest**](UpdateUserConfigRequest.md)|  |
 **userId** | [**Object**](.md)|  |

### Return type

[**UserUpdatedResponse**](UserUpdatedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateUserConfigSelf"></a>
# **updateUserConfigSelf**
> UserUpdatedResponse updateUserConfigSelf(body)

Update user configuration for the authenticated user

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
UpdateUserConfigRequest body = new UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
try {
    UserUpdatedResponse result = apiInstance.updateUserConfigSelf(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#updateUserConfigSelf");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateUserConfigRequest**](UpdateUserConfigRequest.md)|  |

### Return type

[**UserUpdatedResponse**](UserUpdatedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="validateSubmitOrder"></a>
# **validateSubmitOrder**
> ValidateSubmitOrderResponse validateSubmitOrder(body)

Validate submit order request data

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
ValidateSubmitOrderRequest body = new ValidateSubmitOrderRequest(); // ValidateSubmitOrderRequest | 
try {
    ValidateSubmitOrderResponse result = apiInstance.validateSubmitOrder(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#validateSubmitOrder");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ValidateSubmitOrderRequest**](ValidateSubmitOrderRequest.md)|  |

### Return type

[**ValidateSubmitOrderResponse**](ValidateSubmitOrderResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="verifyUser"></a>
# **verifyUser**
> UserUpdatedResponse verifyUser(userId)

Verify a user by ID

### Example
```java
// Import classes:
//import tech.dora.ApiClient;
//import tech.dora.ApiException;
//import tech.dora.Configuration;
//import tech.dora.auth.*;
//import tech.dora.api.DefaultApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: apiKeyAuthHeader
ApiKeyAuth apiKeyAuthHeader = (ApiKeyAuth) defaultClient.getAuthentication("apiKeyAuthHeader");
apiKeyAuthHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//apiKeyAuthHeader.setApiKeyPrefix("Token");


DefaultApi apiInstance = new DefaultApi();
Object userId = null; // Object | 
try {
    UserUpdatedResponse result = apiInstance.verifyUser(userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#verifyUser");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**Object**](.md)|  |

### Return type

[**UserUpdatedResponse**](UserUpdatedResponse.md)

### Authorization

[apiKeyAuthHeader](../README.md#apiKeyAuthHeader)[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

