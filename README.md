# Huang Zhongying

**Location:** Osaka, Japan | **Visa:** Japan Humanities & International Services (valid until July 2028)
**Email:** hzying19@gmail.com

## Summary

- Senior Java Engineer with 14+ years of experience in backend and platform engineering.
- Strong track record in microservices architecture design, high-concurrency system optimization, and distributed system development.
- Experienced in leading core module development, resolving complex technical challenges, and mentoring team members.
- Experienced in AI-assisted development to improve development efficiency.
- Actively seeking Senior Java Engineer / Backend Engineer roles in Japan.

## Technical Skills

| Area | Skills |
|---|---|
| Languages | Java 8 / 17 (primary), SQL, JavaScript |
| Frameworks | Spring Boot, Spring Cloud, Spring, MyBatis |
| Frontend (basic) | HTML, JavaScript, Ajax, jQuery, ExtJs |
| Distributed & Middleware | Kafka, Redis, Nacos, Sentinel, Netty, RocketMQ, Redisson |
| DevOps & Infrastructure | Docker, Kubernetes, Jenkins, Git, Maven, Linux (Alibaba Cloud) |
| Databases | MySQL (query tuning, indexing), TiDB, ClickHouse |
| Monitoring & Observability | ELK, Prometheus, Grafana, Arthas |
| AI-assisted development | Claude Code |
| Other | Microservices architecture, multi-threading, high-concurrency; design patterns (Strategy, Template, Factory, Facade) |

## Career History

### Utsugi Co., Ltd. (Dispatched to Futech Co., Ltd.) | Jul 2025 – Oct 2026
*Java Engineer* · Java, Spring Boot, Redis, Redisson, TiDB

- Analyzed system requirements and wrote technical design documents
- Led functional planning and system decomposition for assigned modules
- Collaborated with cross-functional teams to deliver technical solutions

### CLPS Global (Dispatched to Standard Chartered Bank) | Jun 2025 – Jul 2025
*Java Engineer* · Java, Azure

- Collaborated with international teams (India, China) to resolve system incidents
- Participated in cross-timezone feature development and technical discussions

### Jincai Interconnect Data Services Co., Ltd. | Apr 2022 – Oct 2024
*Java Engineer (subsidiary of Fangxin Technology; tenure inherited)* · Spring Boot, Spring Cloud, Kafka, Redis, MySQL, Netty, Kubernetes, Nacos

- Participated in system architecture design and technology selection for key projects
- Led development of core modules in large-scale projects and resolved technical blockers
- Designed and optimized high-concurrency, large-volume data processing systems
- Mentored 2 newly hired developers (1 senior, 1 mid-level), explaining the business domain and system architecture and giving feedback through code reviews
- Served as a technical interviewer, assisting the architect and other departments in interviewing senior and mid-level Java developer candidates

### Fangxin Technology Co., Ltd. | Sep 2018 – Mar 2022
*Java Engineer* · Spring Boot, Kafka, Redis, Apollo, SpEL, Maven

- Designed system architecture and produced technical design documents
- Developed core infrastructure and foundational service components
- Conducted technical research and shared findings with the team
- Continuously improved system architecture and performance

### Guangzhou Boao Zongheng Network Technology Co., Ltd. | Aug 2017 – Aug 2018
*Associate Researcher (H6)* · Spring Boot, Redis, Dubbo, Disconf

- Participated in requirements and design reviews for the e-commerce platform's transaction and payment subsystems
- Wrote system design documents, assigned development tasks, and tracked progress
- Developed and delivered core modules

### Early Career | Software Engineer / Java Developer | Various Companies | Oct 2010 – Jul 2017
Java full-stack development across telecom, healthcare, e-commerce, and enterprise software.

## Key Projects

### Event Venue System | Jan 2026 – Mar 2026
*Spring Boot, TiDB, Prometheus, Claude Code*

An event venue system serving 50M registered users. After a user enters the venue, the system loads claimable benefits (discount coupons, points coupons, product redemption vouchers) based on user level and tags, and the user decides whether to claim them.

- Led requirements analysis and system design; defined system boundaries and identified key risks such as over-issuance and cache breakdown
- Load-tested a key API to 3,000 QPS
- Monitored key metrics with Prometheus and triggered alerts on anomalies
- Used Claude Code to assist with solution design and coding

