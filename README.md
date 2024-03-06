# Super Fibo Idea

This code is a sample implementation of the Super Fibo Idea trading system. It provides functionality for calculating Fibonacci retracement levels, scanning for potential entry points, and executing trades. Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Custom Fibonacci Retracement

The `CalculateFibonacciLevels` function calculates Fibonacci retracement levels based on the provided array of high and low prices. It iterates through the bars and calculates the levels using the formula `lows[i] + (range * ratio)`, where `ratio` is the Fibonacci ratio (0.236, 0.382, 0.5, 0.618). The calculated levels are stored in the `fibonacciLevels` array.

## Scanning System for Entry

The `ScanForEntryPoints` function scans the Fibonacci levels for potential entry points based on the current price. It iterates through the Fibonacci levels and checks if the current price is within the support and resistance levels. If it is, it further checks if the current price is below the 38.2% level for a potential buying entry point or above the 61.8% level for a potential selling entry point. You can add your trading logic within the respective if statements.

## Trading Panel Implementation

The `OnChartEvent` function handles the trading panel events. It listens for the `CHARTEVENT_CLICK` event and checks the `sparam` parameter to determine if the 'Buy' or 'Sell' button was clicked. If the 'Buy' button is clicked, you can add your logic to execute a buy trade. Similarly, if the 'Sell' button is clicked, you can add your logic to execute a sell trade.

## Super Fibo Idea

The `OnTick` function is the main entry point for the trading system. It collects the highs and lows data from the currency market and calculates the Fibonacci levels using the `CalculateFibonacciLevels` function. It then retrieves the current price and calls the `ScanForEntryPoints` function to scan for potential entry points based on the Fibonacci levels and the current price.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Super Fibo Idea Review](https://forexroboteasy.com/forex-robot-review/super-fibo-idea-review-enhance-forex-trading-with-optional-panel/).

Please note that the provided link is for detailed reviews and trading results of the Super Fibo Idea product on Forex Robot Easy. ForexRobotEasy is not the official developer of this product.
