<h1>층간 소음 측정 및 관리 공유 커뮤니티 서비스</h1>


<h2>프로젝트 개요</h2>

  <ul>
    <li>
      최근 증가하는 세종시의 층간소음 민원에 대응하여 빅데이터, IoT, AI, 클라우드 융합기술을 활용한        데이터 기반 관리 서비스를 개발하여 층간소음 문제를 예방 및 해결
    </li>
    <li>
      세종시의 총 인구수 연평균 증가율은 5.12%, 연 평균 증가율은 21% 기록
    </li>
    <li>
      2022년 접수된 층간소음 민원의 71%가 아이들 뛰거나 걷는 소리
    </li>
  </ul>

  <h3>프로젝트 구조도</h3>

  <img width="772" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/5273a201-5b0a-4436-9639-2d92a67860f2">

  
  <h3>활용 장비 및 개발 환경</h3>
  <ul>
    <li>
      IOT : python , VS Code , django , Kotlin , REST , Android Studio</li>
    <li>
      Cloud : python , VS Code , AWS , Jenkins , argo
    </li>
    <li>
      AI : python , colab , jupyer
    </li>
    <li>
        Bigdata : python
    </li>
  </ul>


<h2>수행절차 및 방법</h2>

<h3>Cloud</h3>

<p align="center">AWS Architecture</p>

<img width="708" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/c00baafb-7c0f-4738-82cf-4ca25ac5549e">


<p align="center">EKS Cluster</p>

<img width="606" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/c51b83bb-bc7a-4f70-b1c5-3425f6d743be">


<p align="center">CI/CD</p>

<img width="597" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/5f5fd34d-d8a9-4903-9929-dd6eefb6901d">

<h3>IOT</h3>
<ul>
  <li>소음 측정기로 1분 평균 데시벨 데이터를 지속적으로 전송</li>
  <li>반복 녹음 기능으로 층간 소음 녹음 파일을 기준치 이사의 소음 측정 시 데이터를 amazon s3에 전송</li>
</ul>

<h3>AI 모델 목적</h3>
<ul>
  <li>소음 녹음파일을 수집하고,이를 이미지화하여 구별</li>
  <li>"층간소음"에 해당하는 소음을 구분</li>
  <li>데이터 수집 및 스펙트로그램 분석</li>
  <img width="317" alt="image" src="https://github.com/bananaisgood/multi-it/assets/112065692/109fdcd1-e7c6-409a-8cfb-d2bffa36ba76">

</ul>









<h2>프로젝트 수행 결과</h2>

<h2>자체 평가 의견</h2>






















