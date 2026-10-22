# Bond Pricing & Interest Rate Risk Analysis

## Overview

A Python-based fixed-income analytics project that calculates the price, yield to maturity (YTM), modified duration and DV01 of a fixed-rate bond. It also evaluates the bond's sensitivity to changes in market yields through scenario analysis and visualization.

The project applies fundamental fixed-income valuation and risk concepts using Python.

## Features

- **Bond Pricing:** Discounts future coupon payments and principal repayment to calculate the bond's present value.
- **Yield to Maturity:** Uses SciPy's `brentq` root-finding algorithm to determine the yield implied by an observed market price.
- **Modified Duration:** Calculates Macaulay and modified duration to measure interest-rate sensitivity.
- **DV01:** Estimates the monetary price sensitivity to a one-basis-point change in yield.
- **Scenario Analysis:** Reprices the bond under yield shifts ranging from −200 to +200 basis points.
- **Visualization:** Plots the inverse relationship between bond prices and yields using Matplotlib.

## Tools and Libraries

- Python
- NumPy
- SciPy
- Matplotlib
- Google Colab / Jupyter Notebook

## Model Assumptions

The analysis uses an illustrative fixed-rate bond with the following characteristics:

| Parameter | Value |
|---|---|
| Face Value | KES 100,000 |
| Annual Coupon Rate | 12% |
| Remaining Maturity | 5 years |
| Coupon Frequency | Semiannual |
| Market Price | KES 96,000 |

The model assumes regular coupon payments, settlement on a coupon date, a flat yield to maturity and no credit or liquidity adjustments. It excludes accrued interest, transaction costs and taxes.

## Methodology

The model first calculates bond prices by discounting future cash flows. It then solves for the YTM implied by the market price.

Modified duration and DV01 are used to quantify interest-rate exposure, while scenario analysis evaluates the potential mark-to-market impact of changes in yields.

## How to Run

1. Open `Bond_Pricing_and_Risk.ipynb` in Google Colab or Jupyter Notebook.
2. Run the cells sequentially.
3. Modify the bond assumptions to analyze different coupon rates, maturities and market prices.
4. Review the calculated risk measures, scenario results and price-yield chart.

## Limitations

This is an introductory fixed-income analytics project rather than a full market-convention bond pricing system. It uses simplified cash-flow timing and parallel yield changes, without modelling yield-curve dynamics, credit spreads or liquidity effects.

## Project Purpose

Developed as a practical application of fixed-income valuation and interest-rate risk concepts while building foundational Python programming and numerical analysis skills.
