# skt_ai_fellowship

- 연세대학교 산업공학과 시스템인텔리전스 연구실 (SIL)
- 3기 4번 과제 Smart Factory 서비스를 위한 진동/압력/온도 센서의 Anomaly Detection 개발 수행 
(https://www.sktaifellowship.com/d9788784-5df2-4782-bb12-c2ec7f651e39)
- 최주임팀 최영제, 주재현, 임형구



## [6월 진행 사항]
#### 1~2 주차 :

- SKT AI Fellowship 3기 면접
- 전체 OT 진행

#### 3 주차:

- 킥 오프 미팅
- **소통 방식 및 연구 방향성 설정** (notion 및 주간 회의 "목요일" zoom 미팅으로 진행)

#### 4 주차:

- Case Western Reserve University Bearing Data center 데이터 셋에 조사 및 적합성 검토
- 실험 환경, 불량 측정 방식, Data sample, 주파수 변환 방법 적용 예시 plot
- 최종적으로 CWRU 데이터 셋은 **"과도기 시점" 이 존재하지 않아 연구에 활용 제외하기로 결정**

## [7월 진행 사항]
#### 1주차 :

- SKT AI Fellowship 3기 Devocean에 1차 활동 기록 작성 및 공유 
[https://devocean.sk.com/blog/techBoardDetail.do?ID=163213&searchData=AI+Fellowship&page=&subIndex=&idList=%5B163217%2C+163221%2C+163222%2C+163224%2C+163225%2C+163213%2C+163197%2C+163205%2C+163196%2C+163191%2C+163192%2C+163189%2C+163185%2C+163179%2C+163173%2C+163168%2C+163170%2C+163167%2C+163152%2C+163138%2C+163125%2C+163114%2C+163116%2C+163054%2C+163029%2C+163008%2C+162986%2C+162994%2C+162976%2C+162968%2C+162962%2C+162915%2C+162904%2C+162750%2C+162735%2C+162714%2C+162713%2C+162700%2C+162692%2C+162576%2C+162534%2C+161250%2C+161147%2C+160842%2C+160835%2C+160620%2C+160623%2C+160298%2C+160038%2C+160012%2C+159980%2C+159948%2C+159409%2C+159414%2C+159334%2C+159337%2C+159311%2C+159229%2C+159230%2C+159075%2C+158966%2C+158774%2C+158688%2C+158674%2C+158657%2C+158649%2C+158639%2C+158512%2C+158484%2C+158482%2C+158466%2C+158428%2C+157805%2C+55053%2C+54957%2C+54840%2C+54295%2C+54041%2C+53660%2C+53290%2C+40435%2C+193%5D](https://devocean.sk.com/blog/techBoardDetail.do?ID=163213&searchData=AI+Fellowship&page=&subIndex=&idList=%5B163217%2C+163221%2C+163222%2C+163224%2C+163225%2C+163213%2C+163197%2C+163205%2C+163196%2C+163191%2C+163192%2C+163189%2C+163185%2C+163179%2C+163173%2C+163168%2C+163170%2C+163167%2C+163152%2C+163138%2C+163125%2C+163114%2C+163116%2C+163054%2C+163029%2C+163008%2C+162986%2C+162994%2C+162976%2C+162968%2C+162962%2C+162915%2C+162904%2C+162750%2C+162735%2C+162714%2C+162713%2C+162700%2C+162692%2C+162576%2C+162534%2C+161250%2C+161147%2C+160842%2C+160835%2C+160620%2C+160623%2C+160298%2C+160038%2C+160012%2C+159980%2C+159948%2C+159409%2C+159414%2C+159334%2C+159337%2C+159311%2C+159229%2C+159230%2C+159075%2C+158966%2C+158774%2C+158688%2C+158674%2C+158657%2C+158649%2C+158639%2C+158512%2C+158484%2C+158482%2C+158466%2C+158428%2C+157805%2C+55053%2C+54957%2C+54840%2C+54295%2C+54041%2C+53660%2C+53290%2C+40435%2C+193%5D)
- 연구 목적에 맞는 데이터 셋 추가 조사 (PHM 데이터 셋 위주 약 2010~2021 데이터 검토)

#### 2 주차:

- 3가지 구체적인 기준을 정하고 이에 해당하는 bearing data 조사
- "진동 여부", "Raw 데이터 여부", "과도기 시점" 3가지 기준으로 조사한 데이터 셋에 대한 발표 진행
- 모델링 부분에서는 USAD, TADGAN 구축 및 AI 프레임워크 통일 (pytorch → tensorflow)

#### 3~4 주차:

- PHM 2012 데이터셋을 활용하기로 최종 확정 및 Discrete wavelet transform으로 전처리 진행
- 본 연구진의 핵심 아이디어 였던 AGM (Anomaly GAP Maximization) 실험 진행 및 개선 사항 검토
- 중간 발표 준비 시작 (목차 설정)

## [8월 진행 사항]
#### 1주차 :

- AGM 실험 진행하면서 평가 지표에 대한 고민 커짐 (어떤 평가지표를 사용해야 하느냐에 대한 고민)
- PHM 2012 DATA 수상 솔루션 3가지 방법에 대해서 논문 발표 진행 
(Method 1 ~ 3) 구현  코드 
[https://github.com/hyeonggulim/-SKT-AI-FELLOWSHIP-3-phm-data-challenge2012-dataset/blob/main/preprocessing (winners solution).ipynb](https://github.com/hyeonggulim/-SKT-AI-FELLOWSHIP-3-phm-data-challenge2012-dataset/blob/main/preprocessing%20(winners%20solution).ipynb)
- DAGMM, USAD, GANOMALY 구현 결과 + AGM 프레임워크 적용 실험 
실험 결과 발표 (약 60 % 정도의 베어링에 대해서만 성능 개선) → 추가적인 개선 필요

#### 2 주차:

- 본격적인 중간 발표 자료 준비 & 발표 연습 & 리허설 진행
- 탑재와 관련된 가이드라인을 숙지하기 위해 그랜드뷰 개발자이신 임지성에게 교육 수강

#### 3~4 주차:

- 중간 발표 진행 ([https://titanumm.tistory.com/152?category=994343](https://titanumm.tistory.com/152?category=994343))
- 중간 발표는 10분간의 발표와 질의응답으로 진행 되었으며 "연구진의 아이디어와 실험 결과 및 향후 계획" 중심으로 발표
- 다른 팀의 멘토님들의 질문 정리 및 개선 사항 정리
- 마지막 주는 휴식

## [9월 진행 사항]
#### 1주차 ~ 2주차 :

- 최종 발표까지 남은 추후 TASK를 정리
- 전처리, 모델링 아이디어, 평가 방법 각 부분에 대해 앞으로의 계획 정리
- 중간 발표 때  질문 받았던 내용에 대해 고민 및 정리 (feedback 반영)
- 모델링 아이디어의 한계점 파악 및 아이디어 개선을 위한 노력 
(기존 아이디어의 문제점 파악)

#### 3 주차:

- 모델링 아이디어 (AGM)를 개선하기 위해서 집중
- 새로운 AGM 모델링 아이디어 2개의 방법 제시 & 추가 고민
→ 반복적인 실험을 통해 아이디어 개선 필요성을 느낌
- 전처리 부분에 있어서 DWT의 단점이 개선된 DT-CWT(dual Tree complex wavelet transform) 타당성 검토 (FFT→ STFT →DWT →SWT → DT-CWT 흐름 총 정리)

#### 4 주차:

- 증강 기반의 새로운 아이디어를 위해 다양한 증강 기법을 모두 검토 및 실험
(Tsuag 라이브러리, timesynth 라이브러리 증강 기법 모두 검토)
- 모델링 부분에 있어서 기존에 논문에 근거하여 Label 이 만들어진 원리 조사 
(힐버트 변환 기법에 초점을 둔 label로 전처리마다 label이 달라질 수 밖에 없는 한계 파악)
- 최종 평가 지표에 대해서 Detection 이 얼마나 빨랐는가, False Alarm이 얼마나 적었는가로 평가 지표를 확정


## [10월 진행 사항]
#### 1주차 ~ 2주차 :

- 새로운 모델링 아이디어에 대한 실험 진행 및 결과 발표
- 증강 기반 + classifier + ma(moving average)를 종합하여 모든 베어링에 대해서 성능 개선 확인

#### 3 주차:

- 그랜드뷰 탑재 관련해서 본격적으로 논의
- 탑재 관련 방식 두가지 방법에 대해 논의

#### 4 주차:

- 최종 발표 자료 준비에 집중
- 그랜드뷰 탑재를 위해 임지성 연구원님과 2차 회의
- 탑재를 위한 방향 최종 결정(score를 주고 받는 방식)

## [11월 진행 사항]
#### 1주차:

- 최종 발표 준비
- Devocean에 필수 공유 이외에 "주파수 변환 방법 총 정리" 글 공유 준비

#### 2주차:

- 최종 발표 진행
- 수료식 및 시상식.



## 4팀_최주임_활동 기록
[Devocean - 4회]
1. Smart Factory 서비스를 위한 진동/압력/온도 센서의 Anomaly Detection 개발 - 연구계획(1) (https://devocean.sk.com/search/techBoardDetail.do?ID=163213&query=smart+factory&searchData=AI+Fellowship&page=&subIndex=&idList=%5B163455%2C+163356%2C+163325%2C+163252%2C+163213%2C+163205%2C+163137%5D) / 07.02
2. Smart Factory 서비스를 위한 진동/압력/온도 센서의 Anomaly Detection 개발 - 연구과정(2) (https://devocean.sk.com/search/techBoardDetail.do?ID=163325&query=smart+factory&searchData=AI+Fellowship&page=&subIndex=&idList=%5B163455%2C+163356%2C+163325%2C+163252%2C+163213%2C+163205%2C+163137%5D) / 08.29
3. Smart Factory 서비스를 위한 진동/압력/온도 센서의 Anomaly Detection 개발 - 주파수 변환 방법 총정리 (https://devocean.sk.com/search/techBoardDetail.do?ID=163455&query=smart+factory&searchData=AI+Fellowship&page=&subIndex=&idList=%5B163455%2C+163356%2C+163325%2C+163252%2C+163213%2C+163205%2C+163137%5D) /11.05
4. Smart Factory 서비스를 위한 진동/압력/온도 센서의 Anomaly Detection 개발 - 연구 결과 (https://devocean.sk.com/internal/index.do) /
[주차별 활동기록 - 13회]
5. [SKT AI Fellowship] 3기 선정 후기 (https://titanumm.tistory.com/144?category=994343) / 6.6
6. [SKT AI Fellowship 3기][4주차] 1차 활동 기록 공유 SKT DEVOCEAN 공유(https://titanumm.tistory.com/147?category=994343) / 07.06
7. [SKT AI Fellowship 3기][3주차] NASA , CWRU BEARING DATASET (https://titanumm.tistory.com/148?category=994343) / 07.07
8. [SKT AI Fellowship 3기][5 & 6주차] Phm Data phm challenge 적합 타당성 검토 & 8월 중간 발표 계획(https://titanumm.tistory.com/149?category=994343) / 07.18
9. [SKT AI Fellowship 3기][7주차] PHM Bearing Dataset 데이터 상세 분석(https://titanumm.tistory.com/150?category=994343)/ 08.06
10. [SKT AI Fellowship 3기][8 & 9 주차] Phm Bearing Data Challenge 수상 솔루션 분석 & 구현된 모델 TEST (https://titanumm.tistory.com/151?category=994343)/ 08.06
11. [SKT AI FELLOWSHIP 3기][10 & 11주차] 8/18 (수요일) 중간 발표 (https://titanumm.tistory.com/152?category=994343) / 08.21
12. [SKT AI FELLOWSHIP 3기][9월 1주차] 모델 개선 아이디어 (https://titanumm.tistory.com/154?category=994343) / 09.17
13. [SKT AI FELLOWSHIP 3기][9월 3주차] 모델링 개선 & 전처리 향후 계획 (https://titanumm.tistory.com/155?category=994343) / 09.17
14. [SKT AI Fellowship 3기] SK Careers Journal 인터뷰 진행 (https://titanumm.tistory.com/156?category=994343) 10.07
15. [SKT AI Fellowship 3기][9월 5주차] 데이터 증강 기법 적용 검토 (https://titanumm.tistory.com/157?category=994343) / 10.09
16. [SKT AI Fellowship 3기][10월 1주차] 모델링 개선 결과 (https://titanumm.tistory.com/158?category=994343) / 10.09
17. [SKT AI Fellowship 3기] [10월 3주차] 최종 발표 준비 & 그랜드 뷰 탑재 준비 (https://titanumm.tistory.com/159?category=994343) / 11.10
[논문 리뷰 - 1회]
18. [KDD 2020] USAD: UnSupervised Anomaly Detection on Multivariate Time Series (https://yjchoi-95.gitbook.io/paper-review/paper-review/kdd-2020-usad-unsupervised-anomaly-detection-on-multivariate-time-series) / 7월 중순
[github 코드 repository]
1. SKT-AI-FELLOWSHIP-3-phm-data-challenge2012-dataset (phm 데이터 셋 전처리 관련 코드들) (https://github.com/hyeonggulim/skt_ai_fellowship)
2. https://github.com/hyeonggulim/skt_ai_fellowship (활동 내용 및 CWRU, NASA 전처리 코드들) (https://github.com/hyeonggulim/skt_ai_fellowship)
3. https://github.com/yjchoi-95/SKT_AI_fellowship_3rd (모델 구현 코드들) (https://github.com/yjchoi-95/SKT_AI_fellowship_3rd) 
