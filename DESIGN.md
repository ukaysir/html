# Korea Festival Cause Intelligence Dashboard Design System

## 1. Atmosphere & Identity
A public-interest intelligence dashboard for festival planning risk. It should feel like an investigation room: dense enough for analysts, clear enough for non-specialists. The signature is a cause trail: symptom cards flow into stakeholder relationships, contract traces, and evidence confidence.

## 2. Color
| Role | Token | Value | Usage |
|---|---|---|---|
| Surface primary | --surface-primary | #1f1633 | Page background |
| Surface deep | --surface-deep | #150f23 | Deep panels |
| Surface card | --surface-card | #271d3f | Cards and evidence panels |
| Border | --border | #3b2b5f | Structural dividers |
| Text primary | --text-primary | #ffffff | Main Korean text |
| Text secondary | --text-secondary | #d8d3e5 | Supporting text |
| Text muted | --text-muted | #a99fbd | Metadata |
| Accent | --accent | #c2ef4e | Primary highlights and pass states |
| Warning | --warning | #ffb287 | Caution and partial evidence |
| Danger | --danger | #ff6b8f | Failure/risk signals |
| Info | --info | #8ea7ff | Source links and neutral info |

## 3. Typography
Primary: Pretendard, Noto Sans KR, Segoe UI, sans-serif. Mono: Consolas, Monaco, Menlo, monospace. Display uses the same Korean-safe sans stack with tighter tracking. Body text minimum is 14px.

## 4. Spacing & Layout
Base unit is 4px. Content max width is 1280px. Mobile uses a single column, tablet two columns, desktop mixed grid. Dense data must be progressively disclosed: summary first, evidence second, raw source last.

## 5. Components
### RiskCard
Structure: label, score/severity, short explanation, evidence count. States: default, hover, focus.

### CauseTrail
Structure: symptom -> likely cause -> stakeholder -> evidence. Variants: failure, success, insufficient-data.

### EvidenceBadge
Structure: confidence grade A/B/C/D with tooltip text. Must never rely on color only.

### RelationPanel
Structure: 발주기관 -> 주관기관 -> 총괄대행사 -> 공개 하청/부스 traces -> 미확인 gaps.

### SourceDrawer
Structure: source title, URL, source type, access note, extraction method, caveat.

## 6. Motion & Interaction
Use only opacity and transform. Motion is limited to section reveal and hover affordance. Respect prefers-reduced-motion.

## 7. Depth & Surface
Mixed strategy: purple tonal shifts plus subtle borders. No pure black and no generic purple-blue AI gradient.
