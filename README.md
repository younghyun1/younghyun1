# Young Hyun Chi / 지영현 / 池營賢

Backend Software Engineer · Rust / Infrastructure / Data Pipelines

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=orange)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=green)
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)
![Axum](https://img.shields.io/badge/Axum-000000?style=for-the-badge&logo=rust&logoColor=orange)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Arch Linux](https://img.shields.io/badge/Arch%20Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Amazon Linux](https://img.shields.io/badge/Amazon%20Linux-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=FF9900)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-000000?style=for-the-badge&logo=apple&logoColor=white)
![Protocol Buffers](https://img.shields.io/badge/Protocol%20Buffers-3367D6?style=for-the-badge&logo=google&logoColor=white)
![BACnet](https://img.shields.io/badge/BACnet-004B87?style=for-the-badge&logo=home-assistant&logoColor=white)
![Modbus](https://img.shields.io/badge/Modbus-FFCC00?style=for-the-badge&logo=modin&logoColor=000000)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=for-the-badge&logo=socketdotio&logoColor=white)

---

## 1. Introduction

I am a backend-focused software engineer with experience shipping and operating services across industrial, consumer, and data-heavy analytics contexts.

Recent work has included:

- Building Rust- and Java-based backends, pipelines, and infrastructure for:
  - A digital twin dashboard integrating data from thousands of environmental sensors for Samsung Construction & Trading, deployed on AWS.
  - Hyundai Motor Company’s Hyundai / Kia / Genesis official car apps (Android and iOS), working within a large Java/Spring ecosystem.
  - A K‑Pop group's official fan app backend and supporting tooling.
- Designing and deploying a Rust + PostgreSQL backend and data collection pipeline for an AI-based YouTube analytics product on AWS and GCP.

I care about making web services that actually leverage the performance of modern hardware and languages while staying maintainable for the teams that operate them. Rust, static binaries, careful query design, and straightforward deployments are tools I’ve used to reduce costs and make systems more reliable.

Outside of software, I’ve worked in the military, translation/interpretation, logistics, journalism, and photography. Since 2023, my main focus has been backend engineering.

---

## 2. Background

- **Location:** Currently based in Colorado, USA  
- **Role:** Backend Software Engineer  
- **Education:** B. Eng in Software Engineering, Sungkyunkwan University (성균관대학교), Republic of Korea  
- **Other Experience:**  
  - Military service (KATUSA, 2nd Infantry Division, US/ROK Army)  
  - Translation and interpretation (technical and policy)  
  - Journalism and editorial work  
  - Night-shift logistics labor at warehouses and distribution centers  
  - Tutoring/lecturing and photography

---

## 3. Technology Stack

**Primary focus**

- **Languages:** Rust, C, C++, Java, Python, TypeScript/JavaScript, x86 Assembly  
- **Backend / Frameworks:** Axum, Spring Boot, Express, Django  
- **Data & Protocols:** PostgreSQL, MySQL, SQLite, Redis, Protocol Buffers, WebSockets  
- **Industrial / Protocol Integration:** BACnet, Modbus, environmental and power metering systems  
- **Infrastructure & Cloud:**  
  - AWS (EC2, S3, RDS, Lambda, CodeDeploy, GitHub Actions runners)  
  - GCP (Compute, storage, basic ML infra)  
  - Oracle Cloud, Naver Cloud  
  - Docker, Kubernetes, NGINX  
- **OS & Tooling:**  
  - Linux (Arch, Ubuntu, Amazon Linux), Windows, macOS  
  - Static linking, MUSL, scratch images  
  - CI/CD pipelines, CLI tooling, and automation scripts in Rust/Python

I am especially comfortable working on latency-sensitive services on constrained hardware, and with deployments where cost and operational simplicity matter as much as raw performance.

---

## 4. Professional Highlights

### Samsung C&T Digital Twin (via EAN Technology)

- Replaced an overcomplicated microservice architecture with a streamlined Axum (Rust) monolith serving a building energy management / digital twin dashboard.
- Cut monthly cloud infrastructure costs from roughly **$5,000 to ~$150** by simplifying architecture, optimizing queries, and tightening resource usage.
- Implemented around **30k LOC (~75% of the backend code)** and **80+ endpoints** with non-trivial domain logic and real-time constraints.
- Integrated thousands of building sensors and meters (BACnet, Modbus) and coordinated with on-premise servers at Samsung C&T HQ.
- Optimized PostgreSQL queries and schema design, bringing P99 latency to double-digit milliseconds on a 2-core, 4GB RAM instance (down from multi-second responses on some paths).
- Achieved **zero unplanned runtime shutdowns** across roughly nine months of production uptime, with extensive error handling and observability.
- Introduced and mentored teammates in Rust, helping them transition from Node.js/Java to writing production Rust services in a short period.

### Automotive & Consumer Apps

- Worked on backend systems supporting Hyundai, Kia, and Genesis official apps, collaborating with multiple vendors and teams in a large Java/Spring ecosystem.
- Implemented APIs, bug fixes, and data flows for services used by tens of millions of users across Asia and Europe.
- Built data ingestion and transformation pipelines to support internationalization, including Rust and Python utilities to integrate translated content into corporate databases.

### Data-Heavy Analytics & AI

- Designed PostgreSQL schemas and a Rust backend for an AI-based YouTube analytics platform.
- Led large-scale data collection efforts (tens of millions of comments/users) via YouTube APIs.
- Applied LLMs and on-server open-source models for summarization and insight extraction.
- Deployed and operated these systems on AWS and GCP, balancing cost with throughput.

---

## 5. Interests & Current Focus

**Technical interests**

- High-throughput webservers and low-latency APIs  
- Cache hierarchies and caching strategies (application-level and DB-level)  
- Effective concurrency through asynchrony and parallelism  
- On-premise infrastructure and hybrid setups  
- Infrastructure-as-code, CI/CD, and deployment automation  
- Operating systems, compilers, and low-level systems programming  
- Protocols and integrations for construction and electrical engineering systems

**Currently studying**

- Performance optimization in Rust services (allocation patterns, async runtimes, DB access strategies)  
- Electrical and HVAC systems (especially as they relate to building management and energy optimization)

---

## 6. Languages & Communication

- **Korean:** Native  
- **English:** C2 (TOEFL 117/120, IELTS 8.5/9.0)  
- **Others (basic/rudimentary):** French, German, Spanish, Mandarin  

I am comfortable working in international, multilingual environments, including military, corporate, and academic settings.

---

## 7. Personal Notes

- I graduated from **Sungkyunkwan University** with a B. Eng in Software Engineering, in a program that combined software, hardware, and network fundamentals with electronics and systems engineering.
- I care strongly about open-source ethics, labor rights in STEM, and building systems that are understandable and sustainable for the people who operate them.
- Outside of work I have long-standing interests in photography, journalism, and security/human rights issues.

---

## 8. How to Reach Me

- **Email:** [younghyun1@gmail.com](mailto:younghyun1@gmail.com)  
- **GitHub:** [github.com/younghyun1](https://github.com/younghyun1)  
- **LinkedIn:** [linkedin.com/in/younghyun-chi-a60b59a9](https://www.linkedin.com/in/young-hyun-chi-553431376/)
