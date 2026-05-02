# Macroeconomic Time Series Analysis – Central America  
### Panel Time Series, Forecasting & Economic Dynamics  
**Structural Diagnostics, Growth Dynamics & Predictive Assessment**

---

## Project Overview

The objective of this project is to analyze the **temporal dynamics of macroeconomic development in Central America** using a structured panel time series framework.

The analysis combines:

- Time series diagnostics (stationarity, autocorrelation)
- Cross-country macroeconomic comparison
- Short-term forecasting of economic growth
- Evaluation of predictive limits in macroeconomic dynamics

The focus is not purely predictive accuracy, but rather:

> Understanding whether short-term economic growth contains stable and exploitable temporal structure.

---

## Dataset

The dataset is based on the **UN National Accounts Main Aggregates Database**, covering seven Central American countries over multiple decades.

It includes engineered features such as:

- Log-transformed macroeconomic levels
- Growth-rate transformations
- Lagged variables

This structure enables separation between:

- Long-run structural dynamics (levels)
- Short-run cyclical fluctuations (growth rates)

---

## Data Structure

### Panel Time Series Design

Each country is treated as an independent time series within a panel structure.

Key macroeconomic variables include:

- GDP and GDP growth
- Per capita GNI
- Trade flows (exports and imports)
- Gross capital formation
- Final consumption expenditure
- Population

---

## Exploratory Time Series Diagnostics

### Levels vs Growth Rates

A central empirical result is the clear distinction between:

- **Log-level variables → non-stationary**
- **Growth-rate variables → mostly stationary**

| Dimension | Finding | Interpretation |
|----------|--------|---------------|
| Log-level variables | Predominantly non-stationary | Long-run structural growth and trend components |
| Growth-rate variables | Mostly stationary | Short-run cyclical fluctuations around stable means |
| Trade & investment growth | Strong stationarity | High sensitivity to shocks and fast mean reversion |
| GDP growth | Weak persistence | Limited short-term memory |

---

### Cross-Country Heterogeneity

- Panama and Belize: higher volatility
- Nicaragua: extreme investment fluctuations
- Guatemala and Costa Rica: more stable dynamics

Economic structures and shock responses differ significantly across countries.

---

## Statistical Diagnostics

### Stationarity (ADF Test)

Key findings:

- Strong rejection of unit roots in growth rates
- Persistent non-stationarity in log-levels
- Borderline cases in some GDP growth series

Only growth-rate variables are suitable for short-term forecasting.

---

### Autocorrelation Analysis

- Rapid decay of autocorrelation (typically 1–2 lags)
- Weak to moderate short-term persistence
- Strong heterogeneity across countries

Growth dynamics behave as mostly short-memory processes.

---

## Forecasting Framework

Forecasting is applied exclusively to:

> GDP growth rates (stationary series)

### Models Compared

- Random Walk (baseline)
- AR(1)
- ARIMA(1,0,1)

Objective:

> Evaluate whether short-term predictability exists beyond a naive benchmark.

---

## Baseline Model: Random Walk

The Random Walk assumes:

> The best forecast is the last observed value.

Findings:

- Strong benchmark performance in several countries
- Indicates limited exploitable structure in growth dynamics

---

## AR(1) Model

- Captures short-term persistence
- Weak and inconsistent improvement over baseline
- Strong heterogeneity across countries

---

## ARIMA(1,0,1) Model

- Adds moving average component
- No systematic improvement over AR(1)
- Confirms weak short-memory structure

---

## Forecast Evaluation (RMSE)

Performance evaluated using out-of-sample RMSE.

| Model | Interpretation |
|------|---------------|
| Random Walk | Strong baseline in multiple countries |
| AR(1) | Limited improvement |
| ARIMA(1,0,1) | No consistent gain |

<img width="1331" height="547" alt="image" src="https://github.com/user-attachments/assets/f3935d36-54f3-4f41-b006-177fc42d4019" />

Key result:

> Increasing model complexity does not systematically improve predictive accuracy.

---

## Key Empirical Findings

- Growth rates are mostly stationary
- Short-term GDP growth is weakly predictable
- Random Walk remains highly competitive
- AR and ARIMA models provide limited added value
- Strong cross-country heterogeneity exists

---

## Economic Interpretation

Macroeconomic dynamics in Central America exhibit a dual structure:

- Long-run structural growth trends
- Short-run stochastic fluctuations

Key implication:

> Short-term growth is largely driven by external shocks rather than persistent internal dynamics.

---

## Limitations

| Limitation | Description | Impact |
|------------|------------|--------|
| Aggregated macro data | No sectoral breakdown | Hidden internal heterogeneity |
| Linear models only | No nonlinear methods | Possible underfitting |
| Annual frequency | Low temporal resolution | Limits short-term signal detection |
| No exogenous variables | Pure autoregressive setup | External shocks not modeled |
| Small panel | Limited observations per country | Reduces statistical power |

---

## Conclusion

This project provides a structured analysis of macroeconomic time series dynamics in Central America.

Key insight:

> While long-term macroeconomic variables are structurally persistent, short-term growth dynamics are largely dominated by stochastic shocks and exhibit limited predictability.

The combination of:

- statistical diagnostics  
- time series modeling  
- forecasting evaluation  

provides a coherent framework for understanding both the structure and limitations of macroeconomic predictability in the region.
