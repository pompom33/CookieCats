# CookieCats AB테스트 데이터 분석
<img width="1280" alt="TT_Header_CookieCats_UW_Up-scaled" src="https://github.com/user-attachments/assets/1d924c6f-f715-4b3b-9985-bce326782f5a">


#### AB테스트 주제
이 AB 테스트는 모바일 퍼즐 게임 Cookie Cats의 유저가 게이트에 도달하는 시점을 30 레벨에서 40 레벨로 옮겼을 때, 유저들의 접속(retention)에 어떤 변화가 있는지를 추적한 데이터입니다.
데이터 셋 링크 : [Mobile Games A/B Testing - Cookie Cats](https://www.kaggle.com/datasets/mursideyarkin/mobile-games-ab-testing-cookie-cats)

#### 데이터 셋 구성
![image](https://github.com/user-attachments/assets/c7e241d6-dcf6-456c-89b9-415034f610e1)

* **Userid** : 유저의 고유한 ID값
* **version** : GATE30 또는 GATE40 (무작위 할당)
* **sum_gamerounds** : 유저가 플레이한 라운드 수
* **retention_1** : 앱 설치 후 1일 후 재접속 여부
* **retention_7** : 앱 설치 후 7일 후 재접속 여부

#### 분석 기법
플레이어들은 GATE30, GATE40 집단에 무작위로 할당되었으며, 각 집단 별 게임 접속율을 두 독립표본 t검정, 카이 제곱 검정(독립성 검정)으로 분석하였습니다.

#### 결과
30 라운드 이상 플레이한 유저들을 대상으로 데이터를 분석한 결과, 유저들의 접속과 게이트 레벨의 이동은 관련이 없다는 결론을 내릴 수 있었습니다.

#### 한 걸음 더
50% 이상의 플레이어들이 GATE를 경험하지도 않고 이탈하였습니다.  플레이어의 유지가 목표라면 이러한 초기이탈율 개선이 GATE 이동보다 우선적인 과제일 듯 보입니다.
