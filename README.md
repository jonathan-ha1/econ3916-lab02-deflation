# econ3916-lab02-deflation
Deflating Economic Data — Nominal vs. Real

Objective

This project quantifies the divergence between nominal and inflation-adjusted (real) economic indicators by constructing a CPI-based deflation pipeline and applying it to U.S. wage and consumer price data.

Methodology

Retrieved historical Consumer Price Index (CPI) and Average Hourly Earnings series directly from the Federal Reserve Economic Data (FRED) API using unauthenticated public endpoints
Designed and implemented a reusable deflation function to convert nominal time series into constant (real) dollar terms using a selectable base year
Rebased all series to constant 2020 dollars to enable consistent, apples-to-apples comparison across the full sample period
Applied the deflation methodology to two independent series — average hourly earnings and the U.S. Big Mac price — to validate the approach across different data types
Calculated nominal, real, and CPI growth rates over the full date range to isolate the inflation component of each series' change
Developed an interactive deflation explorer featuring a base-year slider, allowing dynamic re-basing and real-time recalculation of real values

Key Findings

Wages: Nominal average hourly earnings rose from $2.50 to $32.53 over the sample period — a substantial nominal gain. However, once adjusted for inflation, real earnings grew far more modestly, from $20.92 to $25.20, revealing that a large share of the nominal wage increase reflects inflation rather than genuine purchasing power growth.
Big Mac Price: The nominal U.S. Big Mac price increased 178% over the same period, while CPI rose 95%. After deflating, the real price increase was 43% — indicating that Big Mac prices outpaced general inflation, representing genuine real price appreciation beyond the economy-wide cost-of-living increase.
Broader Insight: Across both series, the analysis demonstrates that nominal figures alone can substantially overstate real economic gains, underscoring the importance of CPI-adjustment when evaluating long-run trends in wages and prices.
