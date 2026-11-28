---
layout: default
title: Chinese Institute for Brain Research Internship
---

[← Internships](../) · [← Portfolio](../../../)

# Research Internship at the Chinese Institute for Brain Research, Beijing

<div class="project-meta"><strong>Role:</strong> Research intern &nbsp; · &nbsp; <strong>Period:</strong> Aug–Oct 2026 &nbsp; · &nbsp; <strong>Focus:</strong> multimodal single-neuron analysis</div>

<div class="project-actions"><a class="button" href="../">Browse all internship case studies</a></div>

## Research context

The study examined whether the molecular identity of individual neurons is associated with their functional responses to stimuli. The workflow linked measurements from the same neurons across in vivo GCaMP imaging, ex vivo and post-expansion three-dimensional microscopy, and EASI-FISH gene-expression measurements.

## My contribution

- Supported mouse experiments and tissue processing, including animal-status monitoring, stimulus delivery, GCaMP acquisition, perfusion, tissue collection, and brain sectioning.
- Reviewed multichannel z-stacks in Napari and Fiji.
- Checked model-labeled fluorescent spots, removed false positives, and added missed signals.
- Produced traceable overlays, local comparison views, and coordinate records for signal-level quality control.
- Organized ROI-gene measurements into a binary matrix, standardized marker names, and handled duplicate or missing records.
- Explored expression structure with PCA, Jaccard distance, and k-medoids clustering.
- Used bootstrap-adjusted Rand index and permutation tests to examine cluster stability and sample effects.

## Scale and outputs

After manual review and correction, spot identification agreed with visually verified fluorescence signals at approximately 90%–95%. The work produced corrected annotations, coordinate tables, comparison overlays, a standardized ROI-gene matrix, and an exploratory clustering workflow.

## Research value and boundary

The immediate result was a more reliable, traceable bridge between image-level signals and downstream cell-by-gene analysis. The clustering work was exploratory: bootstrap stability and permutation checks were used to distinguish repeatable expression patterns from sample-specific structure. Raw images, coordinate records, animal data, and unpublished biological findings remain non-public because release requires laboratory approval.

## Challenge and solution

Noisy signals across imaging channels and biological samples could distort downstream expression patterns. I combined signal-level review, local overlay comparison, marker-name standardization, and stability analysis so that corrections remained traceable and apparent clusters could be checked against sample-specific effects.

<div class="tag-list"><span>Neuroscience</span><span>Bioimage Informatics</span><span>Multimodal Data</span><span>Clustering</span><span>Quality Control</span></div>
