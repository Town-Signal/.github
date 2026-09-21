# 타운시그널 (TownSignal)

> 내 조건과 받을 수 있는 지원금으로, 어디서 창업하면 유리한지 거꾸로 찾아주는 서비스

영남대학교 'AI서비스프로젝트' 수업 팀 프로젝트입니다.

---

## 무엇을 만드나요?

서울 지역 청년 예비창업자가 나이·자격증·경력·자본금·희망 업종을 입력하면, 정부·서울시·자치구 청년 창업 지원사업 요건과 매칭해 **받을 수 있는 지원금을 계산**하고, 자본금과 합쳐 **실질 가용 예산**을 구합니다. 그 예산으로 감당 가능한 임대료의 행정동을 걸러낸 뒤, (행정동 × 업종) 조합별 **예상 매출과 생존 기간**을 예측해 순위로 보여줍니다.

핵심은 '조회'가 아니라 **'역산'** 입니다. 위치를 먼저 정하는 것이 아니라, 지원금을 예산으로 환산해 지역을 거꾸로 찾습니다.

## 왜 필요한가요?

- 예비창업자는 지원사업이 자신에게 얼마나 해당하는지, 받으면 최종 예산이 얼마가 되는지 스스로 계산하기 어렵습니다.
- 지원사업 검색과 상권분석이 서로 다른 서비스로 나뉘어 있어, 지원금을 확인한 뒤 지역을 다시 찾아야 하는 이중 작업이 필요합니다.
- 기존 상권분석 서비스는 창업 위치를 이미 정했다는 전제라, 어디서 시작할지 모르는 예비창업자와 맞지 않습니다.

## 차별성

| 서비스 | 방식 | 한계 |
|---|---|---|
| 소상공인365, 서울시 골목상권 분석 | 위치를 먼저 지정하고 현재 지표를 조회 | 예산 입력이 없고, 지원사업은 안내 수준 |
| K-Startup, 청년몽땅정보통 | 청년 창업 지원사업 정보 제공 | 상권분석과 분리되어 있음 |
| **타운시그널** | 인적 조건 → 지원금 → 가용 예산 → 지역 추천 | — |

1. 인적 조건만으로 시작해 지역을 **역으로 추천**합니다.
2. 지원금을 **예산으로 환산**합니다. 자치구마다 지원사업이 달라 가용 예산과 추천 순위도 달라집니다.
3. 추천 요약에도 예산·지원금 맥락을 반영합니다. (예: 매출이 낮아도 지원금 여력이 커 실질 부담이 가장 적은 지역)

## 핵심 기능

- **인적 조건 입력** — 나이, 자격증, 경력, 자본금, 희망 업종
- **지원사업 매칭 및 가용 예산 산출** — 자치구별로 각각 계산
- **행정동 필터링** — 가용 예산으로 감당 가능한 임대료 수준만 통과
- **매출·생존 기간 예측** — 신뢰구간과 함께 제공
- **상권 성장세 반영** — 지금은 평범하지만 성장 중인 지역을 더 높게 평가
- **추천 근거 설명** — 순위가 나온 이유를 항목별로 분해하고 요약 문장 제공
- **지역 직접 검색 · 현황 대시보드 · 후보지 비교**

> 예측 결과는 참고 정보이며, 최종 판단과 책임은 사용자에게 있습니다.

## 활용 데이터

| 구분 | 데이터 소스 |
|---|---|
| 상권·매출·유동인구 | 서울시 상권분석서비스 (서울 열린데이터광장) |
| 개업·폐업 | 서울시 상권분석서비스, 지방행정 인허가(LOCALDATA) |
| 임대료 | 서울시 부동산 전월세가 정보 |
| 지원사업 | 창업진흥원 K-Startup, 서울시·자치구 청년창업 지원사업 공고 |

## 저장소

- [TownSignalFE](https://github.com/Town-Signal/TownSignalFE) — 프론트엔드
- [TownSignalBE](https://github.com/Town-Signal/TownSignalBE) — 백엔드
- [TownSignalAI](https://github.com/Town-Signal/TownSignalAI) — AI 모델

## 팀원

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/gyumin123"><img src="https://github.com/gyumin123.png" width="100px;" alt="규민"/><br /><b>규민</b></a>
    </td>
    <td align="center">
      <a href="https://github.com/FAITRUEE"><img src="https://github.com/FAITRUEE.png" width="100px;" alt="성진"/><br /><b>성진</b></a>
    </td>
    <td align="center">
      <a href="https://github.com/HanSatCode"><img src="https://github.com/HanSatCode.png" width="100px;" alt="석희"/><br /><b>석희</b></a>
    </td>
    <td align="center">
      <a href="https://github.com/nohhyun03"><img src="https://github.com/nohhyun03.png" width="100px;" alt="현석"/><br /><b>현석</b></a>
    </td>
    <td align="center">
      <a href="https://github.com/RohSeungmin"><img src="https://github.com/RohSeungmin.png" width="100px;" alt="승민"/><br /><b>승민</b></a>
    </td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/gyumin123">@gyumin123</a></td>
    <td align="center"><a href="https://github.com/FAITRUEE">@FAITRUEE</a></td>
    <td align="center"><a href="https://github.com/HanSatCode">@HanSatCode</a></td>
    <td align="center"><a href="https://github.com/nohhyun03">@nohhyun03</a></td>
    <td align="center"><a href="https://github.com/RohSeungmin">@RohSeungmin</a></td>
  </tr>
  <tr>
    <td align="center">백엔드 · 팀장</td>
    <td align="center">CTO · AI</td>
    <td align="center">PM · 프론트엔드</td>
    <td align="center">백엔드</td>
    <td align="center">데이터</td>
  </tr>
</table>

---
