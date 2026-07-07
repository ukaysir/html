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

## Expansion wave 3 findings
- Daejeon Zero O'Clock Festival 2024 is a mixed-success case. Daejeon City's release claims more than 2 million visitors, no safety accident/trash/overpricing for two years, AI crowd monitoring, food-price controls and major economic effect, while also acknowledging full vehicle control and citizen inconvenience. This makes it useful for studying how a successful demand surge still creates access and traffic risk.
- Gunsan Time Travel Festival 2022 has a strong evaluation-report pattern. The report measures visitor satisfaction, identifies local-culture/program/safety strengths, and directly names food, souvenirs, accessibility and parking as the weakest areas.
- Hongcheon River Kkongkkong Festival 2024 remains a price/merchant-control risk case. Public reporting links the overpricing controversy to the host foundation's apology and to weak festival food-price disclosure infrastructure. Treat as B/C until direct foundation source material is attached.
- Case evidence now also tracks Hwacheon Sancheoneo 2026/2020, Jinhae Gunhangje 2023/2022, Boryeong Mud 2020/2024, Jinju Namgang Yudeung 2017, Gangneung Danoje 2024, Muju Firefly 2023, Jeju Fire Festival 2023, Inje Icefish 2024, Andong Maskdance 2023 and Itaewon Halloween 2022 as a crowd-risk comparator.
- Procurement evidence now tracks public roles for Yeoju Ogoknaru, Daedeok Waterlight, Daejeon Donggu Dongrak, Gaya Culture, Sunchang Jangryu, Muan Lotus, Boryeong Mud, Jinju Namgang Yudeung, Busan Rock and Jinhae Gunhangje. These records separate host, supervisor, procurement agent, lead contractor package, booth recruitment, selected vendor and cancellation/change evidence.
- Official coverage matrix: MCST annual regional-festival downloads are the strongest 2017-2026 master backbone. Public Data Portal standard data is a current/geocoding snapshot, not a historical panel. Korea Tourism DataLab is a culture-tourism-festival performance overlay, not a national census. Local Finance 365 is strong for large-event cost disclosure. NaraJangteo is a contract-matching layer, not canonical festival finance.
- 2016 remains a coverage gap: the current MCST nationwide annual regional-festival page exposes 2017-2026, while the official 2016 MCST evaluation source covers only 43 culture-tourism festivals.

## Claim discipline
Every claim in the final dashboard must carry a confidence grade. Hidden subcontracting or private coordination must not be asserted unless a public source names it.
