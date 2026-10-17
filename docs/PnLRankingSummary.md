

# PnLRankingSummary


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**allUsersDailyTradingVolume** | **String** | Sum of daily_trading_volume across all users matching ranking filters before pagination. |  |
|**allUsersTotalTradingVolume** | **String** | Sum of total_trading_volume across all users matching ranking filters before pagination. |  |
|**allUsersAvgDailyTradingVolume** | **String** | all_users_total_trading_volume divided by the number of distinct UTC days on which any matching user had an executed fill. 0 if there are none. |  |
|**allUsersAvgDailyTradingVolumeOnNDays** | **String** | Executed trading volume within [start, end) across all users matching ranking filters, divided by the number of requested days elapsed so far (end clamped to now, partial days rounded up). 0 if start is in the future. |  |



