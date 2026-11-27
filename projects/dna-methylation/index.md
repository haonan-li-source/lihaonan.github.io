---
layout: default
title: DNA Methylation Bayesian Structure Learning
---

[← Portfolio](../../)

# DNA Methylation Bayesian Structure Learning

<div class="project-meta"><strong>Role:</strong> Main researcher &nbsp; · &nbsp; <strong>Scale:</strong> 121 ENCODE datasets &nbsp; · &nbsp; <strong>Focus:</strong> local structure learning</div>

## Research question

DNA methylation measurements can be represented as local triplets of binary CpG states. I investigated whether a Bayesian-network structure inferred from one triplet remains coherent when the genomic window moves by one CpG site. The analysis separates local statistical compatibility from stronger claims about biological causation.

## My contribution

Under the supervision of Prof. Pearson Antony, I designed and implemented the complete workflow: data processing, quality control, exhaustive DAG scoring, adjacent-window comparison, methylation-state transition analysis, diagnostics, and visualization. I also developed an eight-state symbolic representation connecting category-level Markov dynamics with triplet joint distributions.

## Methods

- Built a vectorized NumPy and pandas pipeline for 121 ENCODE methylation datasets.
- Applied variability and identifiability checks to binary CpG triplets.
- Exhaustively scored all 25 three-node DAGs with BIC, AIC, and BDeu.
- Grouped structures by statistical equivalence and compared adjacent overlapping triplets.
- Reported both pair-weighted agreement and equal-weight dataset averages.
- Estimated empirical local transitions and an eight-state Markov representation.

## Key results

- Processed 650,152 input triplets and retained 634,824 after quality control (97.64%).
- Evaluated approximately 15.87 million triplet–structure combinations.
- Compared 461,271 overlapping-triplet pairs.
- Pair-weighted agreement reached 89.35% for BDeu, 87.65% for BIC, and 85.26% for AIC.
- The equal-weight dataset mean for BDeu was 87.60%.
- Estimated local persistence included P(1→1) = 0.8369, P(0→0) = 0.3858, and stationary methylated-state probability π1 = 0.7902.

## Challenge and solution

Similar-looking summaries answered different questions. Pair weighting emphasizes datasets with more comparable windows, while the dataset mean gives every dataset equal influence. I reported both and kept the spatial-window analysis separate from the symbolic within-triplet Markov model, preventing local dependence measures from being interpreted as genome-wide causal dynamics.

## Outputs

Reviewed Python scripts, aggregate tables, compatibility distributions, ranked-dataset figures, methylation-class summaries, transition analyses, and input-schema documentation.

<div class="tag-list"><span>Bayesian Networks</span><span>DNA Methylation</span><span>Structure Learning</span><span>Markov Chains</span><span>Python</span></div>
