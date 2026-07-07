# ULW Research Synthesis: Korean Festival Cause Dashboard

Access date: 2026-07-07.

## Executive summary
The research should not rely on general web search as the backbone. The strongest public-source workflow starts with official festival master data, then joins tourism-performance signals, local finance cost/accounting data, procurement and contract records, public vendor/attachment traces, and finally lower-confidence news/review/SNS risk signals.

The HTML report should be an investigation surface rather than a raw table. The reader must be able to start with a plain-language answer, then drill into symptoms, causes, stakeholders, contracts, evidence and source provenance.

## Verified source axes
- Festival master: MCST annual regional festival index is strongest for 2017-2026. 2016 is a gap and requires the narrower MCST culture-tourism-festival report plus local backfill.
- Performance: Korea Tourism Data Lab can provide visitor, day-average visitor, spending, demographic and SNS trend signals. Big-data counts are trend indicators, not exact totals.
- Finance: Local Finance 365 cost accounting, budget allocation and contract status are core sources for cost, revenue, net cost, contract method, vendor and amount.
- Procurement: Nara/G2B APIs and attachments can expose bid notices, RFP/task instructions, changes, cancellations and contract chains.
- Cases: Failure/success evidence clusters around crowding/access, pricing, weather/safety, budget efficiency, content differentiation and governance/evaluation.
- UI: A three-layer civic-investigation report shell is appropriate: narrative answer, evidence workspace, source/provenance drawers.

## Expansion wave 2 findings
- Access feasibility: public dataset metadata and file pages are usable immediately, but many OpenAPI endpoints require service-key application. These are recorded as public-docs-only until a key is available.
- G2B/Nara procurement: direct attachment links can expose RFPs and task instructions, but link expiry, guarded downloads and JavaScript flows mean every contract match must store the notice number, agency, date and attachment evidence.
- Local finance: cost-accounting, budget allocation and contract status should be treated as separate tables rather than one blended budget field.
- Scoring: causal conclusions should use source-grade weights, evidence confidence, trend caveats, counterevidence and contract-match confidence. Weak evidence can sort a lead but cannot produce a strong claim.
- Relation graph: public roles should be encoded as nodes and edges only when a source directly supports them. Hidden subcontracting, informal coordination and booth relationships remain `unknown`, `not_disclosed` or `not_observable` unless public documents name them.
- GitHub Pages: the repository root contains `index.html` and is ready for Pages, but Pages was not enabled when checked. The likely final URL after enabling is `https://ukaysir.github.io/html/`.

## Claim discipline
Every claim in the final dashboard must carry a confidence grade. Hidden subcontracting or private coordination must not be asserted unless a public source names it.
