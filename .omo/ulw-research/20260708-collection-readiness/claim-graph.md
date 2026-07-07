# Claim graph: collection-readiness wave

## verified-claims

| claim_id | statement | risk | status | observations | source backing |
|---|---|---|---|---|---|
| CL-001 | The dashboard needs a normalized festival-year key before broad source joins can be trusted. | high | supported | INT-001, OBS-001, OBS-002, OBS-006 | Current repo state plus public source structures. |
| CL-002 | Procurement and booth records must be relationship evidence, not direct outcome-causality evidence. | high | supported | INT-002, OBS-006 | Existing relation schema and procurement evidence. |
| CL-003 | 2016 remains a nationwide master-data gap under currently identified public sources. | high | supported | INT-003, OBS-001 | MCST annual page exposes 2017-2026; separate 2016 selected-festival report remains narrower. |

## unresolved

| claim_id | statement | reason |
|---|---|---|
| CL-U001 | Every MCST annual download is machine-downloadable without manual browser steps. | Not verified in this wave; only page availability and public metadata were checked. |
