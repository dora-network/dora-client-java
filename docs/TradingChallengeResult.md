

# TradingChallengeResult


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**tradingChallengeId** | **UUID** |  |  [optional] |
|**userId** | **UUID** |  |  [optional] |
|**userName** | **String** |  |  [optional] |
|**cumVolume** | **String** |  |  [optional] |
|**cumPnl** | **String** |  |  [optional] |
|**pnlPct** | **String** |  |  [optional] |
|**calendarDaysSinceStart** | **Integer** |  |  [optional] |
|**activeDays** | **Integer** |  |  [optional] |
|**compliantDays** | **Integer** |  |  [optional] |
|**crownEligible** | **Boolean** |  |  [optional] |
|**claimEligible** | **Boolean** |  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |
|**crown** | [**CrownEnum**](#CrownEnum) |  |  [optional] |
|**createdAt** | **OffsetDateTime** |  |  [optional] |
|**currentDayDailyVolume** | **String** |  |  [optional] |
|**currentDayDailyPnl** | **String** |  |  [optional] |
|**currentDayTradingDate** | **LocalDate** |  |  [optional] |
|**cumTrades** | **Integer** |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| PENDING | &quot;PENDING&quot; |
| FUNDED | &quot;FUNDED&quot; |
| ACTIVE | &quot;ACTIVE&quot; |
| BUSTED | &quot;BUSTED&quot; |
| COMPLETED | &quot;COMPLETED&quot; |
| PRIZE_CLAIMED | &quot;PRIZE_CLAIMED&quot; |



## Enum: CrownEnum

| Name | Value |
|---- | -----|
| NONE | &quot;NONE&quot; |
| PNL_GOLD | &quot;PNL_GOLD&quot; |
| PNL_SILVER | &quot;PNL_SILVER&quot; |
| PNL_BRONZE | &quot;PNL_BRONZE&quot; |
| VOLUME_GOLD | &quot;VOLUME_GOLD&quot; |
| VOLUME_SILVER | &quot;VOLUME_SILVER&quot; |
| VOLUME_BRONZE | &quot;VOLUME_BRONZE&quot; |
| IRON_GOLD | &quot;IRON_GOLD&quot; |
| IRON_SILVER | &quot;IRON_SILVER&quot; |
| IRON_BRONZE | &quot;IRON_BRONZE&quot; |



