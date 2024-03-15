# XAUUSD Scalper M1

This is a trading script developed by the Forex Robot Easy Team. For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/xauusd-scalper-m1-review-limited-time-180-offer/). Please note that ForexRobotEasy is not the official developer of this product. We only provide this sample code that can work as described in the product. To find the official developer of this product, please use MQL5.

## Description
The XAUUSD Scalper M1 script is designed to execute scalping trades on the XAUUSD (Gold) currency pair using the 1-minute chart. It aims to take advantage of short-term price movements by opening and closing multiple trades throughout the day.

## Features
- Minimum and maximum number of trades per day can be set using input parameters.
- Stop loss and take profit levels can be customized.
- The script automatically closes all open orders when the maximum number of trades is reached.
- It opens new trades when the minimum number of trades has not been reached and a new trading opportunity occurs.

## How it works
1. The script initializes by retrieving the previous price of the XAUUSD pair.
2. On each tick, the script compares the current price with the previous price to check if a new trading opportunity has occurred.
3. If the price movement exceeds the specified stop loss level, the script proceeds to check the number of trades.
4. If the maximum number of trades has been reached, all open orders are closed, and the trades count is reset.
5. If the minimum number of trades has not been reached, a new trade is opened with a lot size calculated based on the account's free margin and the specified stop loss level.
6. The script updates the previous price with the current price.
7. When the script is deinitialized, it closes all open orders.

## Input Parameters
- `minTrades` (default: 2): Minimum number of trades per day.
- `maxTrades` (default: 10): Maximum number of trades per day.
- `stopLossPips` (default: 10): Stop loss level in pips.
- `takeProfitPips` (default: 20): Take profit level in pips.

## Disclaimer
Please note that ForexRobotEasy is not the official developer of this product. We only provide this sample code that can work as described in the product. To find the official developer of this product, please use MQL5.
