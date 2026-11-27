---
layout: default
title: U.S. Inflation and Monetary Policy
---

[← Portfolio](../../)

# U.S. Inflation and Macroeconomic Factors

<div class="project-meta"><strong>Role:</strong> Independent course project &nbsp; · &nbsp; <strong>Sample:</strong> 298 monthly observations &nbsp; · &nbsp; <strong>Source:</strong> FRED</div>

## Research question

This study examines how U.S. inflation co-moves with monetary, labor-market, energy-price, and real-activity indicators from 2000 through May 2026. The design emphasizes inflation persistence, post-pandemic shifts, time-series diagnostics, and robustness rather than treating conditional associations as causal effects.

## Methods

- Constructed year-over-year transformations for CPI, core CPI, M2, WTI, and industrial production.
- Compared AR(1) through AR(6) specifications on the same sample and selected AR(3) using AIC, BIC, and residual behavior.
- Estimated OLS with calendar-aware Newey-West HAC standard errors using 12 lags.
- Ran ADF, VIF, Durbin-Watson, Ljung-Box, Breusch-Pagan, and White diagnostics.
- Tested alternative inflation measures, post-2008 and adjusted samples, alternative lag orders, HAC bandwidths, and an inflation-change specification.

## Key results

- Final sample: 298 valid monthly observations from April 2001 to May 2026.
- Baseline adjusted R²: 0.953; Durbin-Watson: approximately 1.921.
- Sum of three lagged-inflation coefficients: approximately 0.871, indicating strong persistence.
- Lagged WTI year-over-year growth coefficient: approximately 0.005 with HAC standard error near 0.001.
- Post-pandemic indicator coefficient: approximately 0.238.
- Deliverables include a 16-page paper, two core Python scripts, a one-command runner, and nine traceable result tables.

## Challenge and solution

Year-over-year transformations, dynamic lags, and a missing October 2025 observation created a non-continuous monthly sequence. I matched residual lags by actual calendar month rather than treating observations on either side of the gap as adjacent, then added residual diagnostics and multiple robustness specifications.

## Reproduce the analysis

```bash
python -m pip install -r requirements.txt
python run_all.py
```

<div class="tag-list"><span>Time Series</span><span>Econometrics</span><span>FRED</span><span>Macroeconomics</span><span>Python</span></div>
