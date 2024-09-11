[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/zHsKfIy0)
# Dialogue Summarization | 일상 대화 요약

## Team

| <img src="https://drive.google.com/uc?export=view&id=1LHSq2m119E8Vc590kM6PCwBF9quxjY4R" alt="정인웅" width="150" height="100"> | <img src="https://drive.google.com/uc?export=view&id=1Fg7LNgBWTcaBBXEaVLDwI73o6nklBApt" alt="이범희" width="150" height="100"> | <img src="https://drive.google.com/uc?export=view&id=1G2GLuzvsoSigbdlHFneNkNdUCnRss_Z3" alt="안수민" width="150" height="100"> | <img src="https://drive.google.com/uc?export=view&id=1rfLaDJocTPO2c0ctPnCOebACb39Uz3f2" alt="진수훈" width="150" height="100"> |
| :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: | :--------------------------------------------------------------: |
|            [정인웅](https://github.com/Messengerwoong)             |            [이범희](https://github.com/tmttd)             |            [안수민](https://github.com/soomnia)             |            [진수훈](https://github.com/huniii32)             |
| - Data Processing <br> - Modeling | - Research <br> - Modeling | - Data Augementation <br> - Modeling  | - Data Processing, Augementation <br> - Modeling |


## 0. Overview
### Environment
- Ubuntu 20.04.6 LTS
- GPU: RTX 3090 / 24 GB
- Memory: 60G


## 1. Competiton Info

### Overview
- [Dialogue Summarization | 일상 대화 요약](https://stages.ai/competitions/320/overview/description)

학교 생활, 직장, 치료, 쇼핑, 여가, 여행 등 광범위한 일상 생활 중 하는 대화들에 대해 요약합니다.

- `#비공개대회` `#UpstageAILab3기` `#NLPAdvanced`

### Timeline
- August 29, 2024 - Start Date
- September 10, 2024 - Final submission deadline

## 2. Components

### Directory
```

```

## 3. Data descrption

### Dataset overview

- fname <br>
대화 고유번호

- dialogue <br>
최소 2명에서 최대 7명이 등장하여 나누는 대화 내용 <br> 각각의 발화자를 구분하기 위해 `#Person”N”#`: 을 사용하며, 발화자의 대화가 끝나면 `\n` 으로 구분

- summary : 해당 대화를 바탕으로 작성된 요약문

### Data Processing
1. Data Cleaning 진행
    1. 중복된 summary 및 잘못된 summary 삭제
    2. 일부 잘못 설정된 special token 수정

2. Data Augmentation
    1. LLM을 이용한 증강 시도
    2. EDA를 통한 증강 시도
    3. Back Translation을 통한 증강 시도



## 4. Modeling

### Model descrition
. gogamza-kobart-base-v1 <br>
. ainize-kobart-news

### Modeling Process

- 데이터 전처리
- 데이터 증강
- 모델 선정 및 학습

## 5. Result
Rouge-Score
### Leader Board
> PUBLIC <br>
![PUBLIC](/docs/img/leaderboard-public.PNG)

> PRIVATE <br>
![PRIVATE](/docs/img/leaderboard-private.PNG)

> BEST SCORE <br>
![Best](/docs/img/best_score.PNG)
### Presentation

- [💾 PDF](/docs/pdf/Upstage%20AI%20Lab%203기_NLP%20경진대회_발표자료_8조.pdf)

## etc
### Reference
- [baseline code](https://stages.ai/competitions/320/data/baseline)
