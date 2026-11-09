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
| Distributed & Middleware | Kafka, Redis, Nacos, Sentinel, Netty, RocketMQ, Redisson, Dubbo, Apollo, ShardingSphere |
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

### Workflow Orchestration Engine | Aug 2022 – Nov 2022
*Spring Boot, Redis, MQ, design patterns (Template, Strategy)*

A custom lightweight workflow orchestration engine, live in the enterprise finance and tax business line and hosting dozens of business workflow definitions.

- Owned the overall engine design and implemented its core, abstracting a unified node model with a create, run, and complete lifecycle
- Adapted the NodeHandler mechanism from MyBatis XMLScriptBuilder to register handlers by node type and build workflow definitions into executable node graphs; adding a node type only requires implementing the node and registering its handler
- Implemented conditional branch, loop, and asynchronous MQ nodes, plus workflow instance start, completion, failure retry, and restart with parameters
- Worked with colleagues to add scheduling, distributed locks, rate limiting, and HTTP, SQL, and sub-process nodes

### Tax Risk Indicator Calculation Engine | Aug 2022 – Nov 2022
*Spring Boot, multiple data sources, multi-threading, design patterns (Strategy, Template, Facade)*

Built a general-purpose risk indicator calculation engine to power tax risk detection and report generation, covering ~1,000 risk indicators across all business processes.

- Designed the engine using Strategy, Template, and Facade patterns, unifying SQL, Java API, and RESTful indicator executors
- Ran indicators concurrently in layers by processing order, with per-indicator failure retry and configurable thread count
- Implemented multi-data-source connection pooling, expression-based report risk scoring and grading, and indicator debugging and error monitoring
- Led code review to ensure code quality and team consistency

### Shein Export Tax Refund Invoice Management System | Jan 2022 – Jul 2022
*Spring Cloud, Kafka, Redis, MySQL, Jenkins, Kubernetes, Nacos*

Designed and built the data processing subsystem for a full end-to-end export business tracking system covering product storage, ordering, customs filing, delivery, invoicing, and tax refund. Processes 200M+ records per month.

- Designed batch-based processing to separate pending and processed data, avoiding direct large-table updates
- Split datasets by merchant dimension to keep each batch under 20M records; used Kafka + Kubernetes for horizontal scale-out
- Used Redis as intermediate storage to reduce MySQL write pressure; added validation metadata to ensure data integrity
- Resolved critical production issues: DB transaction timeouts, CPU spikes to 100%, Redis cache data loss

### Tax Bureau Real-Name Auth System – Architecture Optimization | Aug 2021 – Dec 2021
*Spring Boot, microservices, ClickHouse, Prometheus, Grafana, Arthas*

Identified strong coupling between business and technical code and response times exceeding 5 seconds on key interfaces. Led a full optimization initiative to improve performance, maintainability, and observability.

- Separated foundational technical code from core business logic, improving reusability and reducing maintenance cost
- Used Arthas flame graph analysis to pinpoint bottlenecks; improved overall system QPS by 30%+
- Developed a monitoring agent to collect system metrics; integrated Prometheus + Grafana for real-time dashboards and alerting
- Participated in replacing Elasticsearch with ClickHouse for API top-N analysis (by call volume and response time), reducing disk usage by 30% for the same data volume and retention period

### Cloud Configuration Center | May 2019 – Feb 2022
*Spring Boot, Apollo (customized), long polling, SM4*

A visual configuration center for regional configuration staff, developers, and delivery teams. Centrally manages feature switches, parameters, code tables, and service addresses across regions and environments, pushes published changes to applications in real time, and covers about 3 provinces.

- Owned the overall design; extended Apollo into a three-tier architecture of cloud admin console, regional configuration servers, and client SDK
- Implemented configuration distribution from the cloud to regional servers and real-time push to applications via long polling, with client hot reload
- Implemented configuration usage collection and regional data reporting, using batch submission to reduce call overhead
- Encrypted configuration transfer parameters with SM4; implemented batch configuration editing and publishing, and distributed-lock-protected configuration import
- Made the client compatible with JDK 7 and Spring Boot, lowering the cost of onboarding existing systems

### DRDS to ShardingSphere Sharding Migration Plan | Apr 2021 – Jul 2021
*Java, ShardingSphere-Proxy 5.0*

Researched migrating a business database with over 1 billion rows from Alibaba Cloud DRDS to ShardingSphere-Proxy (the migration did not go live).

- Studied ShardingSphere-Proxy source code for rule loading and the sharding flow to locate SPI extension points
- Built SPI-based sharding algorithms matching DRDS hash rules, handling database and table mapping when both share a sharding key, and supporting sharding by month and by day

### API Open Platform | Apr 2020 – Feb 2022
*Spring Boot, Elasticsearch, MySQL, Oracle, SpEL*

- Built API monitoring reports with response-time charts and API call details, with analysis by provider and consumer
- Built routing rule and degradation rule configuration and API import/export, with support for both MySQL and Oracle
- Data permission SDK: designed and built a configuration-driven data permission component that checks protected resources through interceptors and supports SpEL, SQL, and ID-conversion parameter parsing; works without a database or admin UI, integrates with minimal configuration, and can be extended for complex cases
- Migrated platform permissions to the in-house data permission SDK

### Guangdong Tax Bureau – Software Development Base Framework | Sep 2018 – Nov 2018
*Spring Boot, Maven, Kafka, RocketMQ, Redis, Elasticsearch*

Built a reusable foundational framework that won a government procurement contract with the Guangdong Provincial Tax Bureau and became the internal standard for all project teams.

- Logging middleware: supports delivery to Kafka, Redis, Elasticsearch, and ClickHouse; includes aggregation and statistics
- Messaging middleware: unified Kafka/RocketMQ API for easy switching; extended Kafka with delay queue support; non-invasive message subscription requiring no changes to business code; improved consumer throughput by 30% via manual batch offset commits and multi-threading

### E-commerce Refund Workflow | Aug 2017 – Aug 2018
*Spring Boot, Dubbo, MySQL*

- Developed refund application, buyer-seller negotiation, platform intervention, and automatic acceptance flows, plus order details and sales details features

## Education

- **Guangxi University for Nationalities** | Jan 2014 – Jul 2016: Bachelor of Science – Mathematics and Applied Mathematics
- **Guangxi University for Nationalities** | Sep 2008 – Jul 2011: Associate Degree – Software Technology

## Languages

- English: B2 (Early), actively studying
- Japanese: Beginner, actively studying
- Chinese: Native

## Certifications

- National Computer Rank Examination – Level 2, Aug 2009
