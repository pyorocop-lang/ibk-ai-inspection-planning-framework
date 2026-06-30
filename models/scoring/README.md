# 스코어링 모델 (Scoring Model)

> **공통 원칙:** AI는 검사부문을 결정하지 않고 **근거와 함께 추천**만 하며, 최종 결정은 **검사협의회(Inspection Committee)** 가 수행한다.

## 1. Purpose (목적)
차원별 점수와 가중치 정의를 버전관리한다.

## 2. Scope (범위)
차원 정의, 가중치, 산식.

## 3. Input (입력)
측정값, 가중치 설정.

## 4. Process (처리)
`AI_SCORING_ENGINE.md` 산식을 구현하고 가중치 변경을 사유와 함께 기록한다.

## 5. Output (출력)
후보별 점수와 분해표.

## 6. Explainability Requirement (설명가능성 요건)
산출물은 근거·신뢰도·반론을 포함하여 사람이 이해·검증·재현할 수 있어야 한다. 모든 핵심 주장에는 출처를 표기한다.

## 7. Human Review (사람의 검증)
산출물은 1차 검토자의 근거·편향 점검을 거치며, 최종 결정은 검사협의회가 수행한다.

## 8. Example (예시)
가중치 세트 v0.1 (Likelihood 0.25 …).

## 9. File Owner (문서 소유자)
검사기획 AI 운영 담당 (Inspection Planning AI Steward)

## 10. Version History (변경 이력)
| 버전 | 일자 | 변경 내용 | 작성 |
|------|------|-----------|------|
| v0.1 | 2026-06-30 | 초안 작성 | AI Steward |
