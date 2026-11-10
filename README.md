# Hi, I'm Abduhamid Raximov 👋

**Data Engineer & Python Backend Developer** based in Uzbekistan — building production Databricks/PySpark pipelines, high-load ClickHouse + PostgreSQL analytical platforms, distributed microservices, and hardware/IoT integrations.

---

## 🔧 Tech Stack

**Data Engineering & ML**
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat&logo=databricks&logoColor=white)
![Apache Spark](https://img.shields.io/badge/PySpark-E25A1C?style=flat&logo=apachespark&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow%2FKeras-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly%20%2F%20Streamlit-3F4F75?style=flat&logo=plotly&logoColor=white)
`ETL/ELT` `DWH / Star Schema` `Optuna` `SHAP`

**Backend & Microservices**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white)
![DRF](https://img.shields.io/badge/Django%20REST%20Framework-ff1709?style=flat)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat&logo=celery&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat&logo=rabbitmq&logoColor=white)
`SQLAlchemy` `Alembic` `gRPC / Protobuf` `OpenAPI / Swagger` `WebSockets`

**Databases & Storage**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFDD00?style=flat&logo=clickhouse&logoColor=black)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![PostGIS](https://img.shields.io/badge/PostGIS-336791?style=flat)
`Logical Replication` `Sharding` `Materialized Views` `OLAP` `PL/pgSQL` `MS SQL` `MySQL`

**Infrastructure, Systems & Protocols**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git%20%2F%20CI%2FCD-F05032?style=flat&logo=git&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana%20%2F%20Prometheus-F46800?style=flat&logo=grafana&logoColor=white)
![C](https://img.shields.io/badge/C%20%2F%20C%2B%2B-00599C?style=flat&logo=cplusplus&logoColor=white)
`Docker Compose` `Gunicorn` `systemd` `IEC-104` `RS-232 / COM-port` `ESC/POS` `pytest` `Jira`

---

## 🏗️ Production Systems & Experience

### 🏥 Healthcare Data Engineering Pipelines — Symplast (Remote, US)
> **Databricks / PySpark** pipelines over bronze-layer files in Unity Catalog Volumes

- Maintain and scale document-conversion pipelines with **SHA-256** content hashing for file deduplication and identification
- Own pipeline workstreams end to end: root-cause investigation, optimization, and production releases
- Eliminated throughput bottlenecks around Unity Catalog volume-mount latency, hanging LibreOffice subprocesses, and 504 timeouts on long-running notebooks

### 🏛️ Situational Center — Government Analytics Platform (UZINFOCOM)
> **ClickHouse + PostgreSQL** hybrid aggregating millions of records from **tax, traffic police, 112 emergency, sanitary service, MyGov, and utilities**

- Dynamic Query Builders: multi-parameter filtering, timeline grouping, and trend calculation over **1M+ records**
- Fixed 30s export timeouts via **Celery** background jobs with a status-polling API (`pending → processing → downloading → finished`)
- SOATO-normalized reporting across 12+ modules & secure government/corporate API integrations with **OAuth2 / eGov SSO**

### 🗺️ GeoServer / PostGIS Spatial Infrastructure
> Geospatial data engineering for water billing, district heating, and municipal mapping

- PostgreSQL 15 **Selective Logical Replication** (Pub/Sub) — only geometry columns, protecting OLTP from heavy WMS/WFS load
- **Materialized Views** with `CONCURRENT` refresh, spatial indexes, and `EPSG:3857` Web Mercator layers behind Docker + Nginx

### ⚡ Energy Monitoring System (IEC-104)
> Real-time 24/7 industrial telemetry ingestion from national grid stations

- Custom **IEC-104** frame decoder & encrypted structured data ingestion written to ClickHouse/PostgreSQL every few seconds
- Consolidated 20 `systemd` station services into a single `asyncio` service and stabilized ClickHouse/Gunicorn RAM usage on Ubuntu

### 🔌 AGNKS Fiscal System (uGaz) & Geospatial/Automation Tools
> Hardware-level fiscal integration & standalone geospatial/automation engineering

- Built RS-232/COM-port **KKM driver from scratch** (`STX, ENQ, ACK, LRC XOR, Little-Endian`), integrating **7 KKM vendors** (*Simurg, SmartOne, UzKassa, EPOS, Fiscal Box, RahmatPOS, Era*), cutting latency **15s → 1.3s** with async ACK, Soliq OFD fiscalization, QR generation, and Django + Celery COM-port locking
- Built **SunCheck** (3D sunlight-compliance analysis across 2,880 Tashkent buildings from OSM data with PDF audit reports) and **e-Login** (bulk CSV/Excel automation for ~1,000 accounts)

---

## 🎓 School 21 Portfolio (`79` Completed Projects)

Grouped engineering tracks from the peer-to-peer **School 21** program (`volentib`):

| Track Repository | Modules | Core Focus & Technologies |
| --- | ---: | --- |
| [**SQL**](https://github.com/raximov/SQL) | 13 | Relational modeling, DML, snapshots, TSP, B-tree/covering indexes (`EXPLAIN ANALYZE`), OLAP window functions, isolation levels, PL/pgSQL procedures/triggers, Star-schema DWH/ETL, `Info21` |
| [**data-science**](https://github.com/raximov/data-science) | 14 | Python OOP, profiling, Pandas, SQL+Pandas, DataViz, MovieLens analytics, Food Nutrition ML, Twitter NLP (`Word2Vec`), Bank Churn MLP (Scikit-learn, TensorFlow/Keras `GradientTape`, pure NumPy FCNN) |
| [**ML**](https://github.com/raximov/ML) | 7 | EDA, Linear/Ridge/Lasso/ElasticNet from scratch, Optuna & SHAP model validation, classification pipelines, Decision Trees, PCA/UMAP dimensionality reduction, clustering |
| [**python-backend**](https://github.com/raximov/python-backend) | 14 | Flask/FastAPI OpenAPI APIs, DI & clean architecture, Roguelike MVC, Maze/SimpleNavigator graph algorithms, Nginx reverse proxy/TLS, gRPC Auth, RabbitMQ/Redis event workers, PostgreSQL sharding |
| [**BSA**](https://github.com/raximov/BSA) | 19 | Stakeholder analysis, BPMN 2.0, DFD, Sequence/State diagrams, User Stories, Use Cases, SRS/SRD, NFRs, REST & SOAP integration specifications |
| [**c-and-linux**](https://github.com/raximov/c-and-linux) | 12 | C libraries (`s21_string+`, `s21_math`, `s21_decimal`, `s21_matrix`, `SimpleBashUtils`, `BrickGame`), C/C++ (`Maze`, `SimpleNavigator`, `3DViewer v2`, `C++ MLP`), Ubuntu server admin (`D01_Linux`) |

Other portfolio highlights: [**medalion-project**](https://github.com/raximov/medalion-project) (Azure End-to-End Medallion Data Pipeline) · [**new_york_taxi-report-REST-API**](https://github.com/raximov/new_york_taxi-report-REST-API) · [**flightstatistics**](https://github.com/raximov/flightstatistics)

---

## 📊 LeetCode & Education

- [![LeetCode](https://img.shields.io/badge/LeetCode-270%2B%20solved-FFA116?style=flat&logo=leetcode&logoColor=white)](https://leetcode.com/u/abduhamid_r) · **GRE – ETS (2024)**
- **M.S. Applied Mathematics & Informatics** — Bukhara State University, GPA `93/100` (2023–2025)
- **B.S. Mathematics** — National University of Uzbekistan, GPA `82/100` (2019–2023)
- **School 21** — Intensive software & data engineering program (2024–Present)

---

## 📫 Contact

[![Email](https://img.shields.io/badge/Email-abduhamidraximov01%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:abduhamidraximov01@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abduhamid-rakhimov-758ba2238/)
[![Telegram](https://img.shields.io/badge/Telegram-@abduhamid__r-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/abduhamid_r)

*Open to remote and on-site Data Engineering, Backend, and Python Engineering opportunities.*
