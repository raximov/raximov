# Hi, I'm Abduhamid Raximov 👋

**Python Backend Developer** based in Uzbekistan — building data-intensive government systems, fiscal/IoT integrations, and geospatial platforms.

---

## 🔧 Tech Stack

**Backend**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white)
![DRF](https://img.shields.io/badge/Django%20REST%20Framework-ff1709?style=flat)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)

**Databases & Big Data**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFDD00?style=flat&logo=clickhouse&logoColor=black)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![PostGIS](https://img.shields.io/badge/PostGIS-336791?style=flat)

**Async & Protocols**
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat&logo=celery&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat)
`IEC-104` `RS-232 / COM-port` `ESC/POS`

**DevOps & Tools**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Jira](https://img.shields.io/badge/Jira-0052CC?style=flat&logo=jira&logoColor=white)

---

## 🏗️ What I've Built

### 🏛️ Situation Center — Government Analytics Platform
> ClickHouse + PostgreSQL hybrid aggregating data from **GNK, GAI, 112, SES, MyGov, communal services**

- Dynamic Query Builders: multi-parameter filters, timeline grouping, trend calculations over **1M+ records**
- Fixed 30s export timeout → Celery background job with status-polling API (`pending → processing → downloading → finished`)
- SOATO-normalized reporting across 12+ government agency modules

### 🗺️ GeoServer / PostGIS Spatial Infrastructure
> Geospatial data engineering for district-level mapping and monitoring

- PostgreSQL 15 **Selective Logical Replication** (Pub/Sub) — only geometry columns, protecting OLTP from heavy WMS/WFS load
- **Materialized Views** with `CONCURRENT` refresh and spatial indexes for sub-millisecond map queries
- EPSG:3857 Web Mercator layers for cadastral, billing, and infrastructure data

### 🔌 AGNKS Fiscal System (uGaz)
> Hardware-level fiscal integration for gas stations

- RS-232/COM-port **KKM driver from scratch** (STX, ENQ, ACK, LRC XOR, Little-Endian byte protocol)
- **7 KKM vendor** integrations: Simurg, SmartOne, UzKassa, EPOS, Fiscal Box, RahmatPOS, Era
- **15s → 1.3s** transaction speed via async ACK & dynamic polling
- Soliq OFD fiscalization, QR-code generation, COM-port locking between Django + Celery

### ⚡ Energy Monitoring System (UZINFOCOM)
> Real-time industrial data processing for government energy infrastructure

- IEC-104 industrial protocol data ingestion
- Encrypted stream processing, government API integration

---

## 📊 LeetCode

[![LeetCode](https://img.shields.io/badge/LeetCode-200%2B%20problems-FFA116?style=flat&logo=leetcode&logoColor=white)](https://leetcode.com/u/abduhamid_r)

---

## 🎓 Education

- **M.S. Applied Mathematics & Informatics** — Bukhara State University (GPA: 93/100)
- **B.S. Mathematics** — National University of Uzbekistan
- **School 21** — Intensive software engineering program

---

## 📫 Contact

[![Email](https://img.shields.io/badge/Email-abduhamidraximov01%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:abduhamidraximov01@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat&logo=linkedin&logoColor=white)]([https://linkedin.com/in/raximov](https://www.linkedin.com/in/abduhamid-rakhimov-758ba2238/))

---

*Open to remote and on-site opportunities*
