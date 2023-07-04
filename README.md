# Multi-it

# 층간 소음 측정 및 관리 공유 커뮤니티 서비스

## 방향성

<img width="271" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/07ae58c2-4362-4aa3-aa00-f042cac0b219">

최근 증가하는 세종시의 층간 소음 민원에 대응하여 빅데이터, IOT, AI, 클라우드 융합 기술을 활용한 데이터 기반 관리 서비스를 개발하여 층간 소음 문제를 예방하고 해결한다.

<img width="231" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/bbf9203e-9ca2-4c64-ab94-4710f6afef5c">

2022년 접수된 층간소음 민원의 71%가 아이들 뛰거나 걷는 소리로 가장 많음

수도권(서울, 경기, 인천)과 비교했을 때 세종시는 유일하게 신혼부부수가 증가한 지역

<img width="257" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/94fd73dc-26d6-47ee-8107-22d76ba6edb0">

세종시의 아동기(5~14세) 인구 또한, 최근 10년간 꾸준히 증가

층간소음의 연평균증가율이 21%로 전국에서 세종시가 가장 높은 점과 신혼부부 유입, 아동기인구가 점점 증가한다는 점을 반영하여 앞으로 층간소음의 빈도수가 더 증가할 것으로 예상됨

따라서 해당 프로젝트는 IoT, AI 융복합 기술로 층간소음 감지 및 관리 시스템과 공유 커뮤니티를 구축하여 세종시 아파트 주민들간의 갈등을 사전에 예방하고자 함

### 프로젝트 개요

<img width="970" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/29ceb8ed-a179-4fc0-9e2b-4666d9634db3">

![image](https://github.com/bananaisgood/multi-it/assets/112065692/641365e4-8fca-4849-8b98-9c1b61f22e09)

![image](https://github.com/bananaisgood/multi-it/assets/112065692/0d0e8cf2-a4af-4cab-a499-6e4f3cb01c52)

![image](https://github.com/bananaisgood/multi-it/assets/112065692/5956e7aa-9aa7-4703-b408-b83752d65f00)

### 개발 일정

![image](https://github.com/bananaisgood/multi-it/assets/112065692/20f5afec-6720-476f-8c43-142da6e4936e)

### 수행절차 및 결과

### Cloud

AWS Architecture

<img width="708" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/3d2694b2-9126-4627-8de3-f5753da9f36a">

EKS Cluster

<img width="606" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/d8f422f0-7ce1-4d90-8469-0a29a962f2bc">

AWS Workflow

<img width="798" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/e0c9c3e5-e6fa-4460-b796-a122ff9ff670">

CI/CD

<img width="597" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/56d948e6-7a6b-4d11-b163-b0f65930a1c1">

### IOT

<img width="835" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/5dc355ea-38d8-446f-805e-86e4ee6960f5">

### AI모델

목적

소음 녹음파일 수집,이미지화 하여 구별
"층간 소음"에 해당하는 소음을 구분

<img width="727" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/3b81cd59-8168-4826-99ed-cb1990269c3a">

층간 소음과 집안 소음 판단

데이터 수집

- 위층 소음원(아래층에서 들리는 층간소음)

데이터 분석

- 층간소음은 magnitude(소리의 크기))가 작으며 frequency(주파수)가 작음을 확인
- 소리를 이미지로 변환하는 멜 스펙트로그램에서도 고주파수의 차이를 확인 가능
- 이를 활용해서 AI모델 생성

<img width="422" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/fad77c97-a95a-4a3c-928e-a7221d08aa6e">

<img width="317" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/7e83ca86-f92d-49f2-9c12-d7681164daf9">

AI모델 생성

<img width="255" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/8d4e9ed6-32e5-4633-9b4d-c44b3ace4160">

데이터 수집

AI-hub의 17개 클래스 중 7개 클래스 사용하여 4가지 종류로 구분 → 중량충격음(2개), 가구끄는소리(1개), 악기(2개), 애완동물(2개)

법적 층간소음 종류인 충격음 3가지(발걸음소리, 가구끄는소리), 공기전달소음 1가지(악기소리), 법적기준이 없지만 최근 반려동물 분양 가구수가 증가하는 것을 반영하여 반려동물소리를 포함

해당 오디오 파일을 이미지(멜 스펙토그램)로 변환하여 AI모델에 학습

데이터 전처리
<img width="257" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/4a0a7124-8fe0-4307-9267-1222831ef7f6">




















