# 안녕하세요, 백형준입니다 👋

**대용량 실시간 데이터를 안정적으로 수집하고 서빙하는 Data Engineer**  
대규모 트래픽 처리와 백엔드 실무 경험을 통해 데이터 생성 원리를 깊이 이해하며,  
Kafka·Spark 기반 실시간 파이프라인 설계부터 ClickHouse OLAP 서빙까지 End-to-End로 구축합니다.

---

## 🔧 Tech Stack

**Data Engineering** `Apache Kafka` `Apache Spark (Structured Streaming)` `ClickHouse` `Airflow` `Elasticsearch` `Python`

**Cloud & Infra** `AWS (Lambda · S3 · EventBridge · API Gateway)` `Docker` `Prometheus` `Grafana` `Nginx`

**Backend** `NestJS` `TypeScript` `PostgreSQL` `MongoDB` `Redis (BullMQ · Cache)`

**Data Science & AI** `PyTorch` `LightGBM` `TabNet` `Optuna` `Ollama`

---

## 💼 Experience

**주식회사 페링 (Pering)** | Lead Developer & Data Engineer `2024.06 - 2026.01`

- **데이터 레이크 및 마트 구축 (Workload Isolation)**: 서비스 간섭 방지를 위해 50여 개의 운영 DB(MongoDB)와 분석 환경을 물리적으로 분리. EventBridge 기반 자동 아카이빙으로 **S3 데이터 레이크**를 구축하고, API Gateway 기반 On-Demand ETL을 통해 **PostgreSQL 데이터 마트**로 적재.
- **서버리스 ETL 파이프라인 최적화**: AWS Lambda 배치 사이즈 벤치마킹(최적점 4K 도출)으로 처리 성능 12% 개선 및 운영 서버 부하 0% 달성. Metabase를 연동하여 클라이언트 전용 실시간 KPI 대시보드 자동화.
- **RouteBag (대규모 축제 플랫폼)**: Redis, BullMQ를 도입한 비동기 대기열 설계로 동시 접속 수용량 5배 향상, P95 응답 속도 92% 단축 (15s → 1.2s).
- **FESPA (결제/멀티 서비스)**: NestJS Monorepo 기반 Web, CMS, Socket 앱 분리 설계 및 MongoDB 트랜잭션을 통한 결제 데이터 정합성 확보.

---

## 🚀 Currently Building

**[CoinWhale](https://coinwhale.dev)** — 실시간 금융 데이터 통합 분석 플랫폼 (운영 중)

- 일일 7,200만+ 건 수집 · 평균 836 req/s · 피크 9.1K TPS · 14개 Docker 컨테이너 운영
- Kafka 18 Topics → PySpark 7 Plugin Auto-Discovery → ClickHouse 15 테이블 Medallion 아키텍처
- ReplacingMergeTree + 3-레이어 체크포인트 방어(Process Lock, State Recovery, GAP Prune)로 멱등 파이프라인 구축 (88회 재시작 루프 → 0회)
- Prometheus · Grafana 실시간 모니터링 및 mem-watchdog을 통한 OOM 방지 및 자동 재시작 관리 체계 구축

---

## 📌 Featured Projects


| 프로젝트                                                                                                          | 설명                                                               | 스택                                                |
| ------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- | ------------------------------------------------- |
| [CoinWhale](https://coinwhale.dev)                                                                            | 실시간 금융 데이터 E2E 파이프라인 · Medallion 아키텍처                            | Kafka, Spark, ClickHouse, Airflow, Ollama         |
| AWS Data Platform (페링)                                                                                        | S3 데이터 레이크 및 PostgreSQL 마트 구축 · 서버리스 ETL 최적화                     | AWS Lambda, EventBridge, S3, PostgreSQL, Metabase |
| RouteBag (페링)                                                                                                 | 대규모 트래픽 대응 축제 플랫폼 · P95 응답 92% 단축                                | NestJS, Redis, BullMQ, MongoDB                    |
| FESPA (페링)                                                                                                    | 결제 및 다중 서비스 운영을 위한 Monorepo 아키텍처                                 | NestJS, MongoDB (Transaction), Redis              |
| [TabBoost (ICTC 2025)](https://drive.google.com/file/d/17tNZVVDlaZRCHZMGJxhz0ZGp8PXqs3ki/view?usp=drive_link) | 멀티모달 센서 데이터 병합(Sequential Stream Merge) OOM 극복 · F1-Score +33.4% | Python, LightGBM, PyTorch, Optuna                 |


---

## 🏆 Certifications & Awards

- **AWS Certified Solutions Architect (Associate)** — AWS (2026.04)
- **SnowPro Core Certification** — Snowflake (2026.02)
- **투자자산운용사** — 한국금융투자협회 (2021.02)
- **ICTC 2025 국제 학술대회 논문 게재** — TabBoost (2025.11)
- **관광 데이터 활용 공모전 장려상** — 한국관광공사 사장상 (2024.11)
- **관광 데이터랩 활용 경진대회 장려상** — 한국관광공사 사장상 (2024.12)
- **GBT Hackathon 최우수상** — 한국외대 총장상 (2023.10)
- **용인시 SW/AI 해커톤 장려상** — 한국외대 AI교육원 (2023.11)

---

## 📫 Contact

[LinkedIn](https://www.linkedin.com/in/%ED%98%95%EC%A4%80-%EB%B0%B1-4b5aa6294/)
[Velog](https://velog.io/@vividbaek/posts)
[Email](mailto:wlwns0324@gmail.com)
[CoinWhale](https://coinwhale.dev)
