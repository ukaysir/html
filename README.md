# Korean Festival Cause Dashboard

Public-source-only research dashboard for tracing why Korean festivals succeed or fail.

Open `index.html` to view the dashboard.

## Scope
- 2016-2026 Korean festivals.
- Demand forecast, visitor performance, budget, contracts, agencies, public subcontract/booth traces and operational risk evidence.
- Agent-only public-source workflow: no phone calls, emails, interviews, information disclosure requests, paid/login-only sources or access-control bypass.

## Current status
This repository is a pushed research checkpoint. It contains:
- A standalone HTML investigation dashboard.
- Source maps for festival master, tourism, finance, procurement, contract and case evidence.
- Claim/evidence graph files to prevent unsupported causal claims.
- Access-feasibility and scoring models for the next collection waves.

The dataset is not yet a complete national raw-data archive. The dashboard explicitly keeps coverage and access limitations visible.

## GitHub Pages
The repo is structurally ready for GitHub Pages because `index.html` is at the repository root.

Pages was checked as not enabled during the research run. To publish, use:
- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/(root)`
- Expected URL after activation: `https://ukaysir.github.io/html/`

## Key data files
- `data/festival-source-map.json`
- `data/festival-cases.json`
- `data/evidence-manifest.json`
- `data/claim-graph.json`
- `data/schema.json`
- `data/scoring-rubric.json`
- `data/relation-graph-schema.json`
- `data/access-feasibility.json`
- `data/festival-case-evidence-wave3.json`
- `data/procurement-evidence-wave3.json`
- `data/source-coverage-matrix.json`
- `data/cause-index.json`