### Distributed Proxy System for Web Crawlers | Feb 2023 – Oct 2024
*Alibaba Cloud, Netty, custom proxy protocol, obfuscation, load balancing*

High-performance distributed proxy system to solve IP-blocking issues caused by frequent calls to tax bureau APIs. Routes HTTP requests through a cloud proxy server to lightweight client agents deployed on customer PCs or cloud instances.

- Independently designed the full architecture, including request routing and automatic egress IP switching
- Built IP health monitoring and auto-removal mechanism, achieving 99.9%+ system availability
- Optimized Netty configuration and used separate read/write socket channels, supporting 30M+ daily API calls
- Designed large/small packet splitting to prevent head-of-line blocking
- Client agent runs on 2-core CPU + 2GB RAM; currently connected to 4,000+ client nodes

### Jincai Guard – Risk Control Service | Aug 2022 – Nov 2022
*Spring Boot, custom workflow engine, design patterns (Strategy, Template, Facade)*

Built a general-purpose risk indicator calculation engine and a custom workflow engine to power tax risk detection and report generation, covering ~1,000 risk indicators across all business processes.

- Designed the risk indicator engine using Strategy, Template, and Facade patterns with multi-threaded concurrent execution
- Designed the workflow engine with configurable node chains supporting MQ, SQL, HTTP, and sub-processes
- Led code review to ensure code quality and team consistency

### Shein Export Tax Refund Invoice Management System | Jan 2022 – Jul 2022
*Spring Cloud, Kafka, Redis, MySQL, Jenkins, Kubernetes, Nacos*

Designed and built the data processing subsystem for a full end-to-end export business tracking system covering product storage, ordering, customs filing, delivery, invoicing, and tax refund. Processes 200M+ records per month.

- Designed batch-based processing to separate pending and processed data, avoiding direct large-table updates
- Split datasets by merchant dimension to keep each batch under 20M records; used Kafka + Kubernetes for horizontal scale-out
- Used Redis as intermediate storage to reduce MySQL write pressure; added validation metadata to ensure data integrity
- Resolved critical production issues: DB transaction timeouts, CPU spikes to 100%, Redis cache data loss

### Guangdong Tax Bureau – Software Development Base Framework | Sep 2018 – Nov 2018
*Spring Boot, Maven, Kafka, RocketMQ, Redis, Elasticsearch*

Built a reusable foundational framework that won a government procurement contract with the Guangdong Provincial Tax Bureau and became the internal standard for all project teams.

- Logging middleware: supports delivery to Kafka, Redis, Elasticsearch, and ClickHouse; includes aggregation and statistics
- Messaging middleware: unified Kafka/RocketMQ API for easy switching; extended Kafka with delay queue support; non-invasive message subscription requiring no changes to business code; improved consumer throughput by 30% via manual batch offset commits and multi-threading

### Tax Bureau Real-Name Auth System – Architecture Optimization | Aug 2021 – Dec 2021
*Spring Boot, microservices, ClickHouse, Prometheus, Grafana, Arthas*

Identified strong coupling between business and technical code and response times exceeding 5 seconds on key interfaces. Led a full optimization initiative to improve performance, maintainability, and observability.

- Separated foundational technical code from core business logic, improving reusability and reducing maintenance cost
- Used Arthas flame graph analysis to pinpoint bottlenecks; improved overall system QPS by 30%+
- Developed a monitoring agent to collect system metrics; integrated Prometheus + Grafana for real-time dashboards and alerting
- Participated in replacing Elasticsearch with ClickHouse for API top-N analysis (by call volume and response time), reducing disk usage by 30% for the same data volume and retention period

## Education

- **Guangxi University for Nationalities** | Jan 2014 – Jul 2016: Bachelor of Science – Mathematics and Applied Mathematics
- **Guangxi University for Nationalities** | Sep 2008 – Jul 2011: Associate Degree – Software Technology

## Languages

- English: B2 (Early), actively studying
- Japanese: Beginner, actively studying
- Chinese: Native

## Certifications

- National Computer Rank Examination – Level 2, Aug 2009
- AWS Solutions Architect – Associate (SAA): In progress
