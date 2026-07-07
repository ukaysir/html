# Intent diff: collection-readiness wave

| intent_id | expected truth | observed reality | status | supporting observations | linked claim ids |
|---|---|---|---|---|---|
| INT-001 | Dashboard must support nationwide 2016-2026 festival research, not only isolated cases. | Current repo has source maps and case evidence, but still needs a normalized collection model. | violated | `RESEARCH_STATUS.md` current limitations | CL-001 |
| INT-002 | Data joins must not invent hidden contractor/subcontractor relationships. | Existing relation schema and procurement evidence separate public roles, but collection keys need explicit match/reject rules. | partial | `data/relation-graph-schema.json`, `data/procurement-evidence-wave3.json` | CL-002 |
| INT-003 | 2016 coverage gap must stay visible. | Current files state the 2016 nationwide master gap. | true | `data/source-coverage-matrix.json`, MCST page observation | CL-003 |
