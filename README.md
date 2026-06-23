# 안녕하세요, 백형준입니다 👋

**대용량 실시간 데이터를 안정적으로 수집하고 서빙하는 Data Engineer**
대규모 트래픽 처리와 백엔드 실무 경험을 통해 데이터 생성 원리를 깊이 이해하며, Kafka·Spark 기반 실시간 파이프라인 설계부터 ClickHouse OLAP 서빙, AI Agent를 위한 데이터 플랫폼 구축까지 End-to-End로 수행합니다.

---

## 🌱 Open Source Contributions

**Apache Airflow & kafka-python Contributor**

Contributing practical documentation, runnable examples, and operational guidance to Apache Airflow and kafka-python. Focused on clarifying real-world workflow patterns, retry strategies, task orchestration behavior, and Kafka consumer semantics.

문서와 예제 중심의 작은 기여부터 시작해, 실제 사용자들이 헷갈리기 쉬운 동작을 더 명확하게 설명하는 데 집중했습니다. 현재는 Airflow와 Kafka 생태계의 사용 경험을 바탕으로 documentation contribution을 이어가고 있으며, 이후에는 테스트·버그 수정·core 코드 레벨의 기여까지 확장하는 것을 목표로 하고 있습니다.

| Project        | PR                                                      | Contribution                                                                                                                                                                  |
| -------------- | ------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Apache Airflow | [#67705](https://github.com/apache/airflow/pull/67705)  | Added guidance for automated remediation guardrails in retry workflows, including cooldown markers, maximum automatic action counts, and operational safety considerations.   |
| Apache Airflow | [#67022](https://github.com/apache/airflow/pull/67022)  | Added a zero-length dynamic task mapping no-op example, showing how skipped mapped tasks can still lead to a successful downstream summary task with the proper trigger rule. |
| Apache Airflow | [#66597](https://github.com/apache/airflow/pull/66597)  | Clarified `HttpOperator.response_filter` and XCom usage in documentation and system test examples. Updated the example to match the actual `httpbin /get` response structure. |
| kafka-python   | [#3015](https://github.com/dpkp/kafka-python/pull/3015) | Added a `KafkaConsumer` manual offset commit example and clarified that consumers should commit the next offset to consume (`message.offset + 1`).                            |

### Highlights

* 4 upstream PRs merged into Apache Airflow and kafka-python.
* Contributed documentation, runnable examples, and operational guidance around Airflow workflows and Kafka consumer behavior.
* Focused on reducing ambiguity for users by documenting real-world patterns such as HTTP response branching, dynamic task mapping edge cases, retry guardrails, and offset management.
* Next goal: expand contributions from documentation into tests, bug fixes, and core implementation work.

---

## 🔧 Tech Stack

### Data Engineering

`Apache Kafka` `Apache Spark (Structured Streaming)` `ClickHouse` `Apache Airflow` `Elasticsearch` `Python`

### Cloud & Infra

`AWS (Lambda · S3 · EventBridge · API Gateway)` `Docker` `Prometheus` `Grafana` `Nginx`

### Backend

`NestJS` `TypeScript` `PostgreSQL` `MongoDB` `Redis (BullMQ · Cache)`

### Data Science & AI

`PyTorch` `LightGBM` `TabNet` `Optuna` `Ollama`

---

## 💼 Experience

### 주식회사 페링 (Pering)

**Lead Developer & Data Engineer** | 2024.06 - 2026.01

#### 데이터 레이크 및 마트 구축 (Workload Isolation)

* 서비스 간섭 방지를 위해 50여 개의 운영 DB(MongoDB)와 분석 환경을 물리적으로 분리
* EventBridge 기반 자동 아카이빙으로 S3 데이터 레이크 구축
* API Gateway 기반 On-Demand ETL을 통해 PostgreSQL 데이터 마트 적재

#### 서버리스 ETL 파이프라인 최적화

* AWS Lambda 배치 사이즈 벤치마킹을 통해 최적 처리 단위(4K) 도출
* 처리 성능 12% 개선 및 운영 서버 부하 0% 달성
* Metabase 기반 클라이언트 전용 KPI 대시보드 자동화

#### RouteBag (대규모 축제 플랫폼)

* Redis Cache 및 BullMQ 기반 비동기 대기열 설계
* 동시 접속 수용량 5배 향상
* P95 응답 속도 92% 단축 (15s → 1.2s)

#### FESPA (결제·멀티 서비스)

* NestJS Monorepo 기반 Web, CMS, Socket 서비스 분리 설계
* MongoDB Transaction 기반 결제 데이터 정합성 확보

---

## 🚀 Currently Building

### CoinWhale

실시간 금융 데이터 통합 분석 플랫폼 (운영 중)

* 일일 1.6억+ 이벤트 처리
* 평균 1,900 req/s
* 피크 14.0K TPS
* Binance WebSocket 18 Streams 운영

#### Real-Time Data Platform

* Kafka 18 Topics / 36 Partitions
* Spark Structured Streaming 기반 실시간 처리
* ClickHouse Medallion Architecture 구축
* dbt 기반 Gold Analytics Mart 및 Evidence Layer 운영

#### Reliability & Operations

* ReplacingMergeTree 기반 멱등 처리 파이프라인 구축
* 3단계 체크포인트 방어 (Process Lock · State Recovery · GAP Prune)
* Spark 재시작 루프 88회 → 0회 개선
* Prometheus · Grafana 기반 운영 모니터링 체계 구축
* OOM 자동 감지 및 Runtime Self-Healing 운영

#### AI Agent Layer

* Advisor Chat: Planner → Tool Execution → Evidence QA 기반 금융 분석 Agent
* News RAG: Qdrant Semantic Search + ClickHouse Fallback
* Market Decision Agent: 5초 Trigger Detector + Async Decision Worker
* Ops Agent: Incident Triage · Evidence Collection · Approval Workflow

---

## 📌 Featured Projects

| 프로젝트                                                                                                          | 설명                                                               | 스택                                                |
| ------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- | ------------------------------------------------- |
| [CoinWhale](https://coinwhale.dev)                                                                            | 실시간 금융 데이터 E2E 파이프라인 · AI Agent 플랫폼                              | Kafka, Spark, ClickHouse, Airflow, LangGraph      |
| AWS Data Platform (페링)                                                                                        | S3 데이터 레이크 및 PostgreSQL 마트 구축 · 서버리스 ETL 최적화                     | AWS Lambda, EventBridge, S3, PostgreSQL, Metabase |
| RouteBag (페링)                                                                                                 | 대규모 트래픽 대응 축제 플랫폼 · P95 응답 92% 단축                                | NestJS, Redis, BullMQ, MongoDB                    |
| FESPA (페링)                                                                                                    | 결제 및 다중 서비스 운영을 위한 Monorepo 아키텍처                                 | NestJS, MongoDB Transaction, Redis                |
| [TabBoost (ICTC 2025)](https://drive.google.com/file/d/17tNZVVDlaZRCHZMGJxhz0ZGp8PXqs3ki/view?usp=drive_link) | 멀티모달 센서 데이터 병합(Sequential Stream Merge) OOM 극복 · F1-Score +33.4% | Python, LightGBM, PyTorch, Optuna                 |

---

## 🏆 Certifications & Awards

* AWS Certified Solutions Architect – Associate (2026.04)
* SnowPro Core Certification (2026.02)
* 투자자산운용사 (2021.02)
* ICTC 2025 국제 학술대회 논문 게재 (TabBoost)
* 관광 데이터 활용 공모전 장려상 (한국관광공사)
* 관광 데이터랩 활용 경진대회 장려상 (한국관광공사)
* GBT Hackathon 최우수상 (한국외국어대학교 총장상)
* 용인시 SW/AI 해커톤 장려상

---

## 📫 Contact

* LinkedIn: https://www.linkedin.com/in/형준-백-4b5aa6294/
* Velog: https://velog.io/@vividbaek/posts
* Email: [wlwns0324@gmail.com](mailto:wlwns0324@gmail.com)
* CoinWhale: https://coinwhale.dev
