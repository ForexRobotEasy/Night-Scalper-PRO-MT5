# Night Scalper PRO MT5

This repository contains the code for the Night Scalper PRO MT5 expert advisor. Night Scalper PRO is a multi-currency expert advisor developed by Forex Robot Easy Team. Please note that ForexRobotEasy is not the official developer of this product, but we are providing a sample code that can work as described in this product.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Night Scalper PRO MT5 Review](https://forexroboteasy.com/forex-robot-review/night-scalper-pro-mt5-review-multi-currency-expert-advisor/).

## Input Parameters

- SymbolName: The symbol name to trade (default: 'EURUSD')
- TimeFrame: The timeframe to trade (default: PERIOD_M15)
- LotSize: The lot size for trading (default: 0.01)
- MaxSpread: The maximum allowed spread for trading (default: 5)
- UseNewsFilter: Enable/disable the news filter (default: true)

## Expert Advisor Start Function

The expert advisor starts by checking if it's the end of the day using the `IsEndOfDay()` function. If it's the end of the day, it calculates the upper and lower shadow of the daily candle. If both shadows exist, it checks if the spread is within the maximum allowed spread. If the spread is acceptable, it checks if the news filter is enabled and there are no important news using the `IsImportantNews()` function. If the news filter is disabled or there are no important news, it opens a trade using the `OpenTrade()` function.

## Functions

### IsEndOfDay()

This function checks if it's the end of the day. It compares the current time with the end of the day time (23:00). If the current time is after 23:00, it sets the end of the day time to the next day. It returns true if it's the end of the day, false otherwise.

### IsImportantNews()

This function checks if there are any important news. The logic to check for important news is not implemented in the code and should be implemented by the user. It should return true if there are important news, false otherwise.

### OpenTrade()

This function is responsible for opening a trade. The logic to open a trade is not implemented in the code and should be implemented by the user. The LotSize input parameter should be used as the lot size for the trade. Necessary stop loss and take profit levels should also be implemented.

Please note that this is a sample code and the actual implementation may vary. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Night Scalper PRO MT5 Review](https://forexroboteasy.com/forex-robot-review/night-scalper-pro-mt5-review-multi-currency-expert-advisor/).
