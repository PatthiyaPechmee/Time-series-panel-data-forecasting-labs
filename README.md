# Time Series, Panel Data & Forecasting Labs
Python labs from TS 4016 at Columbia University (Fall 2025), covering time series trend analysis, panel data methods, and stationarity testing using real-world survey and administrative data.

---

## Lab 1 — Belief in the Afterlife: Trend Analysis
**Data:** General Social Survey (GSS), 1972–2022  
**Methods:** OLS with linear time trend, year fixed effects (dummies), subgroup analysis, interaction terms  
**Key finding:** Contrary to prior literature, belief in the afterlife has been increasing over time (+0.09 pp/year), and this trend holds similarly for both religious and non-religious respondents.  
**Libraries:** `pandas`, `numpy`, `statsmodels`, `matplotlib`, `seaborn`

---

## Lab 2 — Education Spending & Life Expectancy: Fixed Effects
**Data:** Quality of Government (QoG) Basic Dataset, 188 countries, 1970–2021  
**Methods:** Pooled OLS with year dummies, two-way fixed effects (PanelOLS), additional predictor (urbanization)  
**Key finding:** Education spending shows a positive but statistically insignificant effect on life expectancy once country and year fixed effects are applied. Urbanization partially mediates the relationship (β = 0.09, p < 0.05).  
**Libraries:** `pandas`, `statsmodels`, `linearmodels`

---

## Lab 3 — Crime Perception & Homicide Rate: Time Series Analysis
**Data:** Gallup annual polling (public crime perception) + FBI homicide statistics, 1989–present  
**Methods:** OLS on levels with linear time trend, first-differencing for stationarity, Durbin-Watson diagnostics  
**Key finding:** Level regression shows a strong correlation (β = 8.4) but significant autocorrelation (DW = 0.83). After first-differencing, the relationship holds (β = 7.3, p < 0.01) with substantially reduced autocorrelation (DW = 2.67).  
**Libraries:** `pandas`, `numpy`, `statsmodels`, `matplotlib`, `seaborn`
