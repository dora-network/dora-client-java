# DefaultApi

All URIs are relative to *https://localhost:8084/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelAllOpenOrders**](DefaultApi.md#cancelAllOpenOrders) | **DELETE** /v1/orders | Cancel all open orders
[**cancelOrderById**](DefaultApi.md#cancelOrderById) | **DELETE** /v1/orders/{order_id} | Cancel an order by ID
[**createOrder**](DefaultApi.md#createOrder) | **POST** /v1/orders | Create a new order
[**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /v1/user/{user_id} | Delete user by ID
[**getAllAssetPrices**](DefaultApi.md#getAllAssetPrices) | **GET** /v1/price | Get the current price of all assets
[**getAssetById**](DefaultApi.md#getAssetById) | **GET** /v1/assets/{id} | Get asset by ID
[**getAssetPrice**](DefaultApi.md#getAssetPrice) | **GET** /v1/price/asset/{asset_id} | Get the current price of an asset
[**getCandleData**](DefaultApi.md#getCandleData) | **GET** /v1/charts/candle/{orderbook} | Get candlestick data for an orderbook
[**getCouponsByAssetId**](DefaultApi.md#getCouponsByAssetId) | **GET** /v1/assets/{id}/coupons | Get coupons for a bond asset
[**getL1Depth**](DefaultApi.md#getL1Depth) | **GET** /v1/orderbooks/{orderbook_id}/L1 | Get the top price levels for a specific orderbook (L1 market depth)
[**getL2Depth**](DefaultApi.md#getL2Depth) | **GET** /v1/orderbooks/{orderbook_id}/L2 | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getL3Depth**](DefaultApi.md#getL3Depth) | **GET** /v1/orderbooks/{orderbook_id}/L3 | Get all open orders for a specific orderbook (L3 market depth)
[**getLedgerBalancesSelf**](DefaultApi.md#getLedgerBalancesSelf) | **GET** /v1/ledger/balances/self | Get your own available, locked, and borrowed assets
[**getLedgerInterestSelf**](DefaultApi.md#getLedgerInterestSelf) | **GET** /v1/ledger/interest/self | Get your own interest
[**getLedgerModule**](DefaultApi.md#getLedgerModule) | **GET** /v1/ledger/module | Get the entire module object, including unborrowed leverage assets and total leverage trackers
[**getLedgerModuleByAsset**](DefaultApi.md#getLedgerModuleByAsset) | **GET** /v1/ledger/module/{asset_id} | Get the module object for a single asset ID
[**getLedgerPositionsSelf**](DefaultApi.md#getLedgerPositionsSelf) | **GET** /v1/ledger/positions/self | Get your own positions
[**getLedgerValueSelf**](DefaultApi.md#getLedgerValueSelf) | **GET** /v1/ledger/value/self | Get your own available, locked, and borrowed USD value; and realized and unrealized PnL
[**getOrderById**](DefaultApi.md#getOrderById) | **GET** /v1/orders/{order_id} | Get order by ID
[**getOrderbookBBO**](DefaultApi.md#getOrderbookBBO) | **GET** /v1/orderbooks/{orderbook_id}/bbo | Get the top price levels for a specific orderbook (L1 market depth)
[**getOrderbookById**](DefaultApi.md#getOrderbookById) | **GET** /v1/orderbooks/{orderbook_id} | Get orderbook by ID
[**getOrderbookDepth**](DefaultApi.md#getOrderbookDepth) | **GET** /v1/orderbooks/{orderbook_id}/depth | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getOrderbookOrders**](DefaultApi.md#getOrderbookOrders) | **GET** /v1/orderbooks/{orderbook_id}/orders | Get all open orders for a specific orderbook (L3 market depth)
[**getOrderbookSummary**](DefaultApi.md#getOrderbookSummary) | **GET** /v1/orderbooks/{orderbook_id}/summary | Get summary of an orderbook
[**getOrderbookTop**](DefaultApi.md#getOrderbookTop) | **GET** /v1/orderbooks/{orderbook_id}/top | Get the top price levels for a specific orderbook (L1 market depth)
[**getPoolPrice**](DefaultApi.md#getPoolPrice) | **GET** /v1/price/pool/{pool_id} | Get the current price of a pool
[**getTradeById**](DefaultApi.md#getTradeById) | **GET** /v1/trade/{trade_id} | Get a trade by ID
[**getTrades**](DefaultApi.md#getTrades) | **GET** /v1/trade | Get a filtered, paginated list of trades
[**getTransactionById**](DefaultApi.md#getTransactionById) | **GET** /v1/transactions/{id} | Get a transaction by ID
[**getTransactions**](DefaultApi.md#getTransactions) | **GET** /v1/transactions | Get a filtered, paginated list of transactions
[**getUserById**](DefaultApi.md#getUserById) | **GET** /v1/user/{user_id} | Get user by ID
[**getUserLedgerStream**](DefaultApi.md#getUserLedgerStream) | **GET** /v1/user/{user_id}/ledger/stream | Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates
[**getUserOrdersStream**](DefaultApi.md#getUserOrdersStream) | **GET** /v1/user/{user_id}/orders/{orderbook_id}/stream | Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates
[**getUserOrdersStreamAll**](DefaultApi.md#getUserOrdersStreamAll) | **GET** /v1/user/{user_id}/orders/all/stream | Get a snapshot of user&#x27;s order updates since a specific time, and opens a stream for further updates
[**getUserSelf**](DefaultApi.md#getUserSelf) | **GET** /v1/user/self | Get user details for the authenticated user
[**getUserTransactionsStream**](DefaultApi.md#getUserTransactionsStream) | **GET** /v1/user/{user_id}/transactions/stream | Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates
[**ledgerDeposit**](DefaultApi.md#ledgerDeposit) | **POST** /v1/ledger/deposit | Deposit assets into your account from the outside world
[**ledgerWithdraw**](DefaultApi.md#ledgerWithdraw) | **POST** /v1/ledger/withdraw | Withdraw assets from your account to the outside world
[**leverageBorrow**](DefaultApi.md#leverageBorrow) | **POST** /v1/leverage/borrow | Directly borrow assets
[**leverageCollateralize**](DefaultApi.md#leverageCollateralize) | **POST** /v1/leverage/collateralize | Move supplied and available to supplied_collateral and collateral, for a specified position
[**leverageDeCollateralize**](DefaultApi.md#leverageDeCollateralize) | **POST** /v1/leverage/de-collateralize | Move collateral and supplied_collateral to available and supplied, for a specified position.
[**leverageIsolateCollateral**](DefaultApi.md#leverageIsolateCollateral) | **POST** /v1/leverage/isolate_collateral | Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral
[**leverageIsolatePosition**](DefaultApi.md#leverageIsolatePosition) | **POST** /v1/leverage/isolate_position | Create an isolated position using all collateral, supplied_collateral, and borrows from the user&#x27;s global position
[**leverageRepay**](DefaultApi.md#leverageRepay) | **POST** /v1/leverage/repay | Repay borrowed assets
[**leverageSupply**](DefaultApi.md#leverageSupply) | **POST** /v1/leverage/supply | Supply leverage for a specific asset
[**leverageUnite**](DefaultApi.md#leverageUnite) | **POST** /v1/leverage/unite | Combines all isolated positions into a single global position
[**leverageWithdraw**](DefaultApi.md#leverageWithdraw) | **POST** /v1/leverage/withdraw | Withdraw leverage for a specific asset
[**liquidityAdd**](DefaultApi.md#liquidityAdd) | **POST** /v1/liquidity/pool/{pool_id}/add | Add liquidity to a pool
[**liquiditySubtract**](DefaultApi.md#liquiditySubtract) | **POST** /v1/liquidity/pool/{pool_id}/subtract | Subtract liquidity from a pool
[**listAssets**](DefaultApi.md#listAssets) | **GET** /v1/assets | List assets
[**listOrderBooks**](DefaultApi.md#listOrderBooks) | **GET** /v1/orderbooks | List order books
[**listOrders**](DefaultApi.md#listOrders) | **GET** /v1/orders | List all orders
[**streamAssetPrices**](DefaultApi.md#streamAssetPrices) | **GET** /v1/price/stream | Get a snapshot of asset prices from a specific date and open a stream for real-time updates
[**streamCandleData**](DefaultApi.md#streamCandleData) | **GET** /v1/charts/candle/stream/{orderbook} | Get a snapshot of candlestick data from date provided, and open a stream for real-time updates
[**streamOrderBookBalances**](DefaultApi.md#streamOrderBookBalances) | **GET** /v1/orderbooks/{orderbook_id}/stream/balances | Get a snapshot of base and quote balances for an order book and open a stream for real-time updates
[**streamOrderbookOpenOrders**](DefaultApi.md#streamOrderbookOpenOrders) | **GET** /v1/orderbooks/{orderbook_id}/stream/open | Get a snapshot of open orders in an order book and open a stream for real-time updates
[**streamTrades**](DefaultApi.md#streamTrades) | **GET** /v1/trade/{orderbook_id}/stream | Get a snapshot of trades from a specific date and open a stream for real-time updates
[**updateUserConfig**](DefaultApi.md#updateUserConfig) | **PUT** /v1/user/{user_id}/config | Update user configuration by ID
[**updateUserConfigSelf**](DefaultApi.md#updateUserConfigSelf) | **PUT** /v1/user/config/self | Update user configuration for the authenticated user
[**verifyUser**](DefaultApi.md#verifyUser) | **PUT** /v1/user/{user_id}/verify | Verify a user by ID

<a name="cancelAllOpenOrders"></a>
# **cancelAllOpenOrders**
> InlineResponse20015 cancelAllOpenOrders()

Cancel all open orders

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    InlineResponse20015 result = apiInstance.cancelAllOpenOrders();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#cancelAllOpenOrders");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse20015**](InlineResponse20015.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="cancelOrderById"></a>
# **cancelOrderById**
> InlineResponse204 cancelOrderById(orderId)

Cancel an order by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderId = new UUID(); // UUID | 
try {
    InlineResponse204 result = apiInstance.cancelOrderById(orderId);
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

[**InlineResponse204**](InlineResponse204.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="createOrder"></a>
# **createOrder**
> OrderId createOrder(body)

Create a new order

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
CreateOrderRequest body = new CreateOrderRequest(); // CreateOrderRequest | 
try {
    OrderId result = apiInstance.createOrder(body);
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

[**OrderId**](OrderId.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteUser"></a>
# **deleteUser**
> InlineResponse2004 deleteUser(userId)

Delete user by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
try {
    InlineResponse2004 result = apiInstance.deleteUser(userId);
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

[**InlineResponse2004**](InlineResponse2004.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAllAssetPrices"></a>
# **getAllAssetPrices**
> InlineResponse20028 getAllAssetPrices()

Get the current price of all assets

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    InlineResponse20028 result = apiInstance.getAllAssetPrices();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAllAssetPrices");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse20028**](InlineResponse20028.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetById"></a>
# **getAssetById**
> InlineResponse2001 getAssetById(id)

Get asset by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse2001 result = apiInstance.getAssetById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getAssetById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAssetPrice"></a>
# **getAssetPrice**
> InlineResponse20029 getAssetPrice(assetId)

Get the current price of an asset

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID assetId = new UUID(); // UUID | 
try {
    InlineResponse20029 result = apiInstance.getAssetPrice(assetId);
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

[**InlineResponse20029**](InlineResponse20029.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getCandleData"></a>
# **getCandleData**
> InlineResponse20017 getCandleData(orderbook, start, end, resolution)

Get candlestick data for an orderbook

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
String orderbook = "orderbook_example"; // String | 
OffsetDateTime start = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime end = new OffsetDateTime(); // OffsetDateTime | 
String resolution = "resolution_example"; // String | 
try {
    InlineResponse20017 result = apiInstance.getCandleData(orderbook, start, end, resolution);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getCandleData");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbook** | **String**|  |
 **start** | **OffsetDateTime**|  | [optional]
 **end** | **OffsetDateTime**|  | [optional]
 **resolution** | **String**|  | [optional] [enum: 1m, 5m, 15m, 1h, 4h, 1d]

### Return type

[**InlineResponse20017**](InlineResponse20017.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getCouponsByAssetId"></a>
# **getCouponsByAssetId**
> InlineResponse2002 getCouponsByAssetId(id, start, end, page, limit)

Get coupons for a bond asset

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
OffsetDateTime start = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime end = new OffsetDateTime(); // OffsetDateTime | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
try {
    InlineResponse2002 result = apiInstance.getCouponsByAssetId(id, start, end, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getCouponsByAssetId");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |
 **start** | **OffsetDateTime**|  | [optional]
 **end** | **OffsetDateTime**|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL1Depth"></a>
# **getL1Depth**
> InlineResponse20012 getL1Depth(orderbookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse20012 result = apiInstance.getL1Depth(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getL1Depth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20012**](InlineResponse20012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL2Depth"></a>
# **getL2Depth**
> InlineResponse20011 getL2Depth(orderbookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse20011 result = apiInstance.getL2Depth(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getL2Depth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20011**](InlineResponse20011.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL3Depth"></a>
# **getL3Depth**
> InlineResponse2006 getL3Depth(orderbookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse2006 result = apiInstance.getL3Depth(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getL3Depth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerBalancesSelf"></a>
# **getLedgerBalancesSelf**
> InlineResponse20021 getLedgerBalancesSelf()

Get your own available, locked, and borrowed assets

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    InlineResponse20021 result = apiInstance.getLedgerBalancesSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerBalancesSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse20021**](InlineResponse20021.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerInterestSelf"></a>
# **getLedgerInterestSelf**
> InlineResponse20023 getLedgerInterestSelf()

Get your own interest

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    InlineResponse20023 result = apiInstance.getLedgerInterestSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerInterestSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse20023**](InlineResponse20023.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerModule"></a>
# **getLedgerModule**
> InlineResponse20018 getLedgerModule()

Get the entire module object, including unborrowed leverage assets and total leverage trackers

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    InlineResponse20018 result = apiInstance.getLedgerModule();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerModule");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse20018**](InlineResponse20018.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerModuleByAsset"></a>
# **getLedgerModuleByAsset**
> InlineResponse20019 getLedgerModuleByAsset(assetId)

Get the module object for a single asset ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID assetId = new UUID(); // UUID | 
try {
    InlineResponse20019 result = apiInstance.getLedgerModuleByAsset(assetId);
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

[**InlineResponse20019**](InlineResponse20019.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerPositionsSelf"></a>
# **getLedgerPositionsSelf**
> InlineResponse20020 getLedgerPositionsSelf()

Get your own positions

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    InlineResponse20020 result = apiInstance.getLedgerPositionsSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerPositionsSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse20020**](InlineResponse20020.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLedgerValueSelf"></a>
# **getLedgerValueSelf**
> InlineResponse20022 getLedgerValueSelf()

Get your own available, locked, and borrowed USD value; and realized and unrealized PnL

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    InlineResponse20022 result = apiInstance.getLedgerValueSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getLedgerValueSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse20022**](InlineResponse20022.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderById"></a>
# **getOrderById**
> InlineResponse20016 getOrderById(orderId)

Get order by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderId = new UUID(); // UUID | 
try {
    InlineResponse20016 result = apiInstance.getOrderById(orderId);
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

[**InlineResponse20016**](InlineResponse20016.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookBBO"></a>
# **getOrderbookBBO**
> InlineResponse20012 getOrderbookBBO(orderbookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse20012 result = apiInstance.getOrderbookBBO(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookBBO");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20012**](InlineResponse20012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookById"></a>
# **getOrderbookById**
> InlineResponse20010 getOrderbookById(orderbookId)

Get orderbook by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse20010 result = apiInstance.getOrderbookById(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20010**](InlineResponse20010.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookDepth"></a>
# **getOrderbookDepth**
> InlineResponse20011 getOrderbookDepth(orderbookId)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse20011 result = apiInstance.getOrderbookDepth(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookDepth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20011**](InlineResponse20011.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookOrders"></a>
# **getOrderbookOrders**
> InlineResponse2006 getOrderbookOrders(orderbookId)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse2006 result = apiInstance.getOrderbookOrders(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookOrders");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookSummary"></a>
# **getOrderbookSummary**
> InlineResponse20013 getOrderbookSummary(orderbookId)

Get summary of an orderbook

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse20013 result = apiInstance.getOrderbookSummary(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookSummary");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20013**](InlineResponse20013.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookTop"></a>
# **getOrderbookTop**
> InlineResponse20012 getOrderbookTop(orderbookId)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
try {
    InlineResponse20012 result = apiInstance.getOrderbookTop(orderbookId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookTop");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20012**](InlineResponse20012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getPoolPrice"></a>
# **getPoolPrice**
> InlineResponse20030 getPoolPrice(poolId)

Get the current price of a pool

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID poolId = new UUID(); // UUID | 
try {
    InlineResponse20030 result = apiInstance.getPoolPrice(poolId);
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

[**InlineResponse20030**](InlineResponse20030.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTradeById"></a>
# **getTradeById**
> InlineResponse20027 getTradeById(tradeId)

Get a trade by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID tradeId = new UUID(); // UUID | 
try {
    InlineResponse20027 result = apiInstance.getTradeById(tradeId);
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

[**InlineResponse20027**](InlineResponse20027.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTrades"></a>
# **getTrades**
> InlineResponse20026 getTrades(pools, userIds, start, end, page, limit)

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
    InlineResponse20026 result = apiInstance.getTrades(pools, userIds, start, end, page, limit);
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

[**InlineResponse20026**](InlineResponse20026.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTransactionById"></a>
# **getTransactionById**
> InlineResponse20025 getTransactionById(id)

Get a transaction by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse20025 result = apiInstance.getTransactionById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getTransactionById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20025**](InlineResponse20025.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTransactions"></a>
# **getTransactions**
> InlineResponse2008 getTransactions(pools, userIds, txKinds, start, end, page, limit)

Get a filtered, paginated list of transactions

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
List<String> pools = Arrays.asList("pools_example"); // List<String> | 
List<UUID> userIds = Arrays.asList(new UUID()); // List<UUID> | 
List<String> txKinds = Arrays.asList("txKinds_example"); // List<String> | 
OffsetDateTime start = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime end = new OffsetDateTime(); // OffsetDateTime | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
try {
    InlineResponse2008 result = apiInstance.getTransactions(pools, userIds, txKinds, start, end, page, limit);
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
 **txKinds** | [**List&lt;String&gt;**](String.md)|  | [optional] [enum: ACCRUE_INTEREST, ADD_LIQUIDITY, BOND_MATURE, CLAIM_INTEREST, CREDIT, DEBIT, EXTERNAL_DEPOSIT, EXTERNAL_WITHDRAW, FILL, LENDING_INTEREST_ACCRUAL, LIQUIDATE, MATCH_ORDER, PAY_INTEREST, SUBTRACT_LIQUIDITY, REPAY, SUPPLY, WITHDRAW, ISOLATE_COLLATERAL, ISOLATE_POSITION, UNITE_POSITION]
 **start** | **OffsetDateTime**|  | [optional]
 **end** | **OffsetDateTime**|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**InlineResponse2008**](InlineResponse2008.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserById"></a>
# **getUserById**
> InlineResponse2003 getUserById(userId)

Get user by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
try {
    InlineResponse2003 result = apiInstance.getUserById(userId);
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

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserLedgerStream"></a>
# **getUserLedgerStream**
> InlineResponse2007 getUserLedgerStream(userId, since)

Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse2007 result = apiInstance.getUserLedgerStream(userId, since);
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
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**InlineResponse2007**](InlineResponse2007.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserOrdersStream"></a>
# **getUserOrdersStream**
> InlineResponse2006 getUserOrdersStream(userId, orderbookId, since)

Get a snapshot of user&#x27;s order updates for the given order book since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
UUID orderbookId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse2006 result = apiInstance.getUserOrdersStream(userId, orderbookId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserOrdersStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**UUID**](.md)|  |
 **orderbookId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserOrdersStreamAll"></a>
# **getUserOrdersStreamAll**
> InlineResponse2006 getUserOrdersStreamAll(userId, since, orderbookIds)

Get a snapshot of user&#x27;s order updates since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
List<UUID> orderbookIds = Arrays.asList(new UUID()); // List<UUID> | 
try {
    InlineResponse2006 result = apiInstance.getUserOrdersStreamAll(userId, since, orderbookIds);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserOrdersStreamAll");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]
 **orderbookIds** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional]

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserSelf"></a>
# **getUserSelf**
> InlineResponse2003 getUserSelf()

Get user details for the authenticated user

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
try {
    InlineResponse2003 result = apiInstance.getUserSelf();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserSelf");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserTransactionsStream"></a>
# **getUserTransactionsStream**
> InlineResponse2008 getUserTransactionsStream(userId, since)

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
    InlineResponse2008 result = apiInstance.getUserTransactionsStream(userId, since);
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

[**InlineResponse2008**](InlineResponse2008.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="ledgerDeposit"></a>
# **ledgerDeposit**
> InlineResponse201 ledgerDeposit(body)

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
    InlineResponse201 result = apiInstance.ledgerDeposit(body);
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

[**InlineResponse201**](InlineResponse201.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="ledgerWithdraw"></a>
# **ledgerWithdraw**
> InlineResponse201 ledgerWithdraw(body)

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
    InlineResponse201 result = apiInstance.ledgerWithdraw(body);
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

[**InlineResponse201**](InlineResponse201.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageBorrow"></a>
# **leverageBorrow**
> InlineResponse2015 leverageBorrow(body)

Directly borrow assets

TODO: Finish this when implementation has been completed

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object body = null; // Object | 
try {
    InlineResponse2015 result = apiInstance.leverageBorrow(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageBorrow");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Object**](Object.md)|  |

### Return type

[**InlineResponse2015**](InlineResponse2015.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageCollateralize"></a>
# **leverageCollateralize**
> InlineResponse2011 leverageCollateralize(body)

Move supplied and available to supplied_collateral and collateral, for a specified position

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
CollateralizeRequest body = new CollateralizeRequest(); // CollateralizeRequest | 
try {
    InlineResponse2011 result = apiInstance.leverageCollateralize(body);
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

[**InlineResponse2011**](InlineResponse2011.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageDeCollateralize"></a>
# **leverageDeCollateralize**
> InlineResponse2012 leverageDeCollateralize(body)

Move collateral and supplied_collateral to available and supplied, for a specified position.

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
DeCollateralizeRequest body = new DeCollateralizeRequest(); // DeCollateralizeRequest | 
try {
    InlineResponse2012 result = apiInstance.leverageDeCollateralize(body);
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

[**InlineResponse2012**](InlineResponse2012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageIsolateCollateral"></a>
# **leverageIsolateCollateral**
> InlineResponse2016 leverageIsolateCollateral(body)

Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
IsolateCollateralRequest body = new IsolateCollateralRequest(); // IsolateCollateralRequest | 
try {
    InlineResponse2016 result = apiInstance.leverageIsolateCollateral(body);
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

[**InlineResponse2016**](InlineResponse2016.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageIsolatePosition"></a>
# **leverageIsolatePosition**
> InlineResponse2017 leverageIsolatePosition(body)

Create an isolated position using all collateral, supplied_collateral, and borrows from the user&#x27;s global position

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
IsolatePositionRequest body = new IsolatePositionRequest(); // IsolatePositionRequest | 
try {
    InlineResponse2017 result = apiInstance.leverageIsolatePosition(body);
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

[**InlineResponse2017**](InlineResponse2017.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageRepay"></a>
# **leverageRepay**
> InlineResponse2015 leverageRepay(body)

Repay borrowed assets

TODO: Finish this when implementation has been completed

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
Object body = null; // Object | 
try {
    InlineResponse2015 result = apiInstance.leverageRepay(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#leverageRepay");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Object**](Object.md)|  |

### Return type

[**InlineResponse2015**](InlineResponse2015.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageSupply"></a>
# **leverageSupply**
> InlineResponse2013 leverageSupply(body)

Supply leverage for a specific asset

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
SupplyRequest body = new SupplyRequest(); // SupplyRequest | 
try {
    InlineResponse2013 result = apiInstance.leverageSupply(body);
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

[**InlineResponse2013**](InlineResponse2013.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageUnite"></a>
# **leverageUnite**
> InlineResponse20024 leverageUnite(body)

Combines all isolated positions into a single global position

TODO: Finish this when implementation has been completed

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UnitePositionRequest body = new UnitePositionRequest(); // UnitePositionRequest | 
try {
    InlineResponse20024 result = apiInstance.leverageUnite(body);
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

[**InlineResponse20024**](InlineResponse20024.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageWithdraw"></a>
# **leverageWithdraw**
> InlineResponse2014 leverageWithdraw(body)

Withdraw leverage for a specific asset

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
WithdrawRequest body = new WithdrawRequest(); // WithdrawRequest | 
try {
    InlineResponse2014 result = apiInstance.leverageWithdraw(body);
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

[**InlineResponse2014**](InlineResponse2014.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquidityAdd"></a>
# **liquidityAdd**
> InlineResponse2018 liquidityAdd(body, poolId)

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
    InlineResponse2018 result = apiInstance.liquidityAdd(body, poolId);
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

[**InlineResponse2018**](InlineResponse2018.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquiditySubtract"></a>
# **liquiditySubtract**
> InlineResponse2018 liquiditySubtract(body, poolId)

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
    InlineResponse2018 result = apiInstance.liquiditySubtract(body, poolId);
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

[**InlineResponse2018**](InlineResponse2018.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="listAssets"></a>
# **listAssets**
> InlineResponse200 listAssets(createdAfter, createdBefore, assetKind, canAddLiquidity, canDirectBorrow, canOnboard, canTrade, canVirtualBorrow, page, limit)

List assets

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
OffsetDateTime createdAfter = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime createdBefore = new OffsetDateTime(); // OffsetDateTime | 
String assetKind = "assetKind_example"; // String | Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE)
Boolean canAddLiquidity = true; // Boolean | 
Boolean canDirectBorrow = true; // Boolean | 
Boolean canOnboard = true; // Boolean | 
Boolean canTrade = true; // Boolean | 
Boolean canVirtualBorrow = true; // Boolean | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
try {
    InlineResponse200 result = apiInstance.listAssets(createdAfter, createdBefore, assetKind, canAddLiquidity, canDirectBorrow, canOnboard, canTrade, canVirtualBorrow, page, limit);
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
 **assetKind** | **String**| Asset kind (BOND, CURRENCY, INTEREST, POOL_SHARE) | [optional]
 **canAddLiquidity** | **Boolean**|  | [optional]
 **canDirectBorrow** | **Boolean**|  | [optional]
 **canOnboard** | **Boolean**|  | [optional]
 **canTrade** | **Boolean**|  | [optional]
 **canVirtualBorrow** | **Boolean**|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrderBooks"></a>
# **listOrderBooks**
> InlineResponse2009 listOrderBooks(status, baseAssetId, quoteAssetId, page, limit)

List order books

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
String status = "status_example"; // String | 
UUID baseAssetId = new UUID(); // UUID | 
UUID quoteAssetId = new UUID(); // UUID | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
try {
    InlineResponse2009 result = apiInstance.listOrderBooks(status, baseAssetId, quoteAssetId, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#listOrderBooks");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **String**|  | [optional] [enum: OPEN, CLOSED, SUSPENDED]
 **baseAssetId** | [**UUID**](.md)|  | [optional]
 **quoteAssetId** | [**UUID**](.md)|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**InlineResponse2009**](InlineResponse2009.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrders"></a>
# **listOrders**
> InlineResponse2006 listOrders(orderbookId, kind, status, side, from, to, page, limit)

List all orders

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
List<UUID> orderbookId = Arrays.asList(new UUID()); // List<UUID> | 
String kind = "kind_example"; // String | 
String status = "status_example"; // String | 
String side = "side_example"; // String | 
OffsetDateTime from = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime to = new OffsetDateTime(); // OffsetDateTime | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
try {
    InlineResponse2006 result = apiInstance.listOrders(orderbookId, kind, status, side, from, to, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#listOrders");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional]
 **kind** | **String**|  | [optional] [enum: LIMIT, MARKET]
 **status** | **String**|  | [optional] [enum: OPEN, CLOSED, CANCELED]
 **side** | **String**|  | [optional] [enum: BUY, SELL]
 **from** | **OffsetDateTime**|  | [optional]
 **to** | **OffsetDateTime**|  | [optional]
 **page** | **Integer**|  | [optional] [default to 1]
 **limit** | **Integer**|  | [optional] [default to 100]

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamAssetPrices"></a>
# **streamAssetPrices**
> InlineResponse20028 streamAssetPrices(since)

Get a snapshot of asset prices from a specific date and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse20028 result = apiInstance.streamAssetPrices(since);
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

[**InlineResponse20028**](InlineResponse20028.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamCandleData"></a>
# **streamCandleData**
> InlineResponse20017 streamCandleData(orderbook, since, resolution)

Get a snapshot of candlestick data from date provided, and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
String orderbook = "orderbook_example"; // String | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
String resolution = "resolution_example"; // String | 
try {
    InlineResponse20017 result = apiInstance.streamCandleData(orderbook, since, resolution);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamCandleData");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbook** | **String**|  |
 **since** | **OffsetDateTime**|  | [optional]
 **resolution** | **String**|  | [optional] [enum: 1m, 5m, 15m, 1h, 4h, 1d]

### Return type

[**InlineResponse20017**](InlineResponse20017.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamOrderBookBalances"></a>
# **streamOrderBookBalances**
> InlineResponse20014 streamOrderBookBalances(orderbookId, since)

Get a snapshot of base and quote balances for an order book and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse20014 result = apiInstance.streamOrderBookBalances(orderbookId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamOrderBookBalances");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**InlineResponse20014**](InlineResponse20014.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamOrderbookOpenOrders"></a>
# **streamOrderbookOpenOrders**
> InlineResponse2006 streamOrderbookOpenOrders(orderbookId, since)

Get a snapshot of open orders in an order book and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse2006 result = apiInstance.streamOrderbookOpenOrders(orderbookId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamOrderbookOpenOrders");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="streamTrades"></a>
# **streamTrades**
> TradeResponse streamTrades(orderbookId, since)

Get a snapshot of trades from a specific date and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID orderbookId = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    TradeResponse result = apiInstance.streamTrades(orderbookId, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamTrades");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderbookId** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]

### Return type

[**TradeResponse**](TradeResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateUserConfig"></a>
# **updateUserConfig**
> InlineResponse2005 updateUserConfig(body, userId)

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
    InlineResponse2005 result = apiInstance.updateUserConfig(body, userId);
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

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateUserConfigSelf"></a>
# **updateUserConfigSelf**
> InlineResponse2005 updateUserConfigSelf(body)

Update user configuration for the authenticated user

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UpdateUserConfigRequest body = new UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
try {
    InlineResponse2005 result = apiInstance.updateUserConfigSelf(body);
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

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="verifyUser"></a>
# **verifyUser**
> InlineResponse2005 verifyUser(userId)

Verify a user by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID userId = new UUID(); // UUID | 
try {
    InlineResponse2005 result = apiInstance.verifyUser(userId);
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

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

