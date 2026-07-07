# intent-diff

| intent_id | expected truth | observed reality | diff | violated invariant | intent source | supporting observations | status | linked claims |
|---|---|---|---|---|---|---|---|
| I-WONJU-01 | 성공/실패 이유가 방문객 수보다 우선이어야 한다 | 원주는 성공 수치와 주차·날씨·집계 리스크가 공존한다 | 단순 성공 라벨 금지 | cause-first | user goal | O-WONJU-01..O-WONJU-08 | true | C-WONJU-01,C-WONJU-02 |
| I-WONJU-02 | 대행사/하청 관계를 확인하되 무리한 귀속은 금지해야 한다 | 2025 무대시스템 용역과 낙찰자는 확인되나 실패귀속 증거는 부족하다 | 계약-성과 연결 공백 | attribution guardrail | user goal | O-WONJU-09,O-WONJU-10 | true | C-WONJU-04 |
