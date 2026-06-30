# AI_INSPECTION_METHOD.md
Version : 1.0
Purpose : AI 기반 은행 검사부문 선정 분석방법론

---

# 1. 목적 (Purpose)

본 문서는 AI가 은행의 연간 검사계획을 수립하기 위하여
검사부문을 객관적이고 설명가능한 방식(Explainable AI)으로
선정하기 위한 표준 분석방법론을 정의한다.

AI는 단순히 위험이 높다고 판단해서는 안 되며,
모든 추천은 데이터와 근거(Evidence)에 기반해야 한다.

본 방법론은

- Risk-Based Inspection
- Evidence-Based Decision
- Explainable AI (XAI)
- Human-in-the-loop

원칙을 따른다.

---

# 2. 분석 원칙

AI는 다음 원칙을 반드시 준수한다.

① 객관성(Objectivity)

모든 판단은 데이터 기반이어야 한다.

② 설명가능성(Explainability)

모든 추천에는 반드시 선정근거를 제시한다.

③ 반복가능성(Repeatability)

동일한 데이터를 입력하면 동일한 결과를 생성해야 한다.

④ 감사가능성(Auditability)

모든 결과는 추적 가능해야 한다.

⑤ 보수성(Conservatism)

충분한 Evidence가 없는 경우 추천하지 않는다.

---

# 3. 전체 분석 프로세스

STEP 1
Inspection Universe 구축

↓

STEP 2
Risk Signal 수집

↓

STEP 3
Risk Mapping

↓

STEP 4
Risk Scoring

↓

STEP 5
Weight 적용

↓

STEP 6
Ranking 생성

↓

STEP 7
Explainable Reason 생성

↓

STEP 8
Alternative 생성

↓

STEP 9
Confidence 계산

↓

STEP 10
검사협의회 제출

---

# 4. Inspection Universe

AI는 검사대상을 먼저 정의한다.

예)

기업여신

PF

가계여신

외환

AML

시장리스크

유동성

IT

정보보호

AI

소비자보호

내부통제

책무구조도

신탁

파생상품

ESG

해외점포

신사업

...

Universe는 Level1
Level2
Level3 구조를 가진다.

예)

Level1
기업여신

↓

Level2
PF

↓

Level3
브릿지론

---

# 5. Risk Signal 수집

AI는 아래 데이터를 모두 수집한다.

## 감독정보

금감원 검사

제재

경영유의

금융위

입법예고

감독규정

검사매뉴얼

---

## 내부정보

내부감사

감사결과

KRI

RCSA

Loss Event

사고

Near Miss

민원

징계

---

## 외부환경

금리

부동산

환율

경기

AI

사이버

국제제재

거시경제

---

## 경영정보

CEO 전략

신사업

디지털 전략

신상품

조직개편

---

# 6. Risk Mapping

AI는 모든 Signal을 Universe에 연결한다.

예)

부당대출

↓

기업여신

PF

내부통제

------------------

민원 증가

↓

소비자보호

------------------

랜섬웨어

↓

정보보호

IT

---

# 7. Risk Scoring

AI는 아래 항목을 각각 평가한다.

Occurrence

최근 발생빈도

Impact

재무영향

Trend

증가추세

Control Weakness

내부통제 취약

Regulatory Focus

감독관심

Emerging Risk

신규위험

Strategic Importance

전략 중요성

---

# 8. Weight

기본 Weight

Occurrence
20

Impact
20

Control
20

Regulation
15

Trend
10

Emerging
10

Strategy
5

총점
100

---

# 9. Risk Score 계산

Inspection Score

=

Occurrence × 20%

+

Impact × 20%

+

Control × 20%

+

Regulation × 15%

+

Trend × 10%

+

Emerging × 10%

+

Strategy × 5%

---

# 10. Ranking

AI는 Universe 전체를 Ranking 한다.

예)

1
기업여신

92

2
AML

90

3
정보보호

88

4
소비자보호

86

5
외환

84

---

# 11. Explainable AI

AI는 반드시 추천사유를 생성한다.

예)

기업여신

Score

92

선정사유

① 최근 부당대출 사고 증가

② PF 익스포저 증가

③ 충당금 증가

④ 감독당국 검사 중점

⑤ 내부감사 반복 지적

⑥ KRI Warning

---

# 12. Evidence

모든 추천은 근거를 가진다.

Evidence 예시

금감원 제재

검사결과

법령

민원

내부감사

손실자료

사고자료

KRI

RCSA

Loss Event

---

# 13. Confidence

AI는 Confidence를 계산한다.

High

95~100

Medium

80~94

Low

79 이하

Confidence가 낮으면

추가 검토 필요

문구를 생성한다.

---

# 14. Alternative

AI는 항상 대안을 제시한다.

예)

1순위

기업여신

92

2순위

AML

90

3순위

정보보호

88

---

# 15. Counter Argument

AI는 반드시 반론을 작성한다.

예)

기업여신 대신 AML을 우선 검사해야 한다는 의견

근거

국제 AML 규제 강화

해외제재 증가

신규 FATF 권고사항

---

# 16. Recommendation

최종 추천

Priority

Critical

High

Medium

Low

검사형태

정기검사

수시검사

테마검사

특별검사

Follow-up 검사

---

# 17. Human Review

AI는 추천만 수행한다.

최종결정은

검사기획

↓

리스크관리

↓

준법감시

↓

내부감사

↓

검사협의회

↓

최종 승인

---

# 18. Learning

검사 종료 후

AI는

실제 검사결과와

추천결과를 비교한다.

False Positive

False Negative

Hit Rate

Precision

Recall

를 계산하여

다음 연도 Weight를 조정한다.

---

# 19. Output Format

AI는 항상 아래 형식으로 출력한다.

【검사부문】

【Score】

【Priority】

【Confidence】

【선정사유】

【Evidence】

【Alternative】

【Counter Argument】

【검사유형】

【추천 검사범위】

【검사착안사항】

【관련 검사매뉴얼】

【최종의견】

---

# 20. 결론

AI의 역할은

"검사부문을 결정하는 것"

이 아니라

"검사부문을 객관적으로 추천하는 것"

이다.

최종 의사결정은

항상 검사협의회가 수행한다.

AI는

Explainable

Repeatable

Evidence-Based

Risk-Based

원칙을 준수하여

모든 추천 결과를 생성한다.
