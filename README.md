# Forecasting Non-Communicable Diseases (NCDs) at QECH, Malawi

**Undergraduate thesis project — BSc Applied Statistics, The Catholic University of Malawi (2024)**

A statistical forecasting study using time series modelling to project the future prevalence of non-communicable diseases (NCDs) at Queen Elizabeth Central Hospital (QECH), Malawi's largest referral hospital — with the goal of supporting evidence-based resource allocation and health system planning.

---

## 📌 Research Problem

Non-communicable diseases (cardiovascular disease, diabetes, hypertension, cancer) are rising rapidly in sub-Saharan Africa, yet health facilities often lack data-driven forecasts to guide staffing, bed capacity, and drug procurement decisions.

This project asked: **Can historical NCD admission data at QECH be used to accurately forecast future case loads, and what do those forecasts mean for hospital planning?**

---

## 📊 Data

- **Source:** Queen Elizabeth Central Hospital clinical records
- **Period:** 10 years of monthly NCD admission data
- **Diseases modelled:** Hypertension, Diabetes Mellitus, Cardiovascular Disease
- **Variables:** Monthly case counts, seasonal indicators, trend components

---

## 🔧 Methodology

| Step | Method |
|---|---|
| Stationarity testing | Augmented Dickey-Fuller (ADF) test |
| Decomposition | Classical time series decomposition (trend + seasonality + residual) |
| Model selection | Auto-ARIMA (minimising AIC/BIC) |
| Forecasting | ARIMA model — 24-month forecast horizon |
| Model evaluation | RMSE, MAE, MAPE |

---

## 📈 Key Results

- **Hypertension** showed the strongest upward trend, with forecast models projecting a **~18% increase** in monthly admissions over the next 24 months.
- **Diabetes** admissions followed a seasonal pattern, with peaks observed in the first quarter of each year — consistent with post-harvest dietary changes.
- **Cardiovascular disease** admissions showed the highest volatility, with ARIMA(1,1,1) selected as the best-fit model (MAPE: 8.3%).
- Models achieved satisfactory forecast accuracy overall — RMSE values within acceptable clinical planning margins for resource estimation.

---

## 💡 Planning Implications

1. QECH should plan for **increasing NCD bed demand** through 2026, particularly for hypertension management.
2. **Seasonal staffing adjustments** in Q1 are recommended to manage the diabetes admission peak.
3. The forecasting framework developed here is **replicable** for other disease categories and other district hospitals using the same data structure.

---

## 📁 Repository Structure

```
forecasting_ncds_qech_mw/
├── thesis_document.tex          # LaTeX source of full thesis
└── README.md                    # This file
```

> **Note:** Analysis was conducted in R. The modelling scripts will be uploaded shortly.

---

## 🛠️ Tools Used

- **R** — Time series modelling (forecast package, tseries, ggplot2)
- **LaTeX** — Academic thesis write-up
- **Statistical methods** — ARIMA, ADF test, decomposition, RMSE/MAE evaluation

---

*Thesis by [Alex Maseko](https://github.com/alex166-cmd) — supervised by Mr. Harold Chimutu Banda, Head of Mathematical Sciences, The Catholic University of Malawi*

