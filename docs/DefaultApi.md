# DefaultApi

All URIs are relative to *https://localhost:8084*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelAllOpenOrders**](DefaultApi.md#cancelAllOpenOrders) | **DELETE** /v1/orders | Cancel all open orders
[**cancelOrderById**](DefaultApi.md#cancelOrderById) | **DELETE** /v1/orders/{order_id} | Cancel an order by ID
[**createOrder**](DefaultApi.md#createOrder) | **POST** /v1/orders | Create a new order
[**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /v1/user/{user_id} | Delete user by ID
[**getAllAssetPrices**](DefaultApi.md#getAllAssetPrices) | **GET** /v1/price | Get the current price of all assets
[**getAssetById**](DefaultApi.md#getAssetById) | **GET** /v1/assets/{asset_id} | Get asset by ID
[**getAssetPrice**](DefaultApi.md#getAssetPrice) | **GET** /v1/price/asset/{asset_id} | Get the current price of an asset
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
[**getOrderById**](DefaultApi.md#getOrderById) | **GET** /v1/orders/{order_id} | Get order by ID
[**getOrderbookById**](DefaultApi.md#getOrderbookById) | **GET** /v1/orderbooks/{order_book_id} | Get orderbook by ID
[**getOrderbookDepth**](DefaultApi.md#getOrderbookDepth) | **GET** /v1/orderbooks/{order_book_id}/depth | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getOrderbookOrders**](DefaultApi.md#getOrderbookOrders) | **GET** /v1/orderbooks/{order_book_id}/orders | Get all open orders for a specific orderbook (L3 market depth)
[**getOrderbookSummary**](DefaultApi.md#getOrderbookSummary) | **GET** /v1/orderbooks/{order_book_id}/summary | Get summary of an orderbook
[**getOrderbookTop**](DefaultApi.md#getOrderbookTop) | **GET** /v1/orderbooks/{order_book_id}/top | Get the top price levels for a specific orderbook (L1 market depth)
[**getPoolPrice**](DefaultApi.md#getPoolPrice) | **GET** /v1/price/pool/{pool_id} | Get the current price of a pool
[**getTradeById**](DefaultApi.md#getTradeById) | **GET** /v1/trades/{trade_id} | Get a trade by ID
[**getTrades**](DefaultApi.md#getTrades) | **GET** /v1/trades | Get a filtered, paginated list of trades
[**getTransactionById**](DefaultApi.md#getTransactionById) | **GET** /v1/transactions/{transaction_id} | Get a transaction by ID
[**getTransactions**](DefaultApi.md#getTransactions) | **GET** /v1/transactions | Get a filtered, paginated list of transactions
[**getUserById**](DefaultApi.md#getUserById) | **GET** /v1/user/{user_id} | Get user by ID (admin only)
[**getUserLedgerStream**](DefaultApi.md#getUserLedgerStream) | **GET** /v1/user/{user_id}/ledger/stream | Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates
[**getUserOrderUpdatesStream**](DefaultApi.md#getUserOrderUpdatesStream) | **GET** /v1/user/{user_id}/orders/{order_book_id}/updates/stream | Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates
[**getUserOrdersUpdatesStreamAll**](DefaultApi.md#getUserOrdersUpdatesStreamAll) | **GET** /v1/user/{user_id}/orders/all/updates/stream | Get a snapshot of user&#x27;s order updates across all order books since a specific time, and opens a stream for further updates
[**getUserSelf**](DefaultApi.md#getUserSelf) | **GET** /v1/user/self | Get user details for the authenticated user
[**getUserTransactionsStream**](DefaultApi.md#getUserTransactionsStream) | **GET** /v1/user/{user_id}/transactions/stream | Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates
[**ledgerDeposit**](DefaultApi.md#ledgerDeposit) | **POST** /v1/ledger/deposit | Deposit assets into your account from the outside world
[**ledgerWithdraw**](DefaultApi.md#ledgerWithdraw) | **POST** /v1/ledger/withdraw | Withdraw assets from your account to the outside world
[**leverageCollateralize**](DefaultApi.md#leverageCollateralize) | **POST** /v1/leverage/collateralize | Move supplied and available to supplied_collateral and collateral, for a specified position
[**leverageDeCollateralize**](DefaultApi.md#leverageDeCollateralize) | **POST** /v1/leverage/de-collateralize | Move collateral and supplied_collateral to available and supplied, for a specified position.
[**leverageIsolateCollateral**](DefaultApi.md#leverageIsolateCollateral) | **POST** /v1/leverage/isolate_collateral | Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral
[**leverageIsolatePosition**](DefaultApi.md#leverageIsolatePosition) | **POST** /v1/leverage/isolate_position | Create an isolated position using all collateral, supplied_collateral, and borrows from the user&#x27;s global position
[**leverageSupply**](DefaultApi.md#leverageSupply) | **POST** /v1/leverage/supply | Supply leverage for a specific asset
[**leverageUnite**](DefaultApi.md#leverageUnite) | **POST** /v1/leverage/unite | Combines all isolated positions into a single global position
[**leverageWithdraw**](DefaultApi.md#leverageWithdraw) | **POST** /v1/leverage/withdraw | Withdraw leverage for a specific asset
[**liquidityAdd**](DefaultApi.md#liquidityAdd) | **POST** /v1/liquidity/pool/{pool_id}/add | Add liquidity to a pool
[**liquiditySubtract**](DefaultApi.md#liquiditySubtract) | **POST** /v1/liquidity/pool/{pool_id}/remove | Subtract liquidity from a pool
[**listAssets**](DefaultApi.md#listAssets) | **GET** /v1/assets | List assets
[**listOrderBooks**](DefaultApi.md#listOrderBooks) | **GET** /v1/orderbooks | List order books
[**listOrders**](DefaultApi.md#listOrders) | **GET** /v1/orders | List all orders
[**streamAssetPrices**](DefaultApi.md#streamAssetPrices) | **GET** /v1/prices/stream | Stream real-time asset prices as map objects
[**streamCandleData**](DefaultApi.md#streamCandleData) | **GET** /v1/charts/{order_book_id}/candle/stream | Get a snapshot of candlestick data from date provided, and open a stream for real-time updates
[**streamOrderBookBalances**](DefaultApi.md#streamOrderBookBalances) | **GET** /v1/orderbooks/{order_book_id}/balances/stream | Get a snapshot of base and quote balances for an order book and open a stream for real-time updates
[**streamOrderbookOpenOrders**](DefaultApi.md#streamOrderbookOpenOrders) | **GET** /v1/orderbooks/{order_book_id}/open/stream | Get a snapshot of open orders in an order book and open a stream for real-time updates
[**streamTrades**](DefaultApi.md#streamTrades) | **GET** /v1/trades/{order_book_id}/stream | Get a snapshot of trades executed on the given order book from a specific date and open a stream for real-time updates
[**updateUserConfig**](DefaultApi.md#updateUserConfig) | **PUT** /v1/user/{user_id}/config | Update user configuration by ID
[**updateUserConfigSelf**](DefaultApi.md#updateUserConfigSelf) | **PUT** /v1/user/config/self | Update user configuration for the authenticated user
[**verifyUser**](DefaultApi.md#verifyUser) | **PUT** /v1/user/{user_id}/verify | Verify a user by ID

<a name="cancelAllOpenOrders"></a>
# **cancelAllOpenOrders**
> ListOrdersResponse cancelAllOpenOrders()

Cancel all open orders

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    ListOrdersResponse result = apiInstance.cancelAllOpenOrders();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#cancelAllOpenOrders");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderId = new UUID(); // UUID | 
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
 **orderId** | [**UUID**](.md)|  |

### Return type

[**CancelOrderResponse**](CancelOrderResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="createOrder"></a>
# **createOrder**
> CreateOrderResponse createOrder(body)

Create a new order

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
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
 **userId** | [**UUID**](.md)|  |

### Return type

[**UserDeletedResponse**](UserDeletedResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
UUID assetId = new UUID(); // UUID | 
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
 **assetId** | [**UUID**](.md)|  |

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID assetId = new UUID(); // UUID | 
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
 **assetId** | [**UUID**](.md)|  |

### Return type

[**GetAssetPriceResponse**](GetAssetPriceResponse.md)

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
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime until = new OffsetDateTime(); // OffsetDateTime | 
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
 **since** | **OffsetDateTime**|  | [optional]
 **until** | **OffsetDateTime**|  | [optional]

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
String orderBookId = "orderBookId_example"; // String | 
OffsetDateTime start = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime end = new OffsetDateTime(); // OffsetDateTime | 
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
 **orderBookId** | **String**|  |
 **start** | **OffsetDateTime**|  | [optional]
 **end** | **OffsetDateTime**|  | [optional]
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
UUID assetId = new UUID(); // UUID | 
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
 **assetId** | [**UUID**](.md)|  |

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
UUID orderBookId = new UUID(); // UUID | 
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
 **orderBookId** | [**UUID**](.md)|  |

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
UUID orderBookId = new UUID(); // UUID | 
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
 **orderBookId** | [**UUID**](.md)|  |

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
UUID orderBookId = new UUID(); // UUID | 
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
 **orderBookId** | [**UUID**](.md)|  |

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID assetId = new UUID(); // UUID | 
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
 **assetId** | [**UUID**](.md)|  |

### Return type

[**LedgerModuleByAssetResponse**](LedgerModuleByAssetResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderId = new UUID(); // UUID | 
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
 **orderId** | [**UUID**](.md)|  |

### Return type

[**GetOrderResponse**](GetOrderResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderBookId = new UUID(); // UUID | 
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
 **orderBookId** | [**UUID**](.md)|  |

### Return type

[**GetOrderBookResponse**](GetOrderBookResponse.md)

### Authorization

No authorization required

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
UUID orderBookId = new UUID(); // UUID | 
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
 **orderBookId** | [**UUID**](.md)|  |

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
UUID orderBookId = new UUID(); // UUID | 
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
 **orderBookId** | [**UUID**](.md)|  |

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderBookId = new UUID(); // UUID | 
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
 **orderBookId** | [**UUID**](.md)|  |

### Return type

[**GetOrderBookSummaryResponse**](GetOrderBookSummaryResponse.md)

### Authorization

No authorization required

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
UUID orderBookId = new UUID(); // UUID | 
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
 **orderBookId** | [**UUID**](.md)|  |

### Return type

[**GetTopOfBookResponse**](GetTopOfBookResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID poolId = new UUID(); // UUID | 
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
 **poolId** | [**UUID**](.md)|  |

### Return type

[**GetPoolPriceResponse**](GetPoolPriceResponse.md)

### Authorization

No authorization required

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
UUID tradeId = new UUID(); // UUID | 
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
 **tradeId** | [**UUID**](.md)|  |

### Return type

[**TradeResponse**](TradeResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTrades"></a>
# **getTrades**
> ListTradeResponse getTrades(pools, userIds, start, end, page, limit)

Get a filtered, paginated list of trades

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
List<String> pools = Arrays.asList("pools_example"); // List<String> | 
List<UUID> userIds = Arrays.asList(new UUID()); // List<UUID> | 
OffsetDateTime start = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime end = new OffsetDateTime(); // OffsetDateTime | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
try {
    ListTradeResponse result = apiInstance.getTrades(pools, userIds, start, end, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getTrades");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pools** | [**List&lt;String&gt;**](String.md)|  | [optional]
 **userIds** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional]
 **start** | **OffsetDateTime**|  | [optional]
 **end** | **OffsetDateTime**|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**ListTradeResponse**](ListTradeResponse.md)

### Authorization

No authorization required

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
UUID transactionId = new UUID(); // UUID | 
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
 **transactionId** | [**UUID**](.md)|  |

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
List<String> pools = Arrays.asList("pools_example"); // List<String> | 
List<UUID> userIds = Arrays.asList(new UUID()); // List<UUID> | 
List<TransactionKind> txKinds = Arrays.asList(new TransactionKind()); // List<TransactionKind> | 
OffsetDateTime start = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime end = new OffsetDateTime(); // OffsetDateTime | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
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
 **pools** | [**List&lt;String&gt;**](String.md)|  | [optional]
 **userIds** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional]
 **txKinds** | [**List&lt;TransactionKind&gt;**](TransactionKind.md)|  | [optional]
 **start** | **OffsetDateTime**|  | [optional]
 **end** | **OffsetDateTime**|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
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
 **userId** | [**UUID**](.md)|  |

### Return type

[**GetUserResponse**](GetUserResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
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
 **userId** | [**UUID**](.md)|  |

### Return type

[**StreamPositionsResponse**](StreamPositionsResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
UUID orderBookId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
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
 **userId** | [**UUID**](.md)|  |
 **orderBookId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**StreamOrderUpdatesResponse**](StreamOrderUpdatesResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
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
 **userId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**StreamOrderUpdatesResponse**](StreamOrderUpdatesResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
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
 **userId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**StreamTransactionsResponse**](StreamTransactionsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="ledgerDeposit"></a>
# **ledgerDeposit**
> FundUserResponse ledgerDeposit(body)

Deposit assets into your account from the outside world

TODO: finish this when implementation has been completed

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
FundUserRequest body = new FundUserRequest(); // FundUserRequest | 
try {
    FundUserResponse result = apiInstance.ledgerDeposit(body);
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

### Return type

[**FundUserResponse**](FundUserResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="ledgerWithdraw"></a>
# **ledgerWithdraw**
> FundUserResponse ledgerWithdraw(body)

Withdraw assets from your account to the outside world

TODO: Finish this when implementation has been completed

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
FundUserRequest body = new FundUserRequest(); // FundUserRequest | 
try {
    FundUserResponse result = apiInstance.ledgerWithdraw(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#ledgerWithdraw");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**FundUserRequest**](FundUserRequest.md)|  |

### Return type

[**FundUserResponse**](FundUserResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageCollateralize"></a>
# **leverageCollateralize**
> CollateralizeResponse leverageCollateralize(body)

Move supplied and available to supplied_collateral and collateral, for a specified position

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
CollateralizeRequest body = new CollateralizeRequest(); // CollateralizeRequest | 
try {
    CollateralizeResponse result = apiInstance.leverageCollateralize(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageCollateralize");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CollateralizeRequest**](CollateralizeRequest.md)|  |

### Return type

[**CollateralizeResponse**](CollateralizeResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageDeCollateralize"></a>
# **leverageDeCollateralize**
> DeCollateralizeResponse leverageDeCollateralize(body)

Move collateral and supplied_collateral to available and supplied, for a specified position.

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
DeCollateralizeRequest body = new DeCollateralizeRequest(); // DeCollateralizeRequest | 
try {
    DeCollateralizeResponse result = apiInstance.leverageDeCollateralize(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageDeCollateralize");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DeCollateralizeRequest**](DeCollateralizeRequest.md)|  |

### Return type

[**DeCollateralizeResponse**](DeCollateralizeResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageIsolateCollateral"></a>
# **leverageIsolateCollateral**
> IsolateCollateralResponse leverageIsolateCollateral(body)

Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageIsolatePosition"></a>
# **leverageIsolatePosition**
> IsolatePositionResponse leverageIsolatePosition(body)

Create an isolated position using all collateral, supplied_collateral, and borrows from the user&#x27;s global position

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
IsolatePositionRequest body = new IsolatePositionRequest(); // IsolatePositionRequest | 
try {
    IsolatePositionResponse result = apiInstance.leverageIsolatePosition(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageIsolatePosition");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**IsolatePositionRequest**](IsolatePositionRequest.md)|  |

### Return type

[**IsolatePositionResponse**](IsolatePositionResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
LiquidityRequest body = new LiquidityRequest(); // LiquidityRequest | 
UUID poolId = new UUID(); // UUID | 
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
 **poolId** | [**UUID**](.md)|  |

### Return type

[**LiquidityResponse**](LiquidityResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
LiquidityRequest body = new LiquidityRequest(); // LiquidityRequest | 
UUID poolId = new UUID(); // UUID | 
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
 **poolId** | [**UUID**](.md)|  |

### Return type

[**LiquidityResponse**](LiquidityResponse.md)

### Authorization

No authorization required

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
OffsetDateTime createdAfter = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime createdBefore = new OffsetDateTime(); // OffsetDateTime | 
AssetKind assetKind = new AssetKind(); // AssetKind | Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE)
Boolean canAddLiquidity = true; // Boolean | 
Boolean canDirectBorrow = true; // Boolean | 
Boolean canOnboard = true; // Boolean | 
Boolean canTrade = true; // Boolean | 
Boolean canVirtualBorrow = true; // Boolean | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
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
 **createdAfter** | **OffsetDateTime**|  | [optional]
 **createdBefore** | **OffsetDateTime**|  | [optional]
 **assetKind** | [**AssetKind**](.md)| Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE) | [optional]
 **canAddLiquidity** | **Boolean**|  | [optional]
 **canDirectBorrow** | **Boolean**|  | [optional]
 **canOnboard** | **Boolean**|  | [optional]
 **canTrade** | **Boolean**|  | [optional]
 **canVirtualBorrow** | **Boolean**|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
OrderBookStatus status = new OrderBookStatus(); // OrderBookStatus | 
UUID baseAssetId = new UUID(); // UUID | 
UUID quoteAssetId = new UUID(); // UUID | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
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
 **baseAssetId** | [**UUID**](.md)|  | [optional]
 **quoteAssetId** | [**UUID**](.md)|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**ListOrderBooksResponse**](ListOrderBooksResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
List<UUID> orderBookId = Arrays.asList(new UUID()); // List<UUID> | 
List<OrderKind> kind = Arrays.asList(new OrderKind()); // List<OrderKind> | 
List<OrderStatus> status = Arrays.asList(new OrderStatus()); // List<OrderStatus> | 
Side side = new Side(); // Side | 
OffsetDateTime from = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime to = new OffsetDateTime(); // OffsetDateTime | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
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
 **orderBookId** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional]
 **kind** | [**List&lt;OrderKind&gt;**](OrderKind.md)|  | [optional]
 **status** | [**List&lt;OrderStatus&gt;**](OrderStatus.md)|  | [optional]
 **side** | [**Side**](.md)|  | [optional]
 **from** | **OffsetDateTime**|  | [optional]
 **to** | **OffsetDateTime**|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**ListOrdersResponse**](ListOrdersResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamAssetPrices"></a>
# **streamAssetPrices**
> StreamAssetPricesResponse streamAssetPrices(since)

Stream real-time asset prices as map objects

Opens a WebSocket stream for real-time asset price updates. First message contains all current prices, subsequent messages contain only changed prices. Data is sent as JSON objects keyed by asset ID.

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    StreamAssetPricesResponse result = apiInstance.streamAssetPrices(since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamAssetPrices");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **since** | **OffsetDateTime**|  | [optional]

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
String orderBookId = "orderBookId_example"; // String | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
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
 **orderBookId** | **String**|  |
 **since** | **OffsetDateTime**|  | [optional]
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
UUID orderBookId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
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
 **orderBookId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

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
UUID orderBookId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
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
 **orderBookId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

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
UUID orderBookId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
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
 **orderBookId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**StreamTradesResponse**](StreamTradesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateUserConfig"></a>
# **updateUserConfig**
> UserUpdatedResponse updateUserConfig(body, userId)

Update user configuration by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UpdateUserConfigRequest body = new UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
UUID userId = new UUID(); // UUID | 
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
 **userId** | [**UUID**](.md)|  |

### Return type

[**UserUpdatedResponse**](UserUpdatedResponse.md)

### Authorization

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


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

No authorization required

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
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
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
 **userId** | [**UUID**](.md)|  |

### Return type

[**UserUpdatedResponse**](UserUpdatedResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

