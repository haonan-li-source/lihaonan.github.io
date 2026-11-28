---
layout: default
title: SafeTrace Asset Security Platform
---

[← Portfolio](../../)

# SafeTrace Asset Security Decision Support

<div class="project-meta"><strong>Role:</strong> Technical lead in a five-person team &nbsp; · &nbsp; <strong>Recognition:</strong> Provincial outstanding entrepreneurship project and RMB 15,000 university grant</div>

<div class="project-actions"><a class="button" href="https://github.com/haonan-li-source/safetrace-asset-security-platform">View repository and prototype</a></div>

## Problem

Asset-tracking products often stop at showing a location. SafeTrace explores the next decision layer: how asset type, route, geofence status, device health, time context, and emergency events can be organized into an understandable risk explanation and response prompt.

## Prototype design

- Three interactive scenarios for an electric bicycle, transport/luggage, and a high-value asset.
- Route replay, electronic-geofence events, and SOS triggers.
- Device-status monitoring for battery, connectivity, and signal state.
- Structured event logs and scenario switching.
- Scenario-based low, medium-low, and medium risk levels with reasons and recommended actions.
- Privacy and authorization reminders alongside location-based functions.

## My contribution

I led the technical work and contributed across product planning, prototype architecture, scenario design, rule logic, feasibility analysis, validation, and final materials. I developed and maintained the JavaScript prototype, including webpage interaction, route replay, geofence and SOS events, device-status views, structured logs, and explainable response prompts. Schedule and financial coordination were shared within the team, with another teammate taking primary responsibility for those areas.

## Result and validation boundary

Three simulated scenarios verified that the prototype could carry an event from sensing through risk explanation to a recommended response. This demonstrates a complete decision-support workflow rather than a location-only mock-up. It does not establish real-world detection accuracy, hardware reliability, loss reduction, or user adoption because no live assets or customers were used.

## Challenge and solution

An early tracker concept did not clearly show decision value. I reorganized the prototype around a complete sense–assess–respond flow. Simulated routes and events make each step visible, while rule-based explanations show why the interface assigns a risk level and what the user should do next.

## View the prototype

Open the static `index.html` file in a modern browser. No build step or external service is required.

<div class="tag-list"><span>Asset Tracking</span><span>Risk Management</span><span>JavaScript</span><span>Geofencing</span><span>IoT Prototype</span></div>
