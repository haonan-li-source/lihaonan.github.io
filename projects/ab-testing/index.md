---
layout: default
title: Small-Sample A/B Testing System
---

[← Portfolio](../../)

# Small-Sample A/B Testing Allocation and Inference System

<div class="project-meta"><strong>Role:</strong> Project lead and first-named inventor &nbsp; · &nbsp; <strong>Status:</strong> Published Chinese invention patent application</div>

<div class="project-actions"><a class="button" href="https://github.com/haonan-li-source/small-sample-ab-testing-system">View GitHub repository</a></div>

## Problem

Adaptive allocation can direct more traffic toward promising variants, but the allocation process changes the observed sample and can complicate later treatment-effect interpretation. This project addresses the tension between learning efficiency and inferential credibility when experiment traffic is limited, effects are noisy, or a test begins without reliable historical observations.

## System design

- Divides traffic into a model-guided primary stream and an independent randomized validation stream.
- Uses the primary stream to allocate traffic toward stable, promising variants.
- Maintains parallel treatment-control estimates from the randomized stream.
- Constructs confidence from effective sample size, historical effect variability, and early-trend stability.
- Applies conservative shrinkage before low-confidence effects influence allocation.
- Transfers priors from related historical experiments through a dynamic feature-association representation.

## My contribution

I led the project and contributed to the system architecture, allocation logic, confidence mechanism, historical-prior transfer design, and formalization of the invention for the patent application.

## Challenge and solution

A fully randomized design preserves comparability but may learn slowly, while a purely adaptive design can blur whether observed differences come from the strategy or the allocation process. The dual-stream architecture assigns these responsibilities separately: adaptive learning in the primary stream and cleaner effect validation in the randomized stream.

## Patent record

Chinese invention patent application `202511997982.0` lists Haonan Li as the first-named inventor and was published on April 3, 2026.

## Outputs

Published patent application, system architecture, process diagrams, allocation and validation workflow, and definitions of confidence, shrinkage, and prior transfer.

<div class="tag-list"><span>A/B Testing</span><span>Adaptive Experimentation</span><span>Statistical Inference</span><span>Cold Start</span><span>Patent</span></div>
