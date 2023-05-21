---
layout: post
title:  "DDD(도메인 주도 설계) 모델링 프로세스"
categories: [프로세스]
tags: [번역, DDD, Beginner]
---

> 본 자료는 제가 번역한 자료입니다 :smile: <br>
> 원본: [ddd-crew (Github)](https://github.com/ddd-crew/ddd-starter-modelling-process) <br>
> 번역 장소: [d4veloper (Github)](https://github.com/D4veloper/ddd-starter-modelling-process)

## 도메인 주도 설계를 시작하는 모델링 프로세스
![DDD 스타터 프로세스](/assets/img/2023-05-21/ddd-starter-modelling-process-colored-KO.png)


## 단계
> ddd-crew에서 제시한 순서는 아래와 같습니다.<br>
> [Domain-Driven Design Starter Modelling Process]의 README.md 파일 참고

### 1. 이해
  - 비즈니스 모델과 사용자의 요구사항을 이해하세요.
  - `참고` 원본 그림에는 Align으로 표현 되어있으나, 설명에는 Understand로 표현되어 있습니다.

### 2. 탐구
  - 도메인 모델을 시각적으로 다른 사람과 __함께__ 탐구하세요.
  - `참고` Eric Evans의 저서 [도메인 주도 설계]에서도 __함께__ 탐구하는 것을 매우 중요하게 권장합니다.
  - 저는 [Event Storming](https://www.eventstorming.com/)을 즐겨 사용합니다.

### 3. 분해
  - 대상 도메인을 하위 도메인으로 분해하세요.
  - `참고` 처음에는 마음 가는데로 하더라도, 성숙도를 위해 Eric Evans의 저서 [도메인 주도 설계]의 p.458 [분리된 핵심] 파트 이후를 읽어보시기를 권장합니다.

### 4. 전략
  - 비즈니스 핵심 도메인의 차별화 전략을 세우세요.
  - `Insight` 비즈니스가 성공하기 위해서는 차별화 전략이 필수적입니다. 쿠팡은 e-커머스 플랫폼이지만, 배송을 핵심 도메인으로 볼 수도 있을 것입니다.

### 5. 연결
  - 하위 도메인을 느슨하게 결합된 아키텍처로 연결하세요.

### 6. 조직화
  - Bounded Context를 중심으로 팀을 구성하세요.
  - `Insight` 콘웨이의 법칙(SW 아키텍처는 조직의 의사소통 구조에 따라 결정됨)은 이곳에서도 적용이 됩니다.
  - `Insight` Bounded Context와 무관한 팀은 이상한 설계와 시스템 결과물을 만들어 낼 수도 있습니다.

### 7. 정의
  - 각 Bounded Context의 역할과 책임을 정의하세요.
  - [Bounded Context Canvas](https://github.com/ddd-crew/ddd-starter-modelling-process/blob/master/resources/bounded-context-canvas-v5.jpg)와 같은 도구를 활용하면 조금 더 쉽게 접근할 수 있습니다.

### 8. 코드
  - 전술적 설계 패턴을 활용하여 Bounded Context를 구현하세요.

## 정리
- 이번 포스팅에서는 초보자를 위한 DDD 스타터 프로세스를 간단히 알아보았습니다.
- 단계별 가이드는 차차 작성하겠습니다.
