# GunnersTrio Forex Software - ReadMe File

This ReadMe file provides a brief overview of the GunnersTrio Forex Software code. Please note that ForexRobotEasy is not the official developer of this product, but we are showcasing a sample code that can work as described in this product.

## Product Description

GunnersTrio Forex Software is a trading robot designed to provide stable income with minimal risk. It utilizes the author's indicator signal and a MACD filter to open and close orders.

For detailed reviews and trading results of this product, please visit our website: [https://forexroboteasy.com/forex-robot-review/gunnerstrio-forex-software-stable-income-with-minimal-risk-review/](https://forexroboteasy.com/forex-robot-review/gunnerstrio-forex-software-stable-income-with-minimal-risk-review/)

## Code Overview

The code is written in MQL5 and consists of the following sections:

### Input Parameters

- `LotSize`: Trading lot size (default: 0.01)
- `StopLoss`: Stop Loss distance in pips (default: 100)
- `TakeProfit`: Take Profit distance in pips (default: 200)

### Global Variables

- `ticket`: Order ticket number

### Initialization Function (OnInit)

This function is called when the expert advisor is initialized. It prints a message to indicate that the GunnersTrio Forex Software has been initialized.

### Deinitialization Function (OnDeinit)

This function is called when the expert advisor is deinitialized. It prints a message to indicate that the GunnersTrio Forex Software has been deinitialized.

### Tick Function (OnTick)

This function is called on every tick of the chart. It performs the following actions:

1. Checks if an order is already open.
2. If an order is open, checks if the order has failed to close. If so, it closes the order using a calm and non-aggressive series of orders.
3. If the order has been successfully closed, it prints a message and resets the ticket variable.
4. If no order is open, it checks the author's indicator signal and the MACD filter.
5. If both conditions are met, it opens a new order and prints a message.

### Author Indicator Signal (IsAuthorIndicatorSignal)

This function checks if the author's indicator signal is present. The logic to check the signal needs to be added. It should return true if the signal is present, and false otherwise.

### MACD Filter (IsMACDFilterPassed)

This function checks if the MACD filter is passed. The logic to check the filter needs to be added. It should return true if the filter is passed, and false otherwise.

## Disclaimer

Please note that ForexRobotEasy is not the official developer of the GunnersTrio Forex Software. We are only showcasing a sample code that can work as described in this product. To find the official developer of this product, kindly refer to the MQL5 platform.
