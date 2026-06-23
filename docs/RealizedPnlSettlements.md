

# RealizedPnlSettlements


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**settlements** | [**List&lt;RealizedPnlSettlement&gt;**](RealizedPnlSettlement.md) | A list of realized PnL settlements matching the query parameters of the request |  [optional] |
|**userTotals** | **Map&lt;String, String&gt;** | A map of user IDs to their total realized PnL in USD across all settlements included in the response |  [optional] |
|**tenantTotals** | **Map&lt;String, String&gt;** | A map of tenant IDs to their total realized PnL in USD across all settlements included in the response |  [optional] |
|**userTotalsUnsettled** | **Map&lt;String, String&gt;** | A map of user IDs to their total realized PnL in USD across unsettled settlements (where settled_at is null) included in the response |  [optional] |
|**tenantTotalsUnsettled** | **Map&lt;String, String&gt;** | A map of tenant IDs to their total realized PnL in USD across unsettled settlements (where settled_at is null) included in the response |  [optional] |



