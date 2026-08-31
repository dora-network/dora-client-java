

# PnLRankingResponse


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**userId** | **UUID** |  |  |
|**firstName** | **String** |  |  |
|**totalPnl** | **String** |  |  |
|**realizedPnl** | **String** | Cumulative realized PnL across the user&#39;s full trading lifetime. |  |
|**totalTrades** | **Integer** |  |  |
|**winningTrades** | **Integer** |  |  |
|**losingTrades** | **Integer** |  |  |
|**winRate** | **String** |  |  |
|**dailyTradingVolume** | **String** | Executed trading volume for the current UTC day. |  |
|**totalTradingVolume** | **String** | Cumulative executed trading volume across all UTC trading days. |  |
|**activeTradingDays** | **Integer** | Number of distinct UTC days on which the user has at least one executed fill. |  |
|**activated** | **Boolean** | True once the user has traded on at least 5 distinct UTC days. |  |
|**kycApproved** | **Boolean** | Whether the user is currently considered KYC/verification approved. |  |



