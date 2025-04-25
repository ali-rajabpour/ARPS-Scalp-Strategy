# ARPS Scalp Strategy
**Originally created: July 31, 2020**
*(Note: This script was created in 2020 but is being shared on GitHub on April 25, 2025)*

---

The **ARPS Scalp Strategy** is a highly sophisticated, feature-rich Pine Script designed to enhance your trading analysis and decision-making process. It combines a wide range of powerful indicators, candlestick pattern detection, and trend-following methodologies into a single tool optimized for scalping strategies. Whether you're a beginner or an advanced trader, this indicator provides actionable insights to refine your strategy in highly dynamic markets.

---

## Key Features

### 1. **Alligator Oscillator (AO)**
   - Calculation of AO using smoothed moving averages (SMA) of `hl2` with short-term (5) and long-term (34) periods to determine market momentum.

### 2. **RSI-Stochastic Integration**
   - Combines relative strength index (RSI) and stochastic-related weighted moving averages (WMA) for identifying overbought and oversold conditions.
   - Configurable inputs for Stochastic settings (`K`, `D`, and smoothing parameters).

### 3. **Zero Lag Exponential Moving Averages (EMAs)**
   - Accurate rendering of 50-period and 200-period zero-lag EMAs for enhanced trend direction identification.
   - Dynamic calculations to correct lag and improve responsiveness.

### 4. **Advanced Candlestick Pattern Detection**
   - Real-time identification of multiple reversal and continuation patterns, including:
     - **Doji (Standard, FlyDragon, Gravestone)**.
     - **Morning Star & Evening Star**.
     - **Shooting Star & Hammer**.
     - **Bearish/Bullish Harami & Engulfing**.
     - **Dark Cloud Cover**.
   - Capability to monitor both current and previous candles for pattern detection.

### 5. **Ichimoku Cloud Integration**
   - Configurable Ichimoku Cloud settings to identify equilibrium, trend reversals, and support/resistance zones.
   - Double Ichimoku Cloud setup for adjusted, multi-timeframe analysis.

### 6. **Parabolic SAR**
   - Utilizes the Parabolic SAR indicator with adjustable step and maximum values to spot potential trend reversals.

### 7. **Trend Continuation Factor (TCF)**
   - Measures the strength of upward or downward trend continuation by summing directional price changes.
   - Provides accurate signals for scalping entries.

### 8. **Multi-layered Trading Signal Logic**
   - Long and Short conditions generated based on:
     - RSI & Stochastic Crosses.
     - EMA Crossovers (50-period vs. 200-period).
     - AO trend changes.
     - Bullish/Bearish Pattern alignment with trend conditions.

### 9. **Custom Alerts for Entries**
   - Alerts for actionable Long and Short entries to ensure the user doesn't miss opportunities.
   - Visual label annotations on key levels for easier decision-making.

---

## Configuration Options

### Inputs
- **Candlestick Patterns**: Size thresholds for Doji and Star patterns (`Doji's Max Body size`, `Previous Doji size`, etc.).
- **Indicators**: Adjustable lengths, periods, and sources for AO, RSI-Stochastic, EMAs, SAR, and Ichimoku Cloud parameters.
- **Ichimoku Settings**:
  - `Tenkan-sen`, `Kijun-sen`, `Senkou Span B` customizable periods.
  - Enable/Disable double-Ichimoku mode to enhance signal precision.

---

## How It Works

1. **Trend Identification**:
   - Detects major trend conditions using Zero-Lag EMA crossovers and Ichimoku Cloud positioning.
2. **Reversal & Entry Points**:
   - Pinpoints market transitions via candlestick patterns, AO changes, and SAR signals.
3. **Confirmation Signals**:
   - Uses RSI-Stochastic alignment or TCF crossover to validate entry conditions.

### Visual Elements
- **Candlestick Patterns**: Marked directly on the chart as arrows, labels, or shapes.
- **Clouds**: Painted with different colors based on Ichimoku strength and conditions.
- **Labels and Alerts**: Highlight Buy/Sell opportunities for scalping.

---

## Alerts & Notifications

Integrated `alertcondition()` functions for key events:
- **Long Entry**: Triggered for conditions matching strong bullish signals.
- **Short Entry**: Triggered for conditions matching strong bearish signals.

---

## Usage

### How to Install the Script
1. Open your TradingView account.
2. Paste the provided code into the Pine Script editor in TradingView.
3. Save the script under your desired name and add it to your chart.

---

## Example Screen

![Example Screenshot](INSERT_LINK_TO_SCREENSHOT)

*The chart demonstrates real-time Doji patterns, Ichimoku Cloud analysis, and Zero-Lag EMA trend positioning, with visual annotations for Long/Short entries.*

---

## Indicators Breakdown

| **Indicator**         | **Methodology**               | **Purpose**                                      |
|------------------------|-------------------------------|--------------------------------------------------|
| AO                    | SMA of `hl2`                 | Identify momentum shifts.                       |
| RSI + Stochastic       | WMA of RSI                   | Identify overbought/oversold levels.            |
| Zero Lag EMAs          | Advanced EMA calculation     | Detect trend directions with zero lag.          |
| Parabolic SAR          | Points plotted above/below   | Spot potential reversal points.                 |
| Ichimoku Cloud         | Multi-line cloud system      | Assess market phases and equilibrium.           |

---

## License
This script is provided under the **MIT License**. Attribution to the original author, Ali Rajabpour-Sanati, is required for redistribution. Contact for licensing inquiries: ali.poursanati@gmail.com.

---

## Contact
For any questions, feedback, or bug reporting:
- Author: **Ali Rajabpour-Sanati**
- Email: ali.poursanati@gmail.com

---

## Contributing
Contributions to the ARPS Scalp Strategy Suite are welcome. Open an issue or submit a pull request to suggest features or improvements.
