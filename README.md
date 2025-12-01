# 🍽️ HanNoon - 실시간 프랜차이즈 매출 분석 플랫폼

> Apache Flink와 Confluent Kafka 기반의 실시간 매출 분석 및 이상 거래 탐지 시스템

<div align="center">

![Apache Flink](https://img.shields.io/badge/Apache%20Flink-E6526F?style=for-the-badge&logo=apache-flink&logoColor=white)
![Confluent Kafka](https://img.shields.io/badge/Confluent%20Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![Apache Avro](https://img.shields.io/badge/Apache%20Avro-FF6B35?style=for-the-badge&logo=apache&logoColor=white)

</div>

---

## 프로젝트 소개

### 개요
**HanNoon**은 프랜차이즈 사업자를 위한 **실시간 매출 분석 및 이상 거래 탐지 플랫폼**입니다. "한눈에 보는 매출 분석"이라는 의미로, 복잡한 매출 데이터를 직관적으로 시각화하고 실시간으로 모니터링할 수 있습니다.

### 핵심 가치
- **실시간성**: 초 단위 매출 데이터 실시간 처리 및 분석
- **안전성**: 중복 결제 및 이상 거래 패턴 즉시 탐지
- **통찰력**: 브랜드별/매장별 성과 비교 분석
- **확장성**: Confluent Kafka 기반 마이크로서비스 아키텍처

### 제공 기능
- 프랜차이즈 매출 실시간 모니터링
- 중복 결제 및 이상 거래 즉시 탐지
- 브랜드별 성과 분석 및 순위 제공
- 매출 트렌드 기반 비즈니스 인사이트

---


## 기술 스택

### Stream Processing & Data
<p>
 <img src="https://img.shields.io/badge/Apache%20Flink-E6526F?style=for-the-badge&logo=apache-flink&logoColor=white"/>
 <img src="https://img.shields.io/badge/Confluent%20Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white"/>
 <img src="https://img.shields.io/badge/Apache%20Avro-FF6B35?style=for-the-badge&logo=apache&logoColor=white"/>
 <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white"/>
</p>

### Backend & Integration
<p>
 <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
 <img src="https://img.shields.io/badge/WebSocket-010101?style=for-the-badge&logo=socket.io&logoColor=white"/>
 <img src="https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white"/>
</p>

### Frontend & Visualization
<p>
 <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white"/>
 <img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white"/>
 <img src="https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chart.js&logoColor=white"/>
</p>

### DevOps & Infrastructure
<p>
 <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
 <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white"/>
</p>

---

## 주요 기능

### 실시간 매출 분석
- **브랜드별 매출 집계**: Apache Flink 기반 실시간 브랜드 매출 분석
- **분단위 매출 트렌드**: 시간대별 매출 변화 실시간 추적
- **매장별 성과 비교**: 동일 브랜드 내 매장 간 매출 순위
- **프랜차이즈 TOP 매장**: 일별 최고 매출 매장 실시간 순위

### 이상 거래 탐지
- **중복 결제 감지**: 동일 사용자의 연속 결제 패턴 실시간 탐지
- **결제 한도 모니터링**: 비정상적인 고액 결제 패턴 감지
- **동일인 결제 추적**: 같은 사용자의 다중 매장 결제 패턴 분석
- **실시간 알림**: 의심스러운 거래 즉시 알림 및 로깅

### 통합 대시보드
- **실시간 차트**: 매출 데이터 실시간 시각화
- **브랜드 필터링**: 특정 브랜드 매출 데이터 집중 모니터링
- **알림 패널**: 이상 거래 및 시스템 알림 실시간 표시
- **리포트 생성**: 매출 분석 리포트 자동 생성 및 다운로드

---

<div align="center">

### "한눈에 보는 프랜차이즈 매출 분석"

</div>


# 🏪 Store Inactivity Detector

![Java](https://img.shields.io/badge/Java-17-007396?style=flat-square&logo=java&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white)

해당 레포는 Kafka 토픽으로 유입되는 결제/활동 데이터를 실시간으로 분석하여, **일정 시간 동안 활동이 없는 상점(Store)을 자동으로 감지하는 모니터링 애플리케이션**입니다.

---

## 기능

- `test-topic`에서 메시지 소비
- 각 store_brand + store_id 조합의 마지막 활동 시간 추적
- 30초 동안 활동이 없는 상점 감지
- 비활성 상태로 감지된 상점 정보를 `3_non_response` 토픽으로 전송

## 사전 요구사항

- Java 17 이상
- Gradle
- Docker 및 Docker Compose
- purchase-main 프로젝트가 실행 중이고 `test-topic`에 데이터를 전송 중이어야 함

## 실행 방법

1. 권한 부여
   ```bash
   sh chmod-scripts.sh
   ```

2. 토픽 생성 및 애플리케이션 실행
   ```bash
   ./run.sh
   ```

## 알림 형식

비활성 상태로 감지된 상점에 대한 알림은 다음과 같은 JSON 형식으로 전송됩니다:

```json
{
  "alert_type": "inactivity",
  "store_brand": "[store_brand 값]",
  "store_id": [store_id 값],
  "last_activity_time": [timestamp],
  "current_time": [timestamp],
  "inactive_seconds": [seconds]
}
```

## 토픽 확인 방법

Kafka Control Center UI에서 토픽 데이터를 확인할 수 있습니다.
- 접속 URL: http://localhost:9021
- Topics 메뉴에서 `3_non_response` 토픽 선택
- Messages 탭에서 메시지 확인

## 아키텍처

```
[purchase-main]      [payment_guard-main]
Excel 데이터 ---> test-topic ---(가공)--> 3_non_response
                          |
                   상태 관리 및 비활성 감지
```

