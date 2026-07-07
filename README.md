# Korean Festival Cause Dashboard

Public-source-only research dashboard for tracing why Korean festivals succeed or fail.

Open `index.html` to view the dashboard.

See `RESEARCH_STATUS.md` for checkpoint status, completed evidence layers and remaining gaps.

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
- `data/normalized-key-spec.json`
- `data/collection-backlog.json`
- `data/master-source-inventory.json`
- `data/mcst-download-manifest.json`
- `data/mcst-download-probe.json`
- `data/mcst-archive-schema-probe.json`
- `data/master/mcst-region-festivals-2017-2026.master-draft.json`
- `data/master/mcst-region-festivals-2017-2026.master-draft.csv`
- `data/master/mcst-region-festivals-2017-2026.summary.json`
- `data/master/mcst-region-festivals-2017-2026.summary-expanded.json`
- `data/master/mcst-region-festivals-2017-2026.lite-index.json`
- `data/master/mcst-legacy-period-overlays-2017-2021.json`
- `data/master/mcst-legacy-period-overlays-2017-2021.csv`
- `data/master/mcst-legacy-period-overlays-2017-2021.summary.json`
## Latest matching artifacts

- data/master/mcst-finance-procurement-match-keys.json: 10,198 MCST festival rows converted into finance/procurement search and join keys.
- data/master/mcst-finance-procurement-match-keys.csv: spreadsheet-friendly version for filtering by year, local government, budget band, and join priority.
- data/master/mcst-finance-procurement-match-keys.summary.json: year-level readiness counts for the dashboard.


## MCST benchmark cohort

- data/mcst-cultural-tourism-benchmark-2026-2027.json: official 2026-2027 cultural-tourism festival cohort extracted from the MCST HWPX press attachment and joined to the 2026 MCST master.
- data/mcst-cultural-tourism-benchmark-2026-2027.csv: spreadsheet-friendly benchmark join table.
- mcst-cultural-tourism-benchmark-2026-2027.html: human-readable benchmark cohort page.

## Benchmark priority queue

- data/benchmark-risk-priority-queue.json: investigation priority queue for the 2026-2027 cultural-tourism benchmark cohort.
- enchmark-risk-priority-queue.html: human-readable page showing which benchmark festivals should be traced first for budget/procurement/crowding/satisfaction causes.

## Benchmark procurement queue

- data/benchmark-procurement-search-queue.json: procurement/agency search queue for P2 benchmark festivals.
- enchmark-procurement-search-queue.html: human-readable query plan and evidence-seed page for contractor/procurement tracing.

## Procurement source strength

- data/procurement-source-strength-wave1.json: source-strength classification for procurement/agency leads.
- procurement-source-strength-wave1.html: human-readable distinction between official originals, official event pages, mirrors, and publicity-only leads.

## Procurement original download probe

- data/procurement-original-download-probe-wave1.json: official attachment download and source-upgrade probe for P2 benchmark festivals.
- procurement-original-download-probe-wave1.html: human-readable map of official original, evaluation result, mirror-only, blocked, and event-only evidence.

## Governance causal chain

- data/festival-governance-causal-chain-wave1.json: separates causal candidates from procurement-only or outcome-only evidence.
- festival-governance-causal-chain-wave1.html: human-readable chain from incident/success outcome to organizer, contractor, or evaluation structure.
