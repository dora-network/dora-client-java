# DefaultApi

All URIs are relative to *https://localhost:8080/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelAllOpenOrders**](DefaultApi.md#cancelAllOpenOrders) | **DELETE** /orders | Cancel all open orders
[**cancelOrderById**](DefaultApi.md#cancelOrderById) | **DELETE** /orders/{order_id} | Cancel an order by ID
[**createOrder**](DefaultApi.md#createOrder) | **POST** /orders | Create a new order
[**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /user/{id} | Delete user by ID
[**getAllAssetPrices**](DefaultApi.md#getAllAssetPrices) | **GET** /price | Get the current price of all assets
[**getAssetById**](DefaultApi.md#getAssetById) | **GET** /assets/{id} | Get asset by ID
[**getAssetPrice**](DefaultApi.md#getAssetPrice) | **GET** /price/asset/{asset_id} | Get the current price of an asset
[**getCandleData**](DefaultApi.md#getCandleData) | **GET** /charts/candle/{orderbook} | Get candlestick data for an orderbook
[**getCouponsByAssetId**](DefaultApi.md#getCouponsByAssetId) | **GET** /assets/{id}/coupons | Get coupons for a bond asset
[**getL3Depth**](DefaultApi.md#getL3Depth) | **GET** /orderbooks/{id}/orders | Get all open orders for a specific orderbook (L3 market depth)
[**getL3Depth_0**](DefaultApi.md#getL3Depth_0) | **GET** /orderbooks/{id}/L3 | Get all open orders for a specific orderbook (L3 market depth)
[**getLedgerBalancesSelf**](DefaultApi.md#getLedgerBalancesSelf) | **GET** /ledger/balances/self | Get your own available, locked, and borrowed assets
[**getLedgerInterestSelf**](DefaultApi.md#getLedgerInterestSelf) | **GET** /ledger/interest/self | Get your own interest
[**getLedgerModule**](DefaultApi.md#getLedgerModule) | **GET** /ledger/module | Get the entire module object, including unborrowed leverage assets and total leverage trackers
[**getLedgerModuleByAsset**](DefaultApi.md#getLedgerModuleByAsset) | **GET** /ledger/module/{asset_id} | Get the module object for a single asset ID
[**getLedgerPositionsSelf**](DefaultApi.md#getLedgerPositionsSelf) | **GET** /ledger/positions/self | Get your own positions
[**getLedgerValueSelf**](DefaultApi.md#getLedgerValueSelf) | **GET** /ledger/value/self | Get your own available, locked, and borrowed USD value; and realized and unrealized PnL
[**getOrderById**](DefaultApi.md#getOrderById) | **GET** /orders/{order_id} | Get order by ID
[**getOrderbookById**](DefaultApi.md#getOrderbookById) | **GET** /orderbooks/{id} | Get orderbook by ID
[**getOrderbookDepth**](DefaultApi.md#getOrderbookDepth) | **GET** /orderbooks/{id}/depth | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getOrderbookDepth_0**](DefaultApi.md#getOrderbookDepth_0) | **GET** /orderbooks/{id}/L2 | Get the aggregated price levels for a specific orderbook (L2 market depth)
[**getOrderbookSummary**](DefaultApi.md#getOrderbookSummary) | **GET** /orderbooks/{id}/summary | Get summary of an orderbook
[**getOrderbookTop**](DefaultApi.md#getOrderbookTop) | **GET** /orderbooks/{id}/top | Get the top price levels for a specific orderbook (L1 market depth)
[**getOrderbookTop_0**](DefaultApi.md#getOrderbookTop_0) | **GET** /orderbooks/{id}/L1 | Get the top price levels for a specific orderbook (L1 market depth)
[**getPoolPrice**](DefaultApi.md#getPoolPrice) | **GET** /price/pool/{pool_id} | Get the current price of a pool
[**getTradeById**](DefaultApi.md#getTradeById) | **GET** /trade/{id} | Get a trade by ID
[**getTrades**](DefaultApi.md#getTrades) | **GET** /trade | Get a filtered, paginated list of trades
[**getTransactionById**](DefaultApi.md#getTransactionById) | **GET** /transactions/{id} | Get a transaction by ID
[**getTransactions**](DefaultApi.md#getTransactions) | **GET** /transactions | Get a filtered, paginated list of transactions
[**getUserById**](DefaultApi.md#getUserById) | **GET** /user/{id} | Get user by ID
[**getUserLedgerStream**](DefaultApi.md#getUserLedgerStream) | **GET** /user/{id}/ledger/stream | Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates
[**getUserOrdersStream**](DefaultApi.md#getUserOrdersStream) | **GET** /user/{id}/orders/stream | Get a snapshot of user&#x27;s order updates since a specific time, and opens a stream for further updates
[**getUserTransactionsStream**](DefaultApi.md#getUserTransactionsStream) | **GET** /user/{id}/transactions/stream | Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates
[**ledgerDeposit**](DefaultApi.md#ledgerDeposit) | **POST** /ledger/deposit | Deposit assets into your account from the outside world
[**ledgerWithdraw**](DefaultApi.md#ledgerWithdraw) | **POST** /ledger/withdraw | Withdraw assets from your account to the outside world
[**leverageBorrow**](DefaultApi.md#leverageBorrow) | **POST** /leverage/borrow | Directly borrow assets
[**leverageIsolateCollateral**](DefaultApi.md#leverageIsolateCollateral) | **POST** /leverage/isolate_collateral | Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral
[**leverageIsolatePosition**](DefaultApi.md#leverageIsolatePosition) | **POST** /leverage/isolate_position | Create an isolated position using all collateral, supplied_collateral, and borrows from the user&#x27;s global position
[**leverageRepay**](DefaultApi.md#leverageRepay) | **POST** /leverage/repay | Repay borrowed assets
[**leverageSupply**](DefaultApi.md#leverageSupply) | **POST** /leverage/supply | Supply leverage for a specific asset
[**leverageUnite**](DefaultApi.md#leverageUnite) | **POST** /leverage/unite | Combines all isolated positions into a single global position
[**leverageWithdraw**](DefaultApi.md#leverageWithdraw) | **POST** /leverage/withdraw | Withdraw leverage for a specific asset
[**liquidityAdd**](DefaultApi.md#liquidityAdd) | **POST** /liquidity/pool/{pool_id}/add | Add liquidity to a pool
[**liquiditySubtract**](DefaultApi.md#liquiditySubtract) | **POST** /liquidity/pool/{pool_id}/subtract | Subtract liquidity from a pool
[**listAssets**](DefaultApi.md#listAssets) | **GET** /assets | List assets
[**listOrderBooks**](DefaultApi.md#listOrderBooks) | **GET** /orderbooks | List order books
[**listOrders**](DefaultApi.md#listOrders) | **GET** /orders | List all orders
[**streamAssetPrices**](DefaultApi.md#streamAssetPrices) | **GET** /price/stream | Get a snapshot of asset prices from a specific date and open a stream for real-time updates
[**streamCandleData**](DefaultApi.md#streamCandleData) | **GET** /charts/candle/stream/{orderbook} | Get a snapshot of candlestick data from date provided, and open a stream for real-time updates
[**streamOrderBookBalances**](DefaultApi.md#streamOrderBookBalances) | **GET** /orderbooks/{id}/stream/balances | Get a snapshot of base and quote balances for an order book and open a stream for real-time updates
[**streamOrderbookOpenOrders**](DefaultApi.md#streamOrderbookOpenOrders) | **GET** /orderbooks/{id}/stream/open | Get a snapshot of open orders in an order book and open a stream for real-time updates
[**streamTrades**](DefaultApi.md#streamTrades) | **GET** /trade/stream | Get a snapshot of trades from a specific date and open a stream for real-time updates
[**updateUserConfig**](DefaultApi.md#updateUserConfig) | **PUT** /user/{id}/config | Update user configuration by ID
[**verifyUser**](DefaultApi.md#verifyUser) | **PUT** /user/{id}/verify | Verify a user by ID

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
> InlineResponse2004 deleteUser(id)

Delete user by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse2004 result = apiInstance.deleteUser(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#deleteUser");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

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

<a name="getL3Depth"></a>
# **getL3Depth**
> InlineResponse2006 getL3Depth(id)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse2006 result = apiInstance.getL3Depth(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getL3Depth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getL3Depth_0"></a>
# **getL3Depth_0**
> InlineResponse2006 getL3Depth_0(id)

Get all open orders for a specific orderbook (L3 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse2006 result = apiInstance.getL3Depth_0(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getL3Depth_0");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

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

<a name="getOrderbookById"></a>
# **getOrderbookById**
> InlineResponse20010 getOrderbookById(id)

Get orderbook by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse20010 result = apiInstance.getOrderbookById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20010**](InlineResponse20010.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookDepth"></a>
# **getOrderbookDepth**
> InlineResponse20011 getOrderbookDepth(id)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse20011 result = apiInstance.getOrderbookDepth(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookDepth");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20011**](InlineResponse20011.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookDepth_0"></a>
# **getOrderbookDepth_0**
> InlineResponse20011 getOrderbookDepth_0(id)

Get the aggregated price levels for a specific orderbook (L2 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse20011 result = apiInstance.getOrderbookDepth_0(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookDepth_0");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20011**](InlineResponse20011.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookSummary"></a>
# **getOrderbookSummary**
> InlineResponse20013 getOrderbookSummary(id)

Get summary of an orderbook

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse20013 result = apiInstance.getOrderbookSummary(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookSummary");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20013**](InlineResponse20013.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookTop"></a>
# **getOrderbookTop**
> InlineResponse20012 getOrderbookTop(id)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse20012 result = apiInstance.getOrderbookTop(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookTop");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse20012**](InlineResponse20012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getOrderbookTop_0"></a>
# **getOrderbookTop_0**
> InlineResponse20012 getOrderbookTop_0(id)

Get the top price levels for a specific orderbook (L1 market depth)

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse20012 result = apiInstance.getOrderbookTop_0(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getOrderbookTop_0");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

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
> InlineResponse20027 getTradeById(id)

Get a trade by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse20027 result = apiInstance.getTradeById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getTradeById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

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
 **txKinds** | [**List&lt;String&gt;**](String.md)|  | [optional]
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
> InlineResponse2003 getUserById(id)

Get user by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse2003 result = apiInstance.getUserById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserLedgerStream"></a>
# **getUserLedgerStream**
> InlineResponse2007 getUserLedgerStream(id, since)

Get a snapshot of user&#x27;s ledger updates since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse2007 result = apiInstance.getUserLedgerStream(id, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserLedgerStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |
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
> InlineResponse2006 getUserOrdersStream(id, since, orderbookIds)

Get a snapshot of user&#x27;s order updates since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
List<UUID> orderbookIds = Arrays.asList(new UUID()); // List<UUID> | 
try {
    InlineResponse2006 result = apiInstance.getUserOrdersStream(id, since, orderbookIds);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserOrdersStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |
 **since** | **OffsetDateTime**|  | [optional]
 **orderbookIds** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional]

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserTransactionsStream"></a>
# **getUserTransactionsStream**
> InlineResponse2008 getUserTransactionsStream(id, since)

Get a snapshot of user&#x27;s executed transactions since a specific time, and opens a stream for further updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse2008 result = apiInstance.getUserTransactionsStream(id, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getUserTransactionsStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |
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
> InlineResponse2013 leverageBorrow(body)

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
    InlineResponse2013 result = apiInstance.leverageBorrow(body);
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

[**InlineResponse2013**](InlineResponse2013.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageIsolateCollateral"></a>
# **leverageIsolateCollateral**
> InlineResponse2014 leverageIsolateCollateral(body)

Create an isolated position by transferring collateral to the position from the user&#x27;s global collateral

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
IsolateCollateralRequest body = new IsolateCollateralRequest(); // IsolateCollateralRequest | 
try {
    InlineResponse2014 result = apiInstance.leverageIsolateCollateral(body);
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

[**InlineResponse2014**](InlineResponse2014.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageIsolatePosition"></a>
# **leverageIsolatePosition**
> InlineResponse2015 leverageIsolatePosition(body)

Create an isolated position using all collateral, supplied_collateral, and borrows from the user&#x27;s global position

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
IsolatePositionRequest body = new IsolatePositionRequest(); // IsolatePositionRequest | 
try {
    InlineResponse2015 result = apiInstance.leverageIsolatePosition(body);
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

[**InlineResponse2015**](InlineResponse2015.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageRepay"></a>
# **leverageRepay**
> InlineResponse2013 leverageRepay(body)

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
    InlineResponse2013 result = apiInstance.leverageRepay(body);
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

[**InlineResponse2013**](InlineResponse2013.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="leverageSupply"></a>
# **leverageSupply**
> InlineResponse2011 leverageSupply(body)

Supply leverage for a specific asset

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
SupplyRequest body = new SupplyRequest(); // SupplyRequest | 
try {
    InlineResponse2011 result = apiInstance.leverageSupply(body);
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

[**InlineResponse2011**](InlineResponse2011.md)

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
> InlineResponse2012 leverageWithdraw(body)

Withdraw leverage for a specific asset

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
WithdrawRequest body = new WithdrawRequest(); // WithdrawRequest | 
try {
    InlineResponse2012 result = apiInstance.leverageWithdraw(body);
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

[**InlineResponse2012**](InlineResponse2012.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquidityAdd"></a>
# **liquidityAdd**
> InlineResponse2016 liquidityAdd(body, poolId)

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
    InlineResponse2016 result = apiInstance.liquidityAdd(body, poolId);
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

[**InlineResponse2016**](InlineResponse2016.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="liquiditySubtract"></a>
# **liquiditySubtract**
> InlineResponse2016 liquiditySubtract(body, poolId)

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
    InlineResponse2016 result = apiInstance.liquiditySubtract(body, poolId);
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

[**InlineResponse2016**](InlineResponse2016.md)

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
> InlineResponse2009 listOrderBooks(createdAfter, createdBefore, page, limit)

List order books

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
OffsetDateTime createdAfter = new OffsetDateTime(); // OffsetDateTime | 
OffsetDateTime createdBefore = new OffsetDateTime(); // OffsetDateTime | 
Integer page = 1; // Integer | 
Integer limit = 100; // Integer | 
try {
    InlineResponse2009 result = apiInstance.listOrderBooks(createdAfter, createdBefore, page, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#listOrderBooks");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createdAfter** | **OffsetDateTime**|  | [optional]
 **createdBefore** | **OffsetDateTime**|  | [optional]
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
> InlineResponse20017 streamCandleData(since, resolution)

Get a snapshot of candlestick data from date provided, and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
String resolution = "resolution_example"; // String | 
try {
    InlineResponse20017 result = apiInstance.streamCandleData(since, resolution);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamCandleData");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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
> InlineResponse20014 streamOrderBookBalances(id, since)

Get a snapshot of base and quote balances for an order book and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse20014 result = apiInstance.streamOrderBookBalances(id, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamOrderBookBalances");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |
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
> InlineResponse2006 streamOrderbookOpenOrders(id, since)

Get a snapshot of open orders in an order book and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
try {
    InlineResponse2006 result = apiInstance.streamOrderbookOpenOrders(id, since);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamOrderbookOpenOrders");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |
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
> TradeResponse streamTrades(since, orderbookIds)

Get a snapshot of trades from a specific date and open a stream for real-time updates

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
OffsetDateTime since = new OffsetDateTime(); // OffsetDateTime | 
List<UUID> orderbookIds = Arrays.asList(new UUID()); // List<UUID> | 
try {
    TradeResponse result = apiInstance.streamTrades(since, orderbookIds);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#streamTrades");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **since** | **OffsetDateTime**|  | [optional]
 **orderbookIds** | [**List&lt;UUID&gt;**](UUID.md)|  | [optional]

### Return type

[**TradeResponse**](TradeResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateUserConfig"></a>
# **updateUserConfig**
> InlineResponse2005 updateUserConfig(body, id)

Update user configuration by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UpdateUserConfigRequest body = new UpdateUserConfigRequest(); // UpdateUserConfigRequest | 
UUID id = new UUID(); // UUID | 
try {
    InlineResponse2005 result = apiInstance.updateUserConfig(body, id);
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
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="verifyUser"></a>
# **verifyUser**
> InlineResponse2005 verifyUser(id)

Verify a user by ID

### Example
```java
// Import classes:
//import tech.dora.ApiException;
//import tech.dora.api.DefaultApi;


DefaultApi apiInstance = new DefaultApi();
UUID id = new UUID(); // UUID | 
try {
    InlineResponse2005 result = apiInstance.verifyUser(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#verifyUser");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**UUID**](.md)|  |

### Return type

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

