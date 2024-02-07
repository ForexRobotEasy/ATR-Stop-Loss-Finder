# ATR Stop Loss Finder - ReadMe

This code is designed to be used as a custom indicator in MetaTrader 4. It calculates the Average True Range (ATR) and uses it to determine stop loss and take profit levels for trades. The ATR is a volatility indicator that measures the average range of price movement over a specified period of time. By multiplying the ATR by user-defined multipliers, this indicator generates stop loss and take profit levels that adjust dynamically based on market volatility.

## Input Parameters

- **Length**: Specifies the number of bars used for ATR calculation. Default value is 14.
- **Smoothing**: Sets the smoothing factor for the ATR. A higher value results in a smoother ATR line. Default value is 3.
- **Multiplier1**: The first multiplier used to calculate the stop loss and take profit levels. Default value is 1.0.
- **Multiplier2**: The optional second multiplier used to calculate the stop loss and take profit levels. Default value is 0.0.

## Customization Settings

- **EnableHighPrice**: Enables customization of the high price line color. Default value is true.
- **EnableLowPrice**: Enables customization of the low price line color. Default value is true.
- **EnableShowPriceLine**: Enables customization of the price line visibility. Default value is true.
- **ColorHigh**: Specifies the custom color for the high price line. Default value is Red.
- **ColorLow**: Specifies the custom color for the low price line. Default value is Green.
- **ColorPriceLine**: Specifies the custom color for the price line. Default value is Blue.

## Initialization Function

The OnInit() function is called when the indicator is initialized. It sets the indicator buffers and label.

## Calculation Function

The OnCalculate() function is called for each new tick. It calculates the ATR values and then uses them to determine the stop loss and take profit levels based on the current price and multipliers.

## Deinitialization Function

The OnDeinit() function is called when the indicator is removed from the chart. It is currently empty and can be used for any necessary deinitialization tasks.

Please note that Forex Robot Easy is not the official developer of this product. We only provide this sample code that demonstrates how the product can work as described. To find the official developer and obtain the complete version of this product, please visit [MQL5](https://www.mql5.com/).

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - ATR Stop Loss Finder Review](https://forexroboteasy.com/forex-robot-review/atr-stop-loss-finder-review-optimize-forex-trades-with-ease/).
