## 복습
- target(목표, 관심사, 종속 변수)
- 판매량 * 가격 = 매출
- iterator
    - 1. row(필요한 데이터 추가로 한줄 추가 필요)
    - 2. 필요한 쿼리를 검 (조건에 따라 툴 사용법을 익혀야함, 엑셀에 대한 기본기 필요)
        - 좋은 결과에 대한 합리적 이유 필요.
        - 명문 필요.
    - 3. 복잡한 요소들을 일반화 선형 모델로 바꿀수록 직관적이 되어짐(피처엔지니어링 특정분야의 주요 항목)
        - 단 너무 쉽게 변수를 단순화 할경우 놓치는 요소들이 생길수 있음(주의가 필요함)
        - 이 이해과정을 설명하기도 어려움(변수 자체를 줄여 버렸기 때문에 남에게 이해하기 어려움)
    - 4. 전처리 계획 수립(전처리 용어 찾아보자)
        - excel 및 powerBI tool 사용은 익혀둘 필요가 있음
        - 이 분야로 갈거라면
    - 5. 필요한 경우에는 데이터 정렬에 있어서 노가도 필요.
        - 수식이나 정규화를 모르고 데이터가 적은 양일 경우에는 노가다가 빠름
        - 필드 바꾼후 데이터 새로고침 아이콘 클릭시 반영됨(파워비아이)
## 시각화용
    - 툴에 기능들이 많음
    - 의사 소통용 시각화

## 분석용
- 변수의 요인을 조절해서 두개의 시각화 요소를 비교해서 보기 쉬움
- 어제뿌린 전단지 개수와 판매량의 상관계수
    - 데이터 조작이 가능
    - 추쇄선 활용, 스케일(축적의 비율)등을 조작시
    - 시각적으로 특정한 경향성을 나는것처럼 시각화 할수 있으나 해서는 안된다.
- 데이터 분석시 목표가 없을 경우 기간이 끝나지 않는다.
- 변수는 함부로 버리지 말고 가설을 버려야 함
    - 어제의 전단지 뿌린양이 오늘 과의 상관 계수는 없을지라도 누적될 경우
    - 연관성이 나타날수도 있으므로 변수는 함부러 폐기해서는 안된다.

## Descriptive Type: 요약의 힘
- 평균만 볼 거야? 최빈값? 중앙값?
- 편차    1월    2월    3월    4월    5월   6월    7월    8월    9월    10월    11월    12월
- 철수    -4     -6     -8    -2     -5    -7     -9     -3    -5     -2      -6      -6         
- 영희    -2     +2     +4    +6     +7    +4     +1     +3    +6     +9      +6      -4
- 중앙값이 대한 표준 편차가 평균보다 좋음
- 도서관 분석이 이봉으로 나뉜 이유
    - 정보 요약의 트레이드 오프에 주의 많으면 복잡 간단하면 정보손실(노이즈)이 커짐

## 그래프 관계
- 선형성이 제일 쉬움
- 선형 결합 -> 선형대수
- 2차원 관계등 추가적으로 공부할 필요가 있음 
- 쌍곡선만 해도 사람들에게 포물선 하단에서 왜 변했는지 설명하기가 어려울듯
- 그냥 그래프를 그리는것과 저 그래프의 의미를 설명하는건 전혀 다른 문제
- 분포도가 난잡하게 고르게 각 분면에 고르게 분포 할수록 0에 수렴한다.
- 코쉬 수바르츠 부등식 (즉 숫자의 크기로 평가하는게 특정 비율 안에 분포도를 비교하면 된다. 즉 비율 비교, 스케일 척도 참고)
- 복잡한 2차 log 쌍곡선도 변화는 곡점을 기준으로 짤라서 간단한 식을 도출해서 판단해도 된다.
- 수식이나 지표를 만들거면 학문 연구를 해야한다.
- 실전에서는 모든 요인을 통제 제어 연구할 시간이 없다.
- 그렇다고 말도 안되게 발로 해서는 안된다.

## 모델링 예시
- 판매량 = x * bpm + y
- 존재하는 Data
- 해석: 직원들의 복지를 해치면서 bpm을 올려서 8개의 매출을 올릴것인가?
- 판매량 = X * replet + y * bpm + z * bpm + a
- 기준을 가지고 비교해야 한다.
    - 당뇨와 비만의 상관관계 파악을 하려면 독립 시뮬을 확인하고
    - 실제 데이터 수집된 결과를 비교한후
    - 독립 시뮬과 수집된 결과가 같을 수록 독립 요인이고
    - 그 반대의 경우는 비만과 당뇨과 관계가 있다.
- 수학에서 빼기는 우항을 기준으로 좌항이 얼마만큼 떨어져 있냐는 거리로 구술이 가능하다.
- 8.33 이라는 수치는 통계학자 입장에서 설명이 가능한 수치이다.(카이제곱 분포표)

