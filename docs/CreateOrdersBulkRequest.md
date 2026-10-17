

# CreateOrdersBulkRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**orders** | [**List&lt;CreateOrderRequest&gt;**](CreateOrderRequest.md) | Orders to submit, all with the same &#x60;order_book_id&#x60;. The maximum is configurable (matching.bulk_order_max_orders, default 20). |  |
|**atomic** | **Boolean** | Not currently supported: must be omitted or false, and &#x60;true&#x60; is rejected with 400. Orders are processed independently and partial creation is allowed. |  [optional] |



