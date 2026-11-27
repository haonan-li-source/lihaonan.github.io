---
layout: default
title: Financial News Sentiment and the S&P 500
---

[← Portfolio](../../)

# Does Financial News Sentiment Move the S&P 500?

<div class="project-meta"><strong>Role:</strong> Evaluation lead in a five-person capstone &nbsp; · &nbsp; <strong>Period:</strong> 2008–2024 &nbsp; · &nbsp; <strong>Focus:</strong> time-aware validation</div>

<div class="project-actions"><a class="button" href="https://github.com/haonan-li-source/sp500-news-sentiment">View repository and report</a></div>

## Research question

The project tested whether daily financial-news sentiment adds useful information for next-day S&P 500 direction, returns, and simple trading performance. The evaluation focused on whether a text signal survived chronological testing, threshold changes, transaction costs, and different market regimes.

## My contribution

As evaluation lead, I connected classification metrics with economic backtests, ran probability-threshold scans, compared performance across market regimes, assessed robustness to transaction assumptions, and framed the final conclusion around stability rather than the best isolated result.

## Methods

- Started with 19,127 headline records; removed 974 exact duplicates to obtain 18,153 cleaned headlines and 3,506 daily observations.
- Compared dictionary sentiment, VADER, FinBERT, and LDA topics.
- Evaluated logistic regression and XGBoost for next-day direction and continuous models for next-day returns.
- Used training data before 2020, validation in 2020–2021, and testing from 2022 through March 2024.
- Added long/flat backtests, one-basis-point costs, threshold sensitivity, and regime analysis.

## Key results

- Next-day positive-return share: 54.3%.
- Best test balanced accuracy: 51.4%, from XGBoost with VADER features, still close to a chance-level benchmark.
- A FinBERT-logistic strategy returned 13.12% in the test period versus 6.97% for buy-and-hold, but the advantage was sensitive to thresholds and market regime.
- Best return-model RMSE was approximately 0.01193 versus 0.01197 for a historical-mean benchmark.

## Challenge and solution

News volume and source mix changed substantially over time, and a single favorable backtest could overstate predictive value. I used chronological splits, market-regime breakdowns, threshold scans, transaction-cost sensitivity, and a continuous-return benchmark. The resulting conclusion is deliberately measured: some sentiment features show signal in selected tests, but the advantage is not stable enough to support a general trading claim.

## Outputs

Six-page report, interactive static website, ROC and sentiment-comparison figures, regime-level returns, robustness checks, and return-model predictions.

<div class="tag-list"><span>Financial NLP</span><span>Sentiment Analysis</span><span>XGBoost</span><span>Backtesting</span><span>Time-aware Validation</span></div>
