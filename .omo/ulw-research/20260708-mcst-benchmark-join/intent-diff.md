# Intent diff: MCST benchmark join

| intent_id | expected truth | observed reality | status | supporting observations | claim ids |
| --- | --- | --- | --- | --- | --- |
| I-BENCH-001 | Official 2026-2027 cultural-tourism festival cohort should be extracted from a primary source. | HWPX attachment from MCST press page was downloaded through public UplDownloadFile params and text was extracted from section0.xml. | true | O-BENCH-001 | C-BENCH-001 |
| I-BENCH-002 | The official cohort should be usable as a benchmark against the 2017-2026 MCST master. | 27 names were normalized and joined to 2026 MCST master rows; exact/fuzzy/unmatched counts recorded. | true | O-BENCH-002 | C-BENCH-002 |
| I-BENCH-003 | Selection status must not be treated as standalone proof of success. | HTML and JSON include explicit interpretation guardrail. | true | O-BENCH-003 | C-BENCH-003 |
