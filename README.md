<h1 align="center">안녕하세요, 백형준입니다 👋</h1>
<p align="center">
  <b>대용량 실시간 데이터를 안정적으로 수집하고 서빙하는 Data Engineer</b><br/>
  백엔드 실무에서 데이터 생성 원리를 이해하고, Kafka·Spark 기반 실시간 파이프라인 설계부터 ClickHouse OLAP 서빙까지 End-to-End로 구축합니다.
</p>

---

## 🔧 Tech Stack

**Data Engineering**  
`Apache Kafka` `Apache Spark (Structured Streaming)` `ClickHouse` `Airflow` `Elasticsearch` `Python`

**Cloud & Infra**  
`AWS (Lambda · S3 · EventBridge · API Gateway)` `Docker` `Prometheus` `Grafana` `Nginx`

**Backend**  
`NestJS` `TypeScript` `PostgreSQL` `MongoDB` `Redis (BullMQ · Cache)`

**Data Science & AI**  
`PyTorch` `LightGBM` `TabNet` `Optuna` `Ollama`

---

## 🚀 Currently Building

**[CoinWhale](https://coinwhale.dev)** — 실시간 금융 데이터 통합 분석 플랫폼 (운영 중)

- 일일 7,200만+ 건 수집 · 평균 836 req/s · 피크 9.1K TPS · 14개 Docker 컨테이너 운영
- Kafka 18 Topics → PySpark 7 Plugin Auto-Discovery → ClickHouse 15 테이블 Medallion 아키텍처
- ReplacingMergeTree + 3-레이어 체크포인트 방어로 멱등 파이프라인 구축 (88회 재시작 루프 → 0회)
- Ollama 로컬 LLM (DeepSeek-R1 / Qwen3.5) fast/deep 모드 · 장애 시 OpenAI 자동 Fallback
- Prometheus · Grafana 실시간 모니터링 · mem-watchdog 자동 메모리 관리

---

## 📌 Featured Projects

| 프로젝트 | 설명 | 스택 |
|---|---|---|
| [CoinWhale](https://coinwhale.dev) | 실시간 금융 데이터 E2E 파이프라인 · Medallion 아키텍처 | Kafka, Spark, ClickHouse, Airflow, Ollama |
| AWS Data Platform | 서버리스 ETL 100% 자동화 · 운영 서버 부하 0% 달성 | AWS Lambda, EventBridge, S3, PostgreSQL, Metabase |
| RouteBag | 대규모 축제 플랫폼 · P95 응답 92% 단축 (15s → 1.2s) | NestJS, Redis, BullMQ, MongoDB |
| [TabBoost (ICTC 2025)](https://drive.google.com/file/d/17tNZVVDlaZRCHZMGJxhz0ZGp8PXqs3ki/view?usp=drive_link) | LightGBM+TabNet 앙상블 · F1-Score +33.4% | Python, LightGBM, PyTorch, Optuna |

---

## 🏆 Certifications & Awards

- **SnowPro Core Certification** — Snowflake (2026.02)
- **ICTC 2025 국제 학술대회 논문 게재** — TabBoost (2025.11)
- **관광 데이터 활용 공모전 장려상** — 한국관광공사 사장상 (2024)
- **관광 데이터랩 활용 경진대회 장려상** — 한국관광공사 사장상 (2024)
- **GBT Hackathon 최우수상** — 한국외대 총장상 (2023)
- **용인시 SW/AI 해커톤 장려상** — 한국외대 AI교육원 (2023)

---

## 📫 Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/%ED%98%95%EC%A4%80-%EB%B0%B1-4b5aa6294/)
[![Velog](https://img.shields.io/badge/Velog-20C997?style=flat&logo=velog&logoColor=white)](https://velog.io/@vividbaek/posts)
[![Email](https://img.shields.io/badge/Email-wlwns0324@gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:wlwns0324@gmail.com)
[![CoinWhale](https://img.shields.io/badge/CoinWhale-coinwhale.dev-000000?style=flat&logo=vercel&logoColor=white)](https://coinwhale.dev)
