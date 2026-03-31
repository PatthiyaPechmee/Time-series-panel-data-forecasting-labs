# Time Series, Panel Data & Forecasting Labs
Python labs from TS 4016 at Columbia University (Fall 2024), exploring time series analysis, trend modeling, and subgroup decomposition using real-world survey data.

---

## Lab 1 — Belief in the Afterlife: Trend Analysis (GSS Data)

**Research question:** Has belief in the afterlife in the United States changed over the past 50 years? Does it differ between people who identify with a religion vs. those who don't?

**Data:** General Social Survey (GSS), 1972–2022

**Methods:**
- Binary outcome construction from categorical survey responses
- Linear time trend OLS regression
- Year fixed effects (dummy variable) regression
- Subgroup analysis by religious affiliation
- Interaction term modeling (year × no-religion)

**Key findings:**
- Contrary to prior literature (Harley & Firebaugh, 1993), belief in the afterlife has been *increasing* slightly over time (+0.09 pp/year)
- Those with no religious affiliation are ~30 percentage points less likely to believe in the afterlife, but their trend mirrors the religious group
- The year × religion interaction is not statistically significant — both groups are increasing at the same rate

**Libraries:** `pandas`, `numpy`, `statsmodels`, `matplotlib`, `seaborn`, `scipy`
