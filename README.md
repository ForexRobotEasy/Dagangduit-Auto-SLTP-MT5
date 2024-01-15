# Dagangduit Auto SLTP MT5

This code is an Expert Advisor (EA) for MetaTrader 5 (MT5) developed by the Forex Robot Easy Team. The EA is designed to automatically manage stop loss (SL) and take profit (TP) levels for trades in the MT5 platform. It also includes additional features such as hiding SL and TP values, profit locking, and trailing stop.

## Input Parameters

1. StopLoss: Default stop loss in pips.
2. TakeProfit: Default take profit in pips.
3. HideSLTP: Option to hide SL and TP values.
4. LockProfit: Option to enable profit locking.
5. TrailingStop: Option to enable trailing stop.

## Global Variables

1. trailingStop: Trailing stop value.
2. initialStopLoss: Initial stop loss value.
3. initialTakeProfit: Initial take profit value.

## Initialization Function

The `OnInit()` function is executed during the EA initialization. It stores the initial SL and TP values and calculates the trailing stop value based on the current symbol digits.

## Deinitialization Function

The `OnDeinit()` function is executed when the EA is removed or the MT5 platform is closed. It restores the initial SL and TP values.

## Tick Function

The `OnTick()` function is executed on each tick of the market. It checks if the hide SL and TP option is enabled and hides the SL and TP values accordingly. It also checks if the profit locking option is enabled and adjusts the take profit level based on the current unrealized profit. Additionally, it checks if the trailing stop option is enabled and modifies the stop loss level based on the trailing stop value.

## Helper Functions

1. `HideStopLoss()`: Sets the stop loss to 0.
2. `HideTakeProfit()`: Sets the take profit to 0.
3. `LockProfitLevel()`: Calculates the current unrealized profit and adjusts the take profit level based on it.
4. `ApplyTrailingStop()`: Calculates the current unrealized profit and modifies the stop loss level based on the trailing stop value.

## Product Description

This code is a sample implementation of the Dagangduit Auto SLTP MT5 Expert Advisor developed by the Forex Robot Easy Team. It is designed to automate the management of stop loss and take profit levels for trades in the MT5 platform.

The EA offers several customizable options, including the ability to hide SL and TP values, enable profit locking, and activate a trailing stop. These features can help traders effectively manage their positions and optimize their trading strategies.

Please note that ForexRobotEasy is not the official developer of this product. We are showcasing a sample code that can work as described in the official product. To find the official developer and access more detailed reviews and trading results of this product, please visit the official website or use MQL5.

For detailed reviews and trading results of this product, please visit [https://forexroboteasy.com/forex-robot-review/dagangduit-auto-sltp-mt5-expert-review-and-results/](https://forexroboteasy.com/forex-robot-review/dagangduit-auto-sltp-mt5-expert-review-and-results/)
