---
layout: default
title: Xiangchan AI Operations Platform
---

[← Portfolio](../../)

# Xiangchan AI Operations Platform

<div class="project-meta"><strong>Role:</strong> Project lead and full-stack developer &nbsp; · &nbsp; <strong>Recognition:</strong> Beijing Challenge Cup First Prize</div>

<div class="project-actions"><a class="button" href="https://github.com/haonan-li-source/xiangchan-ai-operations-platform">View code and documentation</a></div>

## Problem

Cooperatives, family farms, and rural businesses often lack a stable e-commerce operations team. Product facts are fragmented, promotional materials are inconsistent, and external AI services may fail or produce unsupported claims. Xiangchan turns product information into a reviewable operations package rather than a single untraceable text response.

## What I built

- A Node.js service and dependency-light browser interface.
- Structured product intake with assisted natural-language parsing.
- Optional DeepSeek and Tavily integration for semantic completion and public-reference retrieval.
- Field-level source, completeness, confidence, and human-confirmation records.
- Generation of product positioning, five selling points, product-page structure, short-video scripts, a seven-day calendar, operating SOPs, and risk prompts.
- Content checks for medical claims, government endorsement, guaranteed returns, and unsupported product facts.
- JSON, Markdown, and printable-page export.
- Local templates and rule-based fallback when external services are unavailable.

## Engineering and testing

The curated release contains 22 automated tests covering API configuration, intake parsing, generation, retries, offline fallback, risk handling, and source constraints. API keys remain outside version control; the full demonstration can run without them through the local workflow.

The project received First Prize in the “Qingzhi Future” special track of the “Qingchuang Beijing” 2026 “Challenge Cup” Capital University Student Entrepreneurship Plan Competition.

## Challenge and solution

External models may time out, return incomplete JSON, or generate risky wording. I combined retry and provider-switching logic with local fallbacks, secondary content cleaning, confidence indicators, and explicit human confirmation. This keeps the workflow usable while making uncertain fields visible before export.

## Run locally

```bash
npm install
npm test
npm start
```

Open `http://127.0.0.1:4173`.

<div class="tag-list"><span>AI Workflow</span><span>Node.js</span><span>Decision Support</span><span>Rural E-commerce</span><span>Human in the Loop</span></div>
