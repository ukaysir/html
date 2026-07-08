# Next work handoff

Updated: 2026-07-08.

## Current baseline
- Branch: `main`.
- Remote: `origin/main` at `https://github.com/ukaysir/html`.
- Last completed research commit before this handoff: `e2a316e data: add wonju dancing carnival dossier`.
- The repository was clean and synced before this handoff-document update.
- Current completed case count from the latest matrix summary: 39 festival-case records.
- Latest completed case: `원주댄싱카니발 2016-2026`.

## Active user requirements
- 조사 범위: 대한민국 축제 2016-2026, 가능한 최대 범위.
- 핵심 질문: 왜 성공했는가, 왜 실패했는가, 왜 만족도가 낮아졌는가, 왜 예산 낭비 리스크가 생겼는가.
- 관계 추적: 지자체, 재단, 축제 대행사, 용역, 하청/부스/상인, 경찰/소방/교통/안전 관계를 가능한 한 분리해서 본다.
- 최종 결론: 전체 축제를 종합해 성공 축제 공통점과 실패/리스크 축제 공통점을 축제별로 정리한다.
- HTML 디자인: Pretendard 고정, Toss 느낌의 미니멀하고 깔끔한 단일 디자인. 기준 파일은 `DESIGN.md`, 공통 CSS는 `assets/toss-report-theme.css`.
- 조사 방식: agent-only public-source workflow. 전화, 이메일, 인터뷰, 정보공개청구, 유료/로그인 전용 자료, 우회 접근은 사용하지 않는다.
- 운영 방식: 긴 작업 중 30분마다 commit and push. 토큰/컨텍스트 부족 전에는 반드시 commit and push.

## Next recommended case

### 영등포 여의도 봄꽃축제 2016-2026
Suggested slug: `yeouido-spring-flower-crowd-traffic-governance-dossier`.
Suggested case id: `yeouido-spring-flower-2016-2026`.

Why this case matters:
- 벚꽃 개화 시기와 날씨가 수요 예측을 흔든다.
- 국회 뒤 여의서로 1.7km 구간에 관광객이 좁게 몰린다.
- 차량 통제, 버스정류장 폐쇄/우회, 임시주차장 없음, 개인형 이동장치 제한이 만족도와 주민 불편을 동시에 만든다.
- COVID 기간에는 취소/폐쇄/제한 개방 후 재개라는 수요 복구 문제가 있었다.
- 구청, 문화재단, 경찰, 소방, 자율방범, 녹색어머니, 행사/홍보/체험/물품 용역 등 관계자가 많아 공공-민간 운영 경계를 보기 좋다.

Already found source leads:
- Official 2026 festival page: `https://www.ydp.go.kr/tour/contents.do?key=6107`
- 2024 Yonhap report on full-scale festival and safety system: `https://www.yna.co.kr/view/AKR20240325137300004`
- 2026 Maeil Business/Daum report on 100만+ visitors, 150 programs, CCTV, safety agents, traffic control, police/fire/foundation cooperation: `https://v.daum.net/v/20260405220604610?f=p`
- Open next: 2022 Yonhap reopening/limited access source `https://www.yna.co.kr/view/AKR20220322088700004`
- Open next: 2023 News1 reopening/crowd-control source `https://www.news1.kr/local/seoul/4974369`
- Open next: 2019 Newsis traffic-control source `https://www.newsis.com/view/NISX20190401_0000605509`
- Search next: 2020/2021 cancellation or road-closure official notices.
- Search next: `영등포문화재단 여의도 봄꽃축제 용역`, `여의도 봄꽃축제 수의계약`, `2026 영등포 여의도 봄꽃축제 체험 프로그램 운영 용역`.

Expected outputs for this case:
- `.omo/evidence/yeouido-spring-flower-crowd-traffic-governance-dossier.md`
- `.omo/ulw-research/<timestamp>-yeouido-spring-flower/`
- `data/yeouido-spring-flower-crowd-traffic-governance-dossier.json`
- `data/yeouido-spring-flower-crowd-traffic-governance-dossier.csv`
- `yeouido-spring-flower-crowd-traffic-governance-dossier.html`

Expected index updates:
- `data/case-evidence-matrix-wave2.json`
- `data/case-evidence-matrix-wave2.csv`
- `case-evidence-matrix-wave2.html`
- `data/why-cause-router-wave2.json`
- `data/why-cause-router-wave2.csv`
- `why-cause-router-wave2.html`
- `festival-common-patterns-synthesis.html`
- `index.html`
- `README.md`
- `RESEARCH_STATUS.md`

## Causal guardrails
- Procurement or event-agency evidence is context, not fault by itself.
- Only claim contractor/subcontractor causality when the chain includes scope, responsibility, incident/outcome, and public evaluation or dispute evidence.
- Separate public-host decisions, vendor/booth conduct, nearby-market conduct, and event-agency scope.
- Visitor count, economic effect and satisfaction must be treated as different metrics; do not infer one from another.
- Budget waste requires net cost, revenue or local-capture evidence, outcome evidence, and externalized inconvenience/cost evidence. High budget alone is not waste.

## Design guardrails
- Every top-level HTML page should link the shared stylesheet after local styles: `assets/toss-report-theme.css`.
- Use Pretendard for Korean text.
- Keep pages readable without JavaScript.
- Use the common structure: eyebrow, h1, lead, KPI/cards, cause sections, procurement/stakeholder table, timeline, source list.
- Do not introduce per-festival color themes or dark dashboard variants.

## Known debt
- `festival-common-patterns-synthesis.html` may contain a duplicate 원주댄싱카니발 row from the prior automated insertion. If editing that file, remove the duplicate in the same targeted commit.
- Full visual QA was intentionally deferred because validation was not requested.
- 2016 nationwide master-data coverage remains incomplete.
- Public Data Portal and NaraJangteo bulk automation may require service keys; keep current workflow public-source only unless the user explicitly changes scope.

## Commit workflow
Use the repository root `C:\Users\CKIRUser\Downloads\html`.

1. `rtk git status --short --branch`
2. Research and edit one coherent case batch.
3. Inspect full diff for the intended files.
4. Stage explicit paths only.
5. Commit with the existing style, for example `data: add yeouido spring flower dossier`.
6. `rtk git push`
7. Report commit hash and remaining worktree state.
