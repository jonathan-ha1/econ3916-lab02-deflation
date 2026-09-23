# Deflating Economic Data — Nominal vs. Real

## Objective
This project quantifies the divergence between nominal and inflation-adjusted (real) economic indicators by constructing a CPI-based deflation pipeline and applying it to U.S. wage and price data.

## Methodology
- Retrieved Consumer Price Index (CPI) and Average Hourly Earnings series directly from the FRED API without requiring an API key
- Developed a reusable `deflate_series()` function to convert nominal time series into constant-dollar (real) terms using a selectable base year
- Applied the deflation methodology to two series: average hourly earnings and the U.S. Big Mac price, both rebased to constant 2020 dollars
- Built an interactive deflation explorer allowing users to adjust the base year via a slider and observe the resulting shift in real values in real time

## Key Findings
- **Wages:** Nominal average hourly earnings rose from $2.50 to $32.53 over the sample period, an increase that overstates actual purchasing power gains. In constant 2020 dollars, real earnings rose more modestly from $20.92 to $25.20.
- **Big Mac Price:** The nominal price of a U.S. Big Mac increased by 178% over the same period. After adjusting for inflation (CPI +95%), the real increase was only 43% — indicating that a substantial share of the nominal price growth reflects broad-based inflation rather than a rise in the Big Mac's real cost.
- **Broader Implication:** The comparison across both series illustrates how nominal figures can significantly overstate real economic change, reinforcing the importance of CPI deflation when interpreting long-run price and wage trends.
