---
layout: default
title: Sleep, Stress, and Health
---

[← Portfolio](../../)

# Nonparametric Analysis of Sleep, Stress, and Lifestyle

<div class="project-meta"><strong>Format:</strong> Team course project &nbsp; · &nbsp; <strong>Sample:</strong> 374 records &nbsp; · &nbsp; <strong>Focus:</strong> distribution-free inference</div>

<div class="project-actions"><a class="button" href="https://github.com/haonan-li-source/nonparametric-sleep-health">View code, report, and slides</a></div>

## Research question

The project examines relationships among sleep duration, sleep disorders, stress, physical activity, and lifestyle measures. Because stress is ordinal, several variables contain many ties, and distributions depart from normality, the analysis uses rank-based and distribution-free methods.

## Methods

- Exact two-sided sign test for a median hypothesis.
- Mann-Whitney comparison with a Hodges-Lehmann location-shift estimate.
- Kruskal-Wallis test followed by Dunn comparisons with Holm adjustment.
- Spearman rank correlations and Fisher exact testing.
- Kernel density estimation and Nadaraya-Watson smoothing.
- Midranks and tie corrections for repeated ordinal values.

## Key results

- 374 complete records: 219 without a sleep disorder, 77 with insomnia, and 78 with sleep apnea.
- Median sleep duration was 7.2 hours; sign-test p = 0.0011.
- Stress comparison between disorder and no-disorder groups: p = 0.0025, with a Hodges-Lehmann shift of +1 stress point.
- Sleep-duration differences across three groups: Kruskal-Wallis H = 248.39, p < 0.001.
- High stress and sleep disorder: Fisher odds ratio = 6.01, p < 0.001.
- Sleep duration and stress: Spearman ρ = -0.811.

## Challenge and solution

Discrete scales and tied observations made ordinary normal-theory comparisons inappropriate. The team matched each question to a rank or exact method, applied tie corrections and multiplicity adjustment, and interpreted effect direction and group medians alongside p-values.

## Deliverables and reproduction

The project includes a 17-page report, an 11-page presentation, Python analysis, JSON/CSV results, and generated figures.

```bash
python -X utf8 analysis.py
```

<div class="tag-list"><span>Nonparametric Statistics</span><span>Health Data</span><span>Python</span><span>Rank Tests</span><span>Reproducible Research</span></div>