## comparative Typw: T-test 부터 ANOVA 살짝
- 가설 검증을 사용한다.
    - 대부분의 귀무가설: 예) 보수적인 입장, 차이가 없다. 변화가 없다 등등
    - 대부분의 대립가설: 예) 우리가는 바라는 무언가 차이가 있다. 변화가 있다 등등

## open source api 활용해서 돈 벌기
- ms machine learning studio
- anacond navigator oragne
- knine 머신러닝 파이프라인 자동화 툴
- 먼저 쓰고 봐야 한다.(선점 효과)
- 행동 먼저 검증하는 방식이 보다 실용적이다.
- 엔지니어 자체는 안사라짐(설계자)
- 기술은 전파 속도는 빨라지고 진입장벽이 허물어지는 속도는 빠름
- 대파를 사는 유저는 콩나물을 산다.
- 콩나물을 띄워주는 행위 자체는 유저의 편의성을 올려준다.
- 빅데이터를 활용해서 앱의 특성과 유저의 동선을 활요한 ux 디자인 자체가 가능하다.
- 귀무 가설이 참이라고 했을때 이런 데이터가 관찰이 될 확률은 ?
    - 주사위가 공평하다는데 20번중 10번이나 6이 나올 확률은? 3번 6이 나올 확률은?
    - 5%의 확률은 확률일뿐 실제 발생하면 그것은 1이 되어진다. 때로는 5프로라는 작은 확률에도 도박을 할땐 해야 한다.
- 귀무가설과 대립가설중 표본수가 12개 이상일때는 유용하다. 그러나 가능하면 표본수가 커질수록 유용하다.
- 가장 중요한건 통계적인 디테일한 수치가 아니라 가치가 얼마나 제대로 된 통제된 요인에 의해서 정확한 실험이 되었는지가 중요하다.
- 난수를 통해 a b 배너를 무작위로 노출해 유저의 평가모델에 편견이 끼어서는 안된다.
- 실험의 환경 통제 및 유저 반응에 최대한 객관성을 유지할수 있도록 설계하고 표본이 많아야 하며 요일 변수등도 제어해야 한다.
- 예산이 허락하는 안에서 최대한 설계를 명확히 해서 의사 결정이 가능해야 한다. 현실을 무시해선 안된다.
- 나쁜것이 나와도 기존의 데이터를 활용해서 소거법의 대안으로 사용할수 있다. 문제 원인 파악 가능
- 귀무가설 정의 https://ko.wikipedia.org/wiki/%EC%9C%A0%EC%9D%98_%ED%99%95%EB%A5%A0
- 새로운 방식으로 잡아낸 노이즈 -> 신호로 변경 됨. 변화의 가능성을 의미한다. 그러나 현실에서 실제 설득은 잘 모르겠다.
- 확실히 보다더 세밀한 수치들을 다루고 현대 사회가 세밀해져 가고 있다. 통계 분산 표준 편차들을 통한 보정 수치의 차이들을 설명하려 든다.
- 0.5 13.5배나 이런 표현보다는 비율로 소통해라 50프로의 오차를 잡아 내었습니다. 화술의 모델이 적용된다.
- 임원진 설득 후 실무진들과 일을 도와가면서 비즈니스 도메인 모델을 파악한후 임원진을 재설득 해야 한다. 실사구시 모델
    - 의사결정 이 중요
    - 실무자에게 도움이 됨
    - 매출에 향상이 되어야 함
    - 연구 방법론들은 충격을 주고 실제 실무에 도움이 되는 모델을 만들줄 알아야 함 위의 3가지 사항을 만들수 있어야 함
    - 핵심은 일의 효율 내지는 생산성 아웃풋이 증대되어야 함
- 이탈자들 분기 판단
    - 다양한 요인이 많기 때문에
    - 특정한 날짜(14일)등을 정해서 기준으로 잡고 지표를 잡을 필요가 있음
    - 한 주기를 돌리고 계속해서 요인의 정형화된 범위를 찾아야 함
    - 장기적으로 쌓일수록 데이터를 분석할 요소가 많아지고 정교화 될 가능성이 높아짐
    - 즉 계속 정기적으로 연구 보고서를 올바른 방식으로 할수록 데이터 비교 분석 예측 모델의 정확도 및 활용은 증가 할수 밖에 없음
    - 정답을 찾기 보다는 점점 기업의 운영을 개선하는 학습 모델을 만들어 가는게 중요함.
    - 가설 o x -> o x - > o x -> .... 의 무한 반복 계속해서 o 비율 등으로 수치를 올려야 함
    - 끊임없는 향상과 생존에 대한 치열함 ㅠㅠ