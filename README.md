# Asymmetric Effects of Oil Price Shocks on the Indian Equity Market  
### A Comparative Analysis of Sustainable versus Conventional Finance

This is my dissertation project which was completed as part of the MSc in Finance and Management at Edinburgh Business School, Heriot-Watt University.

The project investigates how global crude-oil price shocks and domestic inflation are transmitted to India’s conventional and sustainable equity markets. It compares the **Nifty 100**, a broad conventional Indian equity index, with the **Nifty 100 ESG**, an index of large Indian companies screened for stronger environmental, social, and governance performance.

Using monthly data from **January 2013 to December 2024**, the study applies a **Nonlinear Autoregressive Distributed Lag (NARDL)** framework to test whether rising and falling oil prices have different long-run effects on equity returns. It also examines whether the ESG index shows a different response to inflation once its close relationship with the broader Indian market is taken into account.

## Research Questions

1. Do rising oil prices affect the two indices more negatively in the long run than falling prices affect them positively?
2. How does the Nifty 100 ESG index respond to Indian CPI inflation compared with the conventional Nifty 100 index?
3. Does the estimated relationship remain stable once the 2022 Russia–Ukraine war period is accounted for?

## Key Findings

- Both indices show evidence of a long-run relationship with oil-price movements and CPI inflation.
- The Wald tests find **no statistically significant long-run asymmetry** between positive and negative oil-price shocks for either index.
- The conventional Nifty 100 has a statistically significant positive long-run CPI coefficient.
- The ESG index’s CPI coefficient is not statistically distinguishable from zero once broad-market co-movement with the Nifty 100 is controlled for.
- Results are materially unchanged when the 2022 war dummy is removed, suggesting that the findings are not driven solely by the Russia–Ukraine war shock.

## Methodology

The study uses two parallel **Nonlinear Autoregressive Distributed Lag (NARDL)** models:

- **Model 1:** Nifty 100 as the dependent variable.
- **Model 2:** Nifty 100 ESG as the dependent variable, with Nifty 100 included as a market-control variable.

Brent crude-oil price changes are decomposed into positive and negative partial sums, following the NARDL framework. The models also include Indian CPI, a COVID-19 dummy for March–April 2020, and a Russia–Ukraine war dummy for February–June 2022.

The INR/USD exchange rate and RBI repo rate were retrieved from the Reserve Bank of India for contextual purposes only and are not included as regressors in the main models.


The analysis includes:

- ADF and KPSS stationarity tests  
- Zivot–Andrews structural-break testing  
- AIC and SBC-based lag selection  
- ARDL bounds tests for cointegration  
- Wald tests for long-run asymmetry  
- Dynamic multiplier analysis  
- CUSUM and CUSUMSQ stability tests  
- Breusch–Godfrey autocorrelation diagnostics  
- Robustness checks excluding the 2022 war dummy  

All estimation was carried out in **Gretl**, with the ADMBP add-on used for long-run multiplier estimation and dynamic multiplier charts.


## Software

- **Gretl** — primary econometric estimation software  
- **ADMBP add-on** — long-run and dynamic multiplier estimation  
- **Excel** — data cleaning and preliminary preparation  
- **EViews 14 Student Lite** — initial estimation attempts  

## Limitations

- The study uses aggregate index-level data, so it cannot identify sector-specific ESG effects.
- The Nifty 100 ESG index closely co-moves with the conventional Nifty 100, making it difficult to isolate an independent ESG effect.
- The model measures statistical association rather than proving causality.
- The analysis does not formally separate the direct oil-price channel from monetary-policy responses.
- Future work could include the RBI repo rate, sector-level ESG data, index-overlap analysis, and cross-equation tests of CPI sensitivity.
