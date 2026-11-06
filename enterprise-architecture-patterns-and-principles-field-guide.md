<a id="top"></a>

<div align="center">

**THE ENTERPRISE ARCHITECTURE FIELD GUIDE**

# Patterns & Principles

### Clear boundaries. Deliberate trade-offs. Better outcomes.

A practical reference spanning **Business, Data, Application,<br>
Solution/Integration, Technology/Cloud, Security and Operational** architecture.

`16 CHAPTERS` · `7 ARCHITECTURE DOMAINS` · `2 COPYABLE TEMPLATES`

**[Explore the guide](#explore-the-guide)** · **[Choose a pattern](#16-pattern-selection-cheat-sheet)** · **[Review warning signs](#15-anti-patterns)** · **[Record a decision](#appendix-a-adr-template)**

</div>

---

> **✦ Architecture is a decision discipline**
>
> Start with the business outcome. Establish responsibilities and constraints.
> Compare credible options, explain the trade-offs and validate the difficult parts.

| 📖 A complete reference | 🎯 Built for practical use | 🧰 Ready to apply |
| :--- | :--- | :--- |
| Principles, patterns, frameworks and operational practices across the architecture lifecycle. | Scan the chapter introductions, compare the tables, then follow the relevant detail. | Pattern selection cheat sheet, ADR template and architecture principle template. |

<a id="explore-the-guide"></a>

## 🧭 Explore the guide

| **01 · FOUNDATIONS** | **02 · DESIGN & CONNECT** | **03 · DATA & PLATFORMS** |
| :--- | :--- | :--- |
| [Disciplines & frameworks](#1-architecture-disciplines--frameworks) | [Application patterns](#4-application-architecture-patterns) | [Data architecture](#8-data-architecture) |
| [Foundational principles](#2-foundational-principles) | [Domain-driven design](#5-domain-driven-design) | [Solution & technology](#9-solution--technology-architecture) |
| [Business architecture](#3-business-architecture) | [Integration & messaging](#6-integration--messaging-patterns) | [Cloud & migration](#10-cloud-architecture--migration) |
| **Business intent → clear boundaries** | [Distributed systems & resilience](#7-distributed-systems--resilience-patterns) | **Models → platforms → safe change** |

| **04 · RUN & ASSURE** | **05 · DECIDE & EVOLVE** | **06 · REUSABLE RESOURCES** |
| :--- | :--- | :--- |
| [Security architecture](#11-security-architecture) | [Governance & documentation](#14-architecture-governance--documentation) | [ADR template](#appendix-a-adr-template) |
| [Observability & operations](#12-observability--operations) | [Anti-patterns](#15-anti-patterns) | [Principle template](#appendix-b-architecture-principle-template-togaf-style) |
| [Quality attributes](#13-quality-attributes-nfrs) | [Pattern selection](#16-pattern-selection-cheat-sheet) | [Reference sources](#appendix-c-key-reference-sources) |
| **Trust → reliability → evidence** | **Decisions → feedback → improvement** | **Document what matters** |

### Pick your route

- **New to architecture?** Start with chapters 1–3, then explore the building blocks.
- **Designing a solution?** Start with chapter 16, consult the relevant pattern tables,
  and check security, operations and quality requirements before committing.
- **Reviewing an existing design?** Combine chapters 11–15 with the relevant domain chapters.
- **Leading change?** Use chapters 3, 9, 10 and 14 to connect outcomes, transition and decision rights.

These routes are navigation aids, not sequential delivery gates. Security, data
ownership, quality and operations should inform the design from the beginning.

<details>
<summary><strong>📚 Open the complete chapter index</strong></summary>

- [1. Architecture Disciplines & Frameworks](#1-architecture-disciplines--frameworks)
- [2. Foundational Principles](#2-foundational-principles)
- [3. Business Architecture](#3-business-architecture)
- [4. Application Architecture Patterns](#4-application-architecture-patterns)
- [5. Domain-Driven Design](#5-domain-driven-design)
- [6. Integration & Messaging Patterns](#6-integration--messaging-patterns)
- [7. Distributed Systems & Resilience Patterns](#7-distributed-systems--resilience-patterns)
- [8. Data Architecture](#8-data-architecture)
- [9. Solution & Technology Architecture](#9-solution--technology-architecture)
- [10. Cloud Architecture & Migration](#10-cloud-architecture--migration)
- [11. Security Architecture](#11-security-architecture)
- [12. Observability & Operations](#12-observability--operations)
- [13. Quality Attributes (NFRs)](#13-quality-attributes-nfrs)
- [14. Architecture Governance & Documentation](#14-architecture-governance--documentation)
- [15. Anti-Patterns](#15-anti-patterns)
- [16. Pattern Selection Cheat Sheet](#16-pattern-selection-cheat-sheet)
- [Appendix A: ADR Template](#appendix-a-adr-template)
- [Appendix B: Architecture Principle Template (TOGAF style)](#appendix-b-architecture-principle-template-togaf-style)
- [Appendix C: Key Reference Sources](#appendix-c-key-reference-sources)

</details>

### How to use this reference

> Notes on use
> - Patterns are trade-offs, not rules. Each entry lists *when to use* and *watch-outs*.
> - Well-known sources are named where the pattern has a clear origin (e.g. Evans, Fowler, Hohpe, Kimball).
> - "Architecture decisions" should be recorded as ADRs with context, options, decision, and consequences.


---

<a id="1-architecture-disciplines--frameworks"></a>

## 🏛️ 1. Architecture Disciplines & Frameworks

`CHAPTER 01` · `FOUNDATIONS`

Understand the disciplines before choosing a framework.


### 1.1 Disciplines

| Discipline | Focus | Typical deliverables |
|---|---|---|
| **Business Architecture** | Capabilities, value streams, org, strategy alignment | Capability map, value stream map, operating model |
| **Data Architecture** | Data models, flows, storage, governance, quality | Conceptual/logical/physical models, lineage, data catalogue |
| **Application Architecture** | Application structure, interactions, lifecycle | Application landscape, component/interface specs |
| **Technology / Infrastructure Architecture** | Platforms, networks, hosting, runtime | Reference architectures, landing zones, network design |
| **Solution Architecture** | End-to-end design of one solution across all domains | Solution design document, HLD, integration design |
| **Security Architecture** | Controls, identity, threat mitigation | Threat model, control mapping, security patterns |
| **Integration Architecture** | How systems exchange data and events | Integration catalogue, API standards, event model |
| **Enterprise Architecture** | Cross-cutting alignment of the above to strategy | Roadmaps, principles, standards, target state |

### 1.2 Frameworks & Standards

- **TOGAF** (The Open Group): ADM phases (Preliminary, A Vision, B Business, C Information Systems [Data/Application], D Technology, E Opportunities & Solutions, F Migration Planning, G Implementation Governance, H Change Management, Requirements Management at centre).
- **Zachman Framework**: classification schema (What/How/Where/Who/When/Why × perspectives).
- **ArchiMate** (The Open Group): modelling language with Business, Application, Technology layers plus Motivation, Strategy, Implementation & Migration.
- **C4 Model** (Simon Brown): Context, Container, Component, Code.
- **arc42**: architecture documentation template.
- **4+1 View Model** (Kruchten): logical, process, development, physical, scenarios.
- **BIAN** (Banking Industry Architecture Network): service landscape for banking.
- **ITIL / COBIT**: service management and IT governance.
- **DAMA-DMBOK**: data management body of knowledge.
- **FEAF / DoDAF**: government architecture frameworks.
- **Well-Architected Frameworks**: AWS (six pillars: Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, Sustainability), Azure (five pillars), Google Cloud Architecture Framework.
- **ATAM** (SEI): Architecture Tradeoff Analysis Method for evaluating architecture against quality attributes.

> **💡 Decision takeaway**
>
> Choose the viewpoint that answers the stakeholder's question. Frameworks organise the work; they do not make the decisions.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 2. Foundational Principles →](#2-foundational-principles)**

---

<a id="2-foundational-principles"></a>

## 🧭 2. Foundational Principles

`CHAPTER 02` · `FOUNDATIONS`

Build a common language for architecture decisions.


### 2.1 Enterprise-Level Principles (TOGAF style: Name, Statement, Rationale, Implications)

| Principle | Statement |
|---|---|
| **Business value first** | Architecture decisions trace to business outcomes and strategy. |
| **Business continuity** | Operations must survive failures, outages, and change. |
| **Data is an asset** | Data is managed, owned, governed, and shared across the enterprise. |
| **Data is shared and accessible** | Avoid silos; provide controlled access to authoritative data. |
| **Common vocabulary and definitions** | Consistent business terms (glossary, canonical definitions). |
| **Single source of truth / system of record** | Each data element has one authoritative source. |
| **Reuse before buy, buy before build** | Prefer existing capability, then commercial/SaaS, then custom for differentiation. |
| **Technology independence** | Avoid unnecessary lock-in; abstract where the cost is justified. |
| **Interoperability** | Use open standards and well-defined interfaces. |
| **Compliance with law and policy** | Regulatory (e.g. privacy, financial regulation) is designed in. |
| **Security by design** | Security is built in, not bolted on. |
| **Simplicity** | Reduce complexity and moving parts; manage technical diversity. |
| **Responsive change management** | Architecture enables incremental, safe change. |
| **Ease of use** | Reduce friction for customers, staff, and developers. |
| **Accountability / ownership** | Every asset (app, data, API) has a named owner. |

### 2.2 Software Design Principles

- **SOLID** (Robert C. Martin)
  - **S**ingle Responsibility
  - **O**pen/Closed
  - **L**iskov Substitution
  - **I**nterface Segregation
  - **D**ependency Inversion
- **Separation of Concerns**
- **High Cohesion, Low Coupling**
- **DRY** (Don't Repeat Yourself), balanced against the cost of wrong abstraction ("duplication is cheaper than the wrong abstraction")
- **KISS** and **YAGNI**
- **Law of Demeter** (principle of least knowledge)
- **Composition over Inheritance**
- **Encapsulation / Information Hiding** (Parnas)
- **Principle of Least Astonishment**
- **Fail Fast**
- **Convention over Configuration**
- **Tell, Don't Ask**
- **Postel's Law / Robustness Principle**: be conservative in what you send, liberal in what you accept (apply carefully; can mask errors).
- **Idempotency** by design for operations that may be retried.
- **Design for failure** ("everything fails all the time").
- **Evolutionary architecture** (Ford, Parsons, Kua): fitness functions guide incremental change.
- **Last Responsible Moment**: delay irreversible decisions until needed information is available.
- **Conway's Law**: system structure mirrors communication structure; use the *Inverse Conway Manoeuvre* to shape teams for the desired architecture.

### 2.3 Application & Service Principles

- **Twelve-Factor App** (Heroku): codebase, dependencies, config, backing services, build/release/run, processes, port binding, concurrency, disposability, dev/prod parity, logs, admin processes.
- **API-first / contract-first** design.
- **Loose coupling, autonomy of services**
- **Statelessness** where possible; externalise state.
- **Smart endpoints, dumb pipes** (microservices guidance).
- **You build it, you run it** (team ownership across lifecycle).
- **Decentralised data management** (each service owns its data).
- **Backward compatibility and versioning discipline** for contracts.
- **Automate everything** (build, test, deploy, infra).
- **Immutable infrastructure**.
- **Infrastructure as Code**.
- **Shift-left** (testing, security, cost).

### 2.4 Data Principles

- **Data ownership and stewardship** (clear owners and stewards).
- **Data quality at source**.
- **Data minimisation and purpose limitation** (privacy).
- **Metadata is first-class** (catalogue, lineage, classification).
- **Data as a product** (Data Mesh).
- **FAIR** (Findable, Accessible, Interoperable, Reusable).
- **Schema evolution with compatibility rules**.
- **Separate operational from analytical workloads**.
- **Single definition of key business entities** (master data).
- **Retention and lifecycle management**.

### 2.5 Business Architecture Principles

- **Capability-based planning**: plan around *what* the business does, not org charts.
- **Value stream orientation**: align to end-to-end value delivery.
- **Customer-centricity**.
- **Business/IT alignment** through shared language (capabilities, value streams).
- **Stable capabilities, volatile implementations**: capabilities change slowly; applications and org structures change quickly.

> **💡 Decision takeaway**
>
> Treat principles as decision guides. Record the rationale, implications and any justified exception.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 3. Business Architecture →](#3-business-architecture)**

---

<a id="3-business-architecture"></a>

## 🎯 3. Business Architecture

`CHAPTER 03` · `FOUNDATIONS`

Connect strategy to capabilities, value streams and ownership.


### 3.1 Core Constructs (BIZBOK-aligned)

- **Capability map**: hierarchical model of what the business does (Level 1 to 3). Heatmap by maturity, investment, risk, strategic importance.
- **Value streams**: end-to-end stages that deliver value to a stakeholder (e.g. Acquire Customer, Open Account, Resolve Dispute).
- **Value stream to capability mapping**: which capabilities enable which stages.
- **Organisation map**: structure, roles, locations.
- **Information map**: business concepts and relationships (conceptual data view).
- **Business Process models** (BPMN), process hierarchy.
- **Stakeholder and customer journey maps**.
- **Business Motivation Model**: Vision, Goals, Objectives, Strategies, Tactics, Drivers, Assessments.
- **Operating model**: how capabilities are organised, governed, sourced (centralised, federated, hub-and-spoke, shared services).
- **Business Model Canvas / Strategy Map / Balanced Scorecard** for strategy articulation.
- **Wardley Mapping**: evolution of components (Genesis, Custom, Product, Commodity) to inform build/buy/outsource.

### 3.2 Business Architecture Patterns

| Pattern | Description |
|---|---|
| **Capability-based planning** | Fund and roadmap by capability uplift, not project lists. |
| **Capability-to-application mapping** | Rationalise duplicated apps supporting the same capability. |
| **Shared services** | Consolidate common capabilities (HR, finance, KYC) for reuse. |
| **Platform business model** | Provide a platform enabling third-party value (e.g. open banking). |
| **Product-aligned organisation** | Stable cross-functional teams owning products/value streams. |
| **Team Topologies** (Skelton & Pais) | Stream-aligned, Platform, Enabling, Complicated-subsystem teams; three interaction modes (collaboration, X-as-a-Service, facilitation). |
| **Centre of Excellence / Community of Practice** | Spread expertise without central bottlenecks. |
| **Federated governance** | Central guardrails, local autonomy. |
| **Strangler transformation** | Replace legacy capability incrementally rather than big bang. |
| **Core / Context** (Geoffrey Moore) | Invest in differentiating *core*; standardise or buy *context*. |
| **Pace-layered architecture** (Gartner) | Systems of Record (slow), Systems of Differentiation (medium), Systems of Innovation (fast). |
| **Bimodal / multi-speed IT** | Different governance and cadence by layer (use with care; avoid creating a two-class system). |

### 3.3 Typical Banking / Financial Services Capability Domains (illustrative)

Customer Management, Product Management, Account Management, Payments, Lending, Deposits, Cards, Treasury, Risk & Compliance (AML/KYC/Fraud), Finance & Reporting, Channel Management, Collections, Disputes, Regulatory Reporting, Data & Analytics, Enterprise Services (HR, Procurement, IT).

> **💡 Decision takeaway**
>
> Use capabilities to explain what the business needs to do, then examine which processes and systems enable it.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 4. Application Architecture Patterns →](#4-application-architecture-patterns)**

---

<a id="4-application-architecture-patterns"></a>

## 🧩 4. Application Architecture Patterns

`CHAPTER 04` · `DESIGN & CONNECT`

Compare structural patterns against the needs of the application.


### 4.1 Structural / Layering Patterns

| Pattern | Summary | Use when | Watch-outs |
|---|---|---|---|
| **Layered (N-tier)** | Presentation, Business, Data Access, Database | Simple to moderate apps, clear separation | Layer leakage, "sinkhole" pass-through layers |
| **Hexagonal (Ports & Adapters)** (Cockburn) | Core domain surrounded by ports; adapters for UI, DB, messaging | Testability, tech independence | More upfront structure |
| **Onion Architecture** (Palermo) | Domain at centre; dependencies point inward | Domain-heavy systems | Same as hexagonal |
| **Clean Architecture** (R. Martin) | Entities, Use Cases, Interface Adapters, Frameworks; dependency rule | Long-lived business logic | Over-engineering for CRUD |
| **Modular Monolith** | Single deployable with strict module boundaries | Most teams starting out; avoids distributed complexity | Needs enforced boundaries (e.g. architectural tests) |
| **Monolith** | Single codebase and deployable | Small teams, early stage | Scaling teams and deployment coupling |
| **Microservices** | Independently deployable services around business capabilities | Large orgs, independent scaling and release | Operational complexity, distributed data, network failure modes |
| **Service-Oriented Architecture (SOA)** | Coarse services, often with ESB, shared contracts | Enterprise integration legacy | Centralised bottleneck ESB, heavyweight governance |
| **Micro-frontends** | Compose UI from independently deployed frontends | Large frontend with multiple teams | Consistency, performance, shared dependencies |
| **Backend for Frontend (BFF)** (Newman) | Dedicated backend per client type | Differing channel needs (web, mobile, partner) | Duplication across BFFs |
| **API Gateway** | Single entry: routing, auth, rate limiting, aggregation | Many services behind one façade | Becoming a monolithic bottleneck |
| **Model-View-Controller (MVC) / MVP / MVVM** | UI separation patterns | UI applications | Fat controllers/view models |
| **Plugin / Microkernel** | Minimal core with extensible plug-ins | Product platforms, IDE-like systems | Plugin contract stability |
| **Pipe and Filter** | Data flows through processing stages | ETL, stream processing, compilers | Error handling across stages |
| **Blackboard** | Shared knowledge store with specialist components | Non-deterministic problems (AI-like) | Complexity, rare in enterprise |
| **Client-Server / Peer-to-Peer** | Basic distribution topologies | Foundational | n/a |
| **Serverless / FaaS** | Event-driven functions, managed runtime | Spiky workloads, glue logic | Cold starts, vendor coupling, observability |
| **Cell-based architecture** | Independent, replicated cells isolating blast radius | High-scale, high-resilience | Routing layer complexity |
| **Sidecar / Service Mesh** | Cross-cutting concerns (mTLS, retries, telemetry) moved to a proxy | Many microservices | Operational overhead |
| **Ambassador / Adapter** | Proxy for outbound calls / interface translation | Legacy integration | Extra hop |

### 4.2 Architectural Styles by Interaction

- **Request/Response (synchronous)**: REST, gRPC, GraphQL, SOAP.
- **Event-Driven Architecture (EDA)**: producers emit events; consumers react asynchronously.
- **Message-Driven**: commands/messages via queues.
- **Publish/Subscribe**: topic-based fan-out.
- **Streaming**: continuous event/data processing (e.g. Kafka-style logs).
- **Batch**: scheduled bulk processing.
- **Hybrid**: sync front, async back-end processing.

### 4.3 API Styles & Practices

| Style | Strengths | Considerations |
|---|---|---|
| **REST** | Ubiquitous, cacheable, resource-oriented | Over/under-fetching; use maturity model (Richardson) pragmatically |
| **GraphQL** | Client-defined queries, single endpoint | Caching, authorisation granularity, query cost control |
| **gRPC** | Efficient binary (HTTP/2, protobuf), strong contracts, streaming | Browser support, human readability |
| **Async APIs (AsyncAPI)** | Document event-driven interfaces | Governance of event schemas |
| **Webhooks** | Push notifications to external parties | Retry, signing, replay, security |
| **SOAP/WSDL** | Strong contracts, WS-* standards | Verbosity, legacy |

API practices: contract-first (OpenAPI), consistent naming, pagination, filtering, idempotency keys, versioning strategy (URI, header, or evolutionary/additive), error model (e.g. RFC 9457 Problem Details), rate limiting, deprecation policy, API lifecycle management, consumer-driven contract tests (e.g. Pact), API product thinking, API catalogue/portal.

### 4.4 Core Design Patterns Relevant at Architecture Level

- **Repository**, **Unit of Work**, **Data Mapper**, **Active Record** (Fowler, PoEAA).
- **Service Layer**, **Domain Model**, **Transaction Script**, **Table Module**.
- **Factory**, **Builder**, **Singleton** (use sparingly), **Dependency Injection**, **Service Locator** (generally discouraged).
- **Strategy**, **Observer**, **Decorator**, **Adapter**, **Facade**, **Proxy**, **Command**, **Chain of Responsibility**, **State**, **Template Method** (GoF).
- **Specification**, **Anti-Corruption Layer**, **Gateway**, **Mapper**, **DTO**, **Value Object**, **Aggregate**.
- **Feature Toggles**, **Branch by Abstraction**, **Parallel Run**, **Dark Launching**.

> **💡 Decision takeaway**
>
> Start with clear module boundaries. Introduce distribution when independent ownership, deployment or scale justifies the cost.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 5. Domain-Driven Design →](#5-domain-driven-design)**

---

<a id="5-domain-driven-design"></a>

## 📐 5. Domain-Driven Design

`CHAPTER 05` · `DESIGN & CONNECT`

Keep domain meaning and consistency boundaries explicit.


### 5.1 Strategic Design (Evans)

- **Domain / Subdomain**: Core, Supporting, Generic.
- **Bounded Context**: explicit boundary where a model and ubiquitous language apply.
- **Ubiquitous Language**: shared vocabulary between business and engineering within a context.
- **Context Map** relationships:
  - **Partnership**
  - **Shared Kernel**
  - **Customer/Supplier**
  - **Conformist**
  - **Anti-Corruption Layer (ACL)**
  - **Open Host Service**
  - **Published Language**
  - **Separate Ways**
  - **Big Ball of Mud** (recognised, to be contained)
- **Event Storming** (Brandolini): collaborative discovery of events, commands, aggregates, policies, bounded contexts.

### 5.2 Tactical Design

- **Entity**, **Value Object**, **Aggregate** (consistency boundary, one root), **Aggregate Root**
- **Domain Service**, **Application Service**
- **Domain Event**, **Integration Event**
- **Repository**, **Factory**
- **Module**

### 5.3 Guidance

- Aim microservice boundaries at bounded contexts, not at entities or tables.
- Keep aggregates small; reference other aggregates by identity.
- Use eventual consistency between aggregates and contexts.

> **💡 Decision takeaway**
>
> Use bounded contexts to protect meaning and aggregates to protect invariants. Neither should be inferred from database tables alone.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 6. Integration & Messaging Patterns →](#6-integration--messaging-patterns)**

---

<a id="6-integration--messaging-patterns"></a>

## 🔗 6. Integration & Messaging Patterns

`CHAPTER 06` · `DESIGN & CONNECT`

Design contracts, message flows and delivery semantics deliberately.


### 6.1 Integration Styles (Hohpe & Woolf, *Enterprise Integration Patterns*)

1. **File Transfer**
2. **Shared Database** (generally an anti-pattern across systems)
3. **Remote Procedure Invocation**
4. **Messaging**

### 6.2 Messaging Patterns (selected from EIP)

| Category | Patterns |
|---|---|
| **Message types** | Command Message, Document Message, Event Message, Request-Reply |
| **Channels** | Point-to-Point Channel, Publish-Subscribe Channel, Dead Letter Channel, Datatype Channel, Guaranteed Delivery, Invalid Message Channel |
| **Routing** | Content-Based Router, Message Filter, Recipient List, Splitter, Aggregator, Resequencer, Scatter-Gather, Routing Slip, Process Manager, Message Broker |
| **Transformation** | Message Translator, Envelope Wrapper, Content Enricher, Content Filter, Claim Check, Normalizer, Canonical Data Model |
| **Endpoints** | Polling Consumer, Event-Driven Consumer, Competing Consumers, Message Dispatcher, Selective Consumer, Durable Subscriber, **Idempotent Receiver**, Service Activator, Messaging Gateway |
| **Management** | Control Bus, Detour, Wire Tap, Message History, Message Store, Smart Proxy, Test Message |

### 6.3 Integration Architecture Patterns

- **Point-to-Point** (does not scale; N×(N-1)/2 connections).
- **Hub-and-Spoke / ESB**: central mediation; risk of central bottleneck and logic sprawl.
- **Event Backbone / Event Mesh**: distributed event distribution.
- **API-led connectivity** (System, Process, Experience API layers).
- **Canonical Data Model**: reduces translations but risks lowest-common-denominator coupling; apply per domain or use published languages.
- **Anti-Corruption Layer**: isolate from legacy/external models.
- **Strangler Fig** (Fowler): route traffic progressively to a new system behind a façade.
- **Change Data Capture (CDC)**: stream DB changes as events (log-based preferred).
- **Transactional Outbox**: write business data and outbox record atomically, publish asynchronously.
- **Inbox / Idempotent Consumer**: deduplicate on receipt.
- **Event Notification vs Event-Carried State Transfer vs Event Sourcing** (Fowler's event taxonomy).
- **Claim Check**: store large payload externally, pass reference.
- **Managed File Transfer (MFT)** for batch partner exchange.
- **iPaaS**: cloud-hosted integration platform.
- **B2B / EDI** gateways.
- **Open Banking / Open APIs** for third-party access.

### 6.4 Event-Driven Specifics

- **Event Sourcing**: persist state as an append-only sequence of events; rebuild by replay.
- **CQRS** (Greg Young): separate command (write) and query (read) models.
- **Event schema management**: schema registry, compatibility modes (backward, forward, full).
- **Ordering and partitioning**: ordering guaranteed only within a partition/key.
- **Delivery semantics**: at-most-once, at-least-once, effectively-once (idempotent processing plus transactional guarantees). True exactly-once end-to-end requires care.
- **Replay and retention** policies; **compacted topics** for latest-state.
- **Dead-letter and retry topics**, poison message handling.
- **Choreography vs Orchestration**: decentralised events vs central coordinator.

> **💡 Decision takeaway**
>
> Reliable integration needs more than a broker: define ownership, compatibility, duplicates, ordering, replay and recovery.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 7. Distributed Systems & Resilience Patterns →](#7-distributed-systems--resilience-patterns)**

---

<a id="7-distributed-systems--resilience-patterns"></a>

## 🛟 7. Distributed Systems & Resilience Patterns

`CHAPTER 07` · `DESIGN & CONNECT`

Make partial failure, scaling and recovery visible in the design.


### 7.1 Theory and Trade-offs

- **CAP theorem** (Brewer): under network partition, choose consistency or availability.
- **PACELC** (Abadi): else (no partition), latency vs consistency.
- **ACID vs BASE**.
- **Consistency models**: strong/linearizable, sequential, causal, read-your-writes, eventual.
- **Fallacies of distributed computing** (Deutsch): network is reliable, latency is zero, bandwidth infinite, network secure, topology static, one administrator, transport cost zero, network homogeneous.
- **Idempotency**, **at-least-once delivery**, **exactly-once myth**.
- **Consensus**: Paxos, Raft.
- **Clocks**: logical/vector clocks; do not rely on wall-clock ordering across nodes.

### 7.2 Distributed Transaction Patterns

| Pattern | Notes |
|---|---|
| **Two-Phase Commit (2PC / XA)** | Strong atomicity, blocking, poor availability; avoid across services where possible |
| **Saga** (Garcia-Molina & Salem) | Sequence of local transactions with **compensating actions**; orchestration or choreography |
| **TCC (Try-Confirm/Cancel)** | Reserve, then confirm or cancel |
| **Transactional Outbox** | Reliable event publication |
| **Idempotent consumer** | Safe retries |
| **Eventual consistency with reconciliation** | Periodic comparison and repair, common in financial systems |

### 7.3 Resilience Patterns (Nygard, *Release It!* and others)

- **Timeouts** (always set; budget across call chains)
- **Retries with exponential backoff and jitter** (only for idempotent/safe operations)
- **Circuit Breaker**
- **Bulkhead** (isolate resources/pools)
- **Rate Limiting / Throttling / Load Shedding**
- **Backpressure**
- **Fallback / Graceful Degradation**
- **Cache-aside / Stale-while-revalidate** for resilience
- **Health Endpoint Monitoring**, readiness/liveness probes
- **Leader Election**
- **Failover** (active-passive), **Active-Active**
- **Redundancy / N+1**
- **Chaos Engineering** (verify resilience through controlled failure)
- **Steady State** (purge/rotate data, logs, sessions)
- **Compensating Transaction**
- **Queue-Based Load Leveling**
- **Competing Consumers**
- **Priority Queue**
- **Throttling per tenant** (noisy-neighbour control)

### 7.4 Scalability Patterns

- **Horizontal vs vertical scaling**
- **Stateless services + externalised session**
- **Sharding / Partitioning** (hash, range, directory/geo)
- **Read replicas**
- **Caching** layers: client, CDN, edge, API gateway, application, distributed cache, DB cache
- **Cache strategies**: cache-aside, read-through, write-through, write-behind; invalidation (TTL, event-based)
- **CDN / Edge computing**
- **Async processing and queues**
- **Materialised views / precomputed read models**
- **Autoscaling** (reactive, scheduled, predictive)
- **Multi-tenancy models**: silo, pool, bridge (hybrid)
- **Cell-based / shuffle sharding** for blast radius reduction
- **Consistent hashing**

### 7.5 Disaster Recovery Strategies

| Strategy | RTO / RPO | Cost |
|---|---|---|
| **Backup & Restore** | Hours / hours | Lowest |
| **Pilot Light** | Tens of minutes to hours | Low |
| **Warm Standby** | Minutes | Medium |
| **Multi-Site Active-Active** | Near zero | Highest |

Define **RTO** (recovery time objective), **RPO** (recovery point objective), **MTD**, and test DR regularly.

> **💡 Decision takeaway**
>
> Retries, failover and replication have consequences. Validate their behaviour under realistic failures and overload.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 8. Data Architecture →](#8-data-architecture)**

---

<a id="8-data-architecture"></a>

## 🗄️ 8. Data Architecture

`CHAPTER 08` · `DATA & PLATFORMS`

Choose models and stores from business meaning and access patterns.


### 8.1 Data Modelling Levels

- **Conceptual** (business entities and relationships)
- **Logical** (attributes, keys, normalised or dimensional, technology-neutral)
- **Physical** (tables, indexes, partitions, storage specifics)

### 8.2 Data Store Types & When to Use

| Type | Examples (category only) | Best for |
|---|---|---|
| **Relational (RDBMS)** | SQL databases | Transactions, integrity, complex queries |
| **Document** | JSON document stores | Flexible schema, aggregate-oriented access |
| **Key-Value** | In-memory/KV stores | Caching, sessions, simple lookups |
| **Wide-Column** | Column-family stores | Massive write scale, time-series-like access patterns |
| **Graph** | Property graph / RDF stores | Relationship-heavy queries (fraud rings, lineage, knowledge graphs) |
| **Time-Series** | TSDBs | Metrics, IoT, telemetry |
| **Search** | Inverted-index engines | Full-text, faceting, log search |
| **Columnar / MPP warehouse** | Cloud data warehouses | Analytical SQL |
| **Object / Blob storage** | Object stores | Data lake, files, archives |
| **Vector** | Vector databases/indexes | Embedding similarity (AI/RAG) |
| **Ledger** | Immutable/ledger databases | Auditable append-only records |
| **NewSQL / Distributed SQL** | Horizontally scalable SQL | Global scale with SQL semantics |

**Polyglot persistence**: use the right store per workload, balanced against operational cost.

### 8.3 Operational Data Patterns

- **Database per service** (microservices)
- **Shared database** (anti-pattern across bounded contexts)
- **CQRS** read/write separation
- **Event Sourcing**
- **Materialised View**
- **Command Query Separation**
- **Outbox / CDC**
- **Sharding, partitioning, replication** (single-leader, multi-leader, leaderless)
- **Optimistic vs pessimistic locking**
- **Soft delete, temporal tables, bi-temporal modelling** (valid-time vs transaction-time; important for finance and audit)
- **Slowly Changing Dimensions** (Types 0 to 7; see below)
- **Reference data management**
- **Master Data Management (MDM)** styles: Registry, Consolidation, Coexistence, Centralised (Transaction)
- **Golden record / survivorship rules**
- **Data virtualisation / federation**
- **Archival and tiered storage**
- **Idempotent upserts / merge**

### 8.4 Analytical Architecture Patterns

| Pattern | Summary | Notes |
|---|---|---|
| **Enterprise Data Warehouse (Inmon)** | Centralised, normalised (3NF) EDW feeding marts | Strong integration, slower delivery |
| **Dimensional / Kimball Bus Architecture** | Conformed dimensions and facts (star schemas) | Business-friendly, fast queries |
| **Data Vault (Linstedt)** | Hubs, Links, Satellites; auditable, agile loading | Good for integration and history; needs presentation layer |
| **Data Lake** | Raw data in object storage, schema-on-read | Risk of "data swamp" without governance |
| **Lakehouse** | Warehouse capabilities (ACID, schema, governance) on lake storage via open table formats | Unifies BI and ML workloads |
| **Medallion (Bronze/Silver/Gold)** | Progressive refinement layers (raw, cleansed/conformed, curated/business) | Common lakehouse layering |
| **Lambda Architecture** (Marz) | Batch layer + speed layer + serving layer | Duplicate logic burden |
| **Kappa Architecture** (Kreps) | Single streaming pipeline, replay for reprocessing | Requires mature streaming |
| **Data Mesh** (Dehghani) | Domain ownership, data as a product, self-serve platform, federated computational governance | Organisational change heavy; needs platform maturity |
| **Data Fabric** | Metadata-driven, automated integration and governance layer | Vendor/vision dependent |
| **Data Hub** | Mediation point for sharing and governance | Variation in definitions |
| **Operational Data Store (ODS)** | Integrated near-real-time operational view | Often feeds DW |
| **Reverse ETL / Operational analytics** | Push analytical outputs back into operational tools | Governance of write-back |
| **Feature Store** | Shared, consistent ML features for training and serving | MLOps component |
| **Semantic Layer / Metrics Layer** | Governed business metrics definitions | Prevents metric drift |

### 8.5 Data Integration & Pipeline Patterns

- **ETL vs ELT** (ELT prevalent with scalable warehouses/lakehouses)
- **Batch, micro-batch, streaming**
- **Incremental loads**: watermark/high-water mark, CDC, snapshot diff
- **Full refresh vs incremental vs append-only**
- **Idempotent, re-runnable pipelines**
- **Backfill and reprocessing strategy**
- **Schema evolution handling** (add-only changes, registry, contracts)
- **Data contracts** between producers and consumers
- **Orchestration** (DAG-based workflow) vs **choreography** (event-triggered)
- **Dead-letter / quarantine tables** for bad records
- **Reconciliation and control totals** (row counts, hash totals, balancing) are essential in financial data
- **Partitioning and clustering** strategies for performance and cost
- **Late-arriving data and out-of-order events** (watermarks, windowing)
- **Windowing**: tumbling, hopping/sliding, session
- **Exactly-once semantics via idempotent sinks / transactional writes**

### 8.6 Dimensional Modelling Essentials (Kimball)

- **Fact table types**: Transaction, Periodic Snapshot, Accumulating Snapshot, Factless.
- **Dimension types**: Conformed, Role-playing, Junk, Degenerate, Outrigger, Mini-dimension.
- **Grain**: declare it first.
- **Slowly Changing Dimensions**:
  - Type 0: retain original
  - Type 1: overwrite
  - Type 2: add new row (history with effective dates / current flag)
  - Type 3: add new column (previous value)
  - Type 4: mini-dimension / history table
  - Type 6: hybrid (1+2+3)
  - Type 7: dual type 1 and 2
- **Surrogate keys**, **additive / semi-additive / non-additive measures**.
- **Bus matrix** for conformed design.

### 8.7 Data Governance & Management (DAMA-DMBOK knowledge areas)

Data Governance, Data Architecture, Data Modelling & Design, Data Storage & Operations, Data Security, Data Integration & Interoperability, Document & Content Management, Reference & Master Data, Data Warehousing & BI, Metadata Management, Data Quality.

Key practices:
- **Roles**: Data Owner, Data Steward, Data Custodian, Data Product Owner, Chief Data Officer.
- **Data catalogue and business glossary**.
- **Data lineage** (technical and business; column-level where feasible).
- **Data classification** (public, internal, confidential, restricted) and handling rules.
- **Data quality dimensions**: accuracy, completeness, consistency, timeliness, validity, uniqueness.
- **Data quality rules, monitoring, and SLAs/SLOs**.
- **Retention, archival, deletion** per policy and regulation.
- **Privacy**: consent, purpose limitation, minimisation, subject access, right to erasure, cross-border transfer; masking, tokenisation, pseudonymisation, anonymisation; differential privacy where relevant.
- **Access control**: RBAC, ABAC, row-level and column-level security, dynamic masking.
- **Data sharing** agreements and clean-room patterns.
- **Data observability**: freshness, volume, schema, distribution, lineage.

### 8.8 AI/ML Data & Architecture Patterns

- **MLOps**: versioned data/features/models, CI/CD for ML, model registry, monitoring for drift.
- **Online vs offline feature serving**.
- **Retrieval-Augmented Generation (RAG)**: retrieve relevant context (vector/keyword/hybrid search) and supply to an LLM.
- **Guardrails, evaluation harnesses, human-in-the-loop**.
- **Model governance**: lineage, explainability, bias monitoring, approvals.
- **AI gateway** pattern: central policy, logging, cost control for model access.
- **Agentic patterns**: tool use, planner/executor, multi-agent orchestration (apply with strong controls).

> **💡 Decision takeaway**
>
> Make data ownership, quality, freshness and lifecycle explicit before selecting a platform or creating another copy.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 9. Solution & Technology Architecture →](#9-solution--technology-architecture)**

---

<a id="9-solution--technology-architecture"></a>

## ⚙️ 9. Solution & Technology Architecture

`CHAPTER 09` · `DATA & PLATFORMS`

Connect solution responsibilities to deployment, change and support.


### 9.1 Solution Architecture Deliverables

- Context and scope, assumptions, constraints, risks, dependencies
- Requirements: functional, NFRs, regulatory
- Options analysis and decision record (ADR)
- Logical and physical views (C4 / ArchiMate)
- Integration and data flows
- Security and compliance design
- Deployment and operations model
- Migration/cutover and rollback plan
- Cost estimate (CapEx/OpEx, run cost)
- Test and quality strategy
- Handover to support

### 9.2 Deployment & Release Patterns

| Pattern | Summary |
|---|---|
| **Blue/Green** | Two identical environments; switch traffic |
| **Canary** | Gradual rollout to a subset, observe, expand |
| **Rolling** | Replace instances progressively |
| **Recreate** | Stop old, start new (downtime) |
| **A/B Testing** | Experiment variants for behaviour |
| **Feature Flags / Toggles** | Decouple deploy from release |
| **Shadow / Dark Launch / Traffic Mirroring** | Test with real traffic, no user impact |
| **Parallel Run** | Old and new systems run concurrently for reconciliation (common in core banking migration) |
| **Expand/Contract (Parallel Change)** | Safe schema and API evolution |
| **Branch by Abstraction** | Replace implementation behind an interface |
| **Trunk-Based Development** | Short-lived branches, continuous integration |
| **GitOps** | Git as source of truth for declarative infra/app state |
| **Progressive Delivery** | Canary + flags + automated analysis |

### 9.3 Infrastructure & Platform Patterns

- **Infrastructure as Code** (declarative), **immutable infrastructure**, **policy as code**
- **Landing Zone / Hub-and-Spoke network**
- **Multi-account / multi-subscription strategy** (isolation by environment, workload, or compliance)
- **Zero-trust networking**, private connectivity, segmentation
- **Containers and orchestration** (Kubernetes concepts: pods, deployments, services, ingress, operators)
- **Service Mesh**
- **Platform Engineering / Internal Developer Platform (IDP)**: golden paths, self-service, paved roads
- **Environment strategy**: dev, test, staging, prod; ephemeral environments
- **Configuration and secrets management** (externalised, rotated)
- **Artifact repositories, SBOM, supply-chain security** (signing, provenance)
- **FinOps**: tagging, showback/chargeback, budgets, rightsizing, commitment discounts
- **Tagging strategy**: ownership, cost centre, environment, data classification, application, criticality (enables governance and cost allocation)
- **High availability topologies**: multi-AZ, multi-region
- **Edge / hybrid / multi-cloud / sovereign cloud** (regulatory and data residency driven)

### 9.4 Legacy Modernisation Patterns

- **Strangler Fig**
- **Anti-Corruption Layer**
- **Branch by Abstraction**
- **Parallel Run / Shadow Running**
- **Event Interception** (capture legacy events via CDC or interception to feed new services)
- **Legacy mimic / façade API**
- **Data migration patterns**: big-bang, phased (by customer cohort, product, or account), trickle migration with synchronisation, reconciliation, dual-write (use cautiously; prefer CDC/outbox)
- **Decomposition by capability / bounded context**
- **Asset capture** and **Replatform vs Rearchitect** decisions (see 10.2)

> **💡 Decision takeaway**
>
> A solution is not complete at the component diagram. Include safe migration, operating ownership, cost and handover.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 10. Cloud Architecture & Migration →](#10-cloud-architecture--migration)**

---

<a id="10-cloud-architecture--migration"></a>

## ☁️ 10. Cloud Architecture & Migration

`CHAPTER 10` · `DATA & PLATFORMS`

Match cloud and migration choices to workload and organisational needs.


### 10.1 Service Models & Principles

- **IaaS, PaaS, SaaS, FaaS, CaaS, DBaaS**
- **Shared responsibility model**
- **Cloud-native**: containers, microservices, declarative APIs, managed services, automation
- **Design for elasticity and pay-per-use**
- **Prefer managed services** to reduce undifferentiated heavy lifting (balanced against lock-in)
- **Region and availability zone design**; data residency and sovereignty
- **Landing zone governance**: guardrails, policies, identity, networking, logging baseline

### 10.2 Migration Strategies ("Rs")

Commonly cited (Gartner 5 Rs, AWS 6/7 Rs): **Rehost** (lift-and-shift), **Replatform** (lift-tinker-shift), **Repurchase** (move to SaaS), **Refactor / Re-architect**, **Retire**, **Retain** (revisit later), **Relocate** (hypervisor-level move).

### 10.3 Well-Architected Pillars (cross-vendor synthesis)

1. **Operational Excellence**
2. **Security**
3. **Reliability**
4. **Performance Efficiency**
5. **Cost Optimisation**
6. **Sustainability**

### 10.4 Cloud Design Patterns (selected, e.g. Microsoft Cloud Design Patterns catalogue)

Ambassador, Anti-Corruption Layer, Asynchronous Request-Reply, Backends for Frontends, Bulkhead, Cache-Aside, Choreography, Circuit Breaker, Claim Check, Compensating Transaction, Competing Consumers, Compute Resource Consolidation, CQRS, Deployment Stamps, Edge Workload Configuration, Event Sourcing, External Configuration Store, Federated Identity, Gateway Aggregation, Gateway Offloading, Gateway Routing, Geode, Health Endpoint Monitoring, Index Table, Leader Election, Materialized View, Pipes and Filters, Priority Queue, Publisher/Subscriber, Queue-Based Load Leveling, Quarantine, Rate Limiting, Retry, Saga, Scheduler Agent Supervisor, Sequential Convoy, Sharding, Sidecar, Static Content Hosting, Strangler Fig, Throttling, Valet Key.

> **💡 Decision takeaway**
>
> Assess service constraints, shared responsibility, residency and operating cost alongside the benefits of managed services.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 11. Security Architecture →](#11-security-architecture)**

---

<a id="11-security-architecture"></a>

## 🛡️ 11. Security Architecture

`CHAPTER 11` · `RUN & ASSURE`

Design trust, identity and information protection into every boundary.


### 11.1 Core Principles

- **Defence in depth**
- **Least privilege**
- **Zero Trust** ("never trust, always verify"; NIST SP 800-207)
- **Secure by default / secure by design**
- **Separation of duties**
- **Fail securely**
- **Complete mediation** (check every access)
- **Minimise attack surface**
- **Economy of mechanism**
- **Open design** (no security through obscurity)
- **Assume breach**
- **Privacy by design** (Cavoukian's seven foundational principles)
- **CIA triad** (Confidentiality, Integrity, Availability) plus authenticity, non-repudiation, accountability

### 11.2 Identity & Access Patterns

- **SSO**, **Federation** (SAML, OpenID Connect), **OAuth 2.0** (delegated authorisation), **JWT** (use with care: validation, expiry, audience)
- **MFA / Passwordless / Passkeys (FIDO2/WebAuthn)**
- **RBAC, ABAC, ReBAC, Policy-based access (PBAC)**; externalised authorisation (policy decision/enforcement points)
- **Privileged Access Management (PAM)**, just-in-time access
- **Workload identity** (service identities, mTLS, short-lived credentials)
- **Customer IAM (CIAM)** vs **Workforce IAM**
- **Token patterns**: access/refresh tokens, token exchange, PKCE for public clients
- **Strong Customer Authentication / step-up authentication** for high-risk actions

### 11.3 Data & Application Security Patterns

- **Encryption** at rest, in transit (TLS), and where warranted in use; envelope encryption; **KMS/HSM**; key rotation; BYOK/HYOK
- **Tokenisation, masking, format-preserving encryption**
- **Secrets management**
- **Input validation, output encoding**, parameterised queries
- **OWASP Top 10**, **OWASP ASVS**, **OWASP API Security Top 10**
- **Threat modelling**: STRIDE, PASTA, LINDDUN (privacy), attack trees, data-flow diagrams
- **Secure SDLC / DevSecOps**: SAST, DAST, IAST, SCA, secret scanning, IaC scanning, container scanning, SBOM
- **WAF, API gateway security, DDoS protection, bot management**
- **Network segmentation, micro-segmentation, DMZ, private endpoints**
- **Security monitoring**: SIEM, SOAR, UEBA, EDR/XDR
- **Audit logging** (immutable, tamper-evident)
- **Fraud detection architectures** (real-time scoring, rules + ML, feedback loops)
- **Backup immutability / ransomware resilience**

### 11.4 Compliance & Frameworks

ISO/IEC 27001/27002, NIST CSF, NIST SP 800-53, CIS Controls, SOC 2, PCI DSS (payments), privacy laws (e.g. GDPR; for New Zealand, the Privacy Act 2020), sector regulation (e.g. prudential and outsourcing/cloud requirements for banks), MITRE ATT&CK for threat behaviours.

> **💡 Decision takeaway**
>
> Security belongs in the initial design. Verify controls at the resource boundary and protect the paths used for recovery.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 12. Observability & Operations →](#12-observability--operations)**

---

<a id="12-observability--operations"></a>

## 📡 12. Observability & Operations

`CHAPTER 12` · `RUN & ASSURE`

Make system health, business outcomes and incident response observable.


### 12.1 Observability

- **Three pillars**: logs, metrics, traces (plus events/profiles increasingly)
- **Distributed tracing** with correlation/trace IDs propagated across services
- **Structured logging** with consistent schema
- **Golden signals** (Google SRE): latency, traffic, errors, saturation
- **RED method** (Rate, Errors, Duration) for services; **USE method** (Utilisation, Saturation, Errors) for resources
- **OpenTelemetry** as vendor-neutral instrumentation standard
- **Dashboards, alerting on symptoms (SLO burn) rather than causes**
- **Synthetic monitoring and real-user monitoring**
- **Audit and business-level monitoring** (e.g. transaction success rates, reconciliation breaks)

### 12.2 SRE & Reliability Practices

- **SLI / SLO / SLA** and **error budgets**
- **Incident management**: severity, roles, runbooks, blameless post-incident reviews
- **Toil reduction and automation**
- **Capacity planning and load/performance testing**
- **Game days / chaos experiments**
- **Change management**: progressive delivery, change windows where required
- **DORA metrics**: deployment frequency, lead time for changes, change failure rate, time to restore service (and reliability)

### 12.3 DevOps / Delivery Practices

- CI/CD pipelines with quality gates
- Test pyramid: unit, integration, contract, end-to-end; plus performance, security, resilience testing
- **Consumer-driven contract testing**
- **Test data management**
- **Environment parity and ephemeral environments**
- **Release trains vs continuous delivery**
- **Trunk-based development**, short-lived branches
- **Documentation as code** (diagrams as code, ADRs in repo)

> **💡 Decision takeaway**
>
> Useful telemetry supports decisions. Pair signals and alerts with service objectives, accountable owners and tested runbooks.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 13. Quality Attributes (NFRs) →](#13-quality-attributes-nfrs)**

---

<a id="13-quality-attributes-nfrs"></a>

## ⚖️ 13. Quality Attributes (NFRs)

`CHAPTER 13` · `RUN & ASSURE`

Translate quality ambitions into measurable architectural requirements.


| Attribute | Typical concerns / tactics |
|---|---|
| **Availability** | Redundancy, failover, health checks, multi-AZ/region, graceful degradation |
| **Reliability** | Fault tolerance, retries, idempotency, data integrity |
| **Performance** | Latency/throughput targets, caching, async, indexing, partitioning |
| **Scalability** | Horizontal scale, statelessness, sharding, autoscaling |
| **Elasticity** | Scale up/down on demand |
| **Resilience** | Recover from failure, bulkheads, circuit breakers, chaos testing |
| **Security** | AuthN/Z, encryption, auditing, threat mitigation |
| **Privacy** | Minimisation, consent, retention, residency |
| **Maintainability** | Modularity, readability, low coupling, documentation |
| **Modifiability / Evolvability** | Loose coupling, versioning, feature toggles, fitness functions |
| **Testability** | DI, seams, determinism, observability |
| **Interoperability** | Standards, open APIs, contracts |
| **Portability** | Containers, abstraction layers, open standards |
| **Observability** | Telemetry, traceability, diagnosability |
| **Usability / Accessibility** | UX, WCAG |
| **Auditability / Traceability** | Immutable logs, lineage |
| **Recoverability** | Backup, RTO/RPO, DR |
| **Cost efficiency** | FinOps, rightsizing, lifecycle |
| **Sustainability** | Energy-efficient design, region choice, utilisation |
| **Compliance** | Regulatory control mapping |
| **Data integrity & consistency** | Constraints, reconciliation, transactions |
| **Supportability / Operability** | Runbooks, automation, clear failure modes |

Practice: express NFRs as **measurable** targets (e.g. p95 latency, availability %, RTO/RPO, throughput), define them early, and verify through tests and fitness functions. Use **quality attribute scenarios** (source, stimulus, artefact, environment, response, response measure) and **utility trees** (ATAM).

> **💡 Decision takeaway**
>
> Replace vague goals with operating conditions, thresholds, measurement locations and a verification method.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 14. Architecture Governance & Documentation →](#14-architecture-governance--documentation)**

---

<a id="14-architecture-governance--documentation"></a>

## 📋 14. Architecture Governance & Documentation

`CHAPTER 14` · `DECIDE & EVOLVE`

Make consequential decisions traceable without creating unnecessary gates.


### 14.1 Governance Mechanisms

- **Architecture principles, standards, and reference architectures**
- **Architecture Review Board (ARB)** / design authority; prefer lightweight, advisory, and asynchronous reviews where possible
- **Architecture Decision Records (ADRs)** (Nygard format: Title, Status, Context, Decision, Consequences)
- **Technology radar** (Adopt, Trial, Assess, Hold)
- **Standards lifecycle and exception (waiver) process**
- **Architecture compliance reviews** at defined gates
- **Technical debt register**, **application portfolio management (TIME model: Tolerate, Invest, Migrate, Eliminate)**
- **Roadmaps**: current state, target state, transition architectures
- **Gap analysis** between baseline and target
- **Architecture repository / enterprise knowledge base**
- **Fitness functions** (automated architecture checks in pipelines)
- **Guardrails over gates**: enable teams via paved roads while protecting key constraints

### 14.2 Documentation Approaches

- **C4 diagrams** for software structure; **ArchiMate** for enterprise-wide, cross-layer views and traceability
- **Sequence, deployment, data-flow, state diagrams** (UML as needed)
- **BPMN** for processes
- **ER / dimensional models** for data
- **Diagrams as code** (e.g. Mermaid, PlantUML, Structurizr) versioned with source
- **Viewpoints and views** tailored to stakeholder concerns (ISO/IEC/IEEE 42010)
- **Architecture Vision, Solution Design Document, HLD/LLD, Interface specifications, Runbooks**
- **Traceability**: requirement → capability → application → data → technology

### 14.3 Stakeholder Communication

- Identify stakeholders and concerns; tailor views (executive, business, delivery, operations, security, risk)
- Communicate **trade-offs, options, risks, and costs**, not just the recommendation
- Use **capability heatmaps, roadmaps, and decision records** as shared artefacts

> **💡 Decision takeaway**
>
> Scale governance and documentation to risk. Communicate options, trade-offs and consequences to each audience.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 15. Anti-Patterns →](#15-anti-patterns)**

---

<a id="15-anti-patterns"></a>

## 🚧 15. Anti-Patterns

`CHAPTER 15` · `DECIDE & EVOLVE`

Recognise structural warning signs and select proportionate remedies.


| Anti-pattern | Description | Remedy |
|---|---|---|
| **Big Ball of Mud** | No discernible structure | Introduce boundaries, strangler, modularise |
| **Distributed Monolith** | Microservices that must deploy and change together | Re-align boundaries, reduce synchronous coupling |
| **Golden Hammer** | One technology for every problem | Fit-for-purpose selection |
| **Resume-Driven / Hype-Driven Development** | Tech chosen for novelty | Tie to requirements and ADRs |
| **Architecture Astronautics / Over-engineering** | Excess abstraction | YAGNI, evolutionary design |
| **Ivory Tower Architecture** | Architects disconnected from delivery | Embed, collaborate, advisory forum |
| **Analysis Paralysis** | Endless design without delivery | Timebox, last responsible moment |
| **Shared Database Integration** | Many systems coupled via one schema | APIs/events, database per service |
| **Chatty Services / N+1 calls** | Excessive fine-grained calls | Coarser APIs, aggregation, caching |
| **God Service / God Object** | One component with too many responsibilities | Decompose by bounded context |
| **Entity Services / CRUD Microservices** | Services per table | Align to business capabilities |
| **Shared Library Coupling** | Common library forcing lock-step upgrades | Versioning, contracts, minimise shared code |
| **Vendor Lock-in by Accident** | Unmanaged proprietary dependencies | Conscious trade-off, exit strategy, abstraction where valuable |
| **ESB as Monolith** | All logic in central bus | Smart endpoints, dumb pipes |
| **Canonical Model Overreach** | Enterprise-wide model that satisfies nobody | Domain-scoped models, published languages |
| **Dual Write** | Writing to DB and broker non-atomically | Outbox / CDC |
| **Distributed Transactions Everywhere** | 2PC across services | Sagas, eventual consistency |
| **Retry Storms** | Uncontrolled retries amplifying failure | Backoff, jitter, circuit breakers, budgets |
| **Missing Timeouts** | Threads/resources stuck waiting | Timeouts everywhere |
| **Data Swamp** | Ungoverned lake | Catalogue, ownership, quality, zones |
| **Spreadsheet/Shadow IT Data Silos** | Unmanaged critical data | Provide governed self-service |
| **Metric Drift** | Different definitions of same KPI | Semantic/metrics layer |
| **Lava Flow** | Dead code/legacy retained out of fear | Remove with tests and telemetry |
| **Cargo Cult Agile/DevOps** | Rituals without outcomes | Focus on flow and feedback metrics |
| **Manual Environments / Snowflake Servers** | Unreproducible infra | IaC, immutability |
| **Security as Afterthought** | Late-stage security reviews | Threat model early, DevSecOps |
| **Premature Optimisation** | Optimising without evidence | Measure first |
| **Premature Microservices** | Splitting before understanding domain | Start modular monolith |
| **Single Point of Failure (SPOF)** | One component takes down the system | Redundancy, isolation |
| **Reinventing the Wheel** | Custom build for commodity capability | Reuse/buy for context capabilities |
| **Tech Debt Denial** | Unmanaged accumulation | Register, prioritise, pay down |

> **💡 Decision takeaway**
>
> Investigate the cause behind an anti-pattern label. A remedy should reduce the problem without introducing unjustified complexity.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: 16. Pattern Selection Cheat Sheet →](#16-pattern-selection-cheat-sheet)**

---

<a id="16-pattern-selection-cheat-sheet"></a>

## 🧰 16. Pattern Selection Cheat Sheet

`CHAPTER 16` · `DECIDE & EVOLVE`

Move from a concrete situation to a shortlist of candidate patterns.


| Situation | Candidate patterns |
|---|---|
| Replace a legacy system gradually | Strangler Fig, ACL, Branch by Abstraction, Parallel Run, CDC |
| Reliable event publication from a service DB | Transactional Outbox, CDC |
| Multi-service business transaction | Saga (orchestrated for complex flows; choreographed for simple), idempotent consumers |
| Protect your model from an external/legacy model | Anti-Corruption Layer, Published Language |
| Different consumers need different APIs | BFF, API Gateway, GraphQL |
| Heavy read load vs complex write logic | CQRS, Materialised Views, caching |
| Full audit trail and temporal queries | Event Sourcing, bi-temporal modelling, ledger store |
| Spiky or unpredictable workload | Serverless, queue-based load leveling, autoscaling |
| Protect downstream from overload | Rate limiting, bulkhead, backpressure, load shedding |
| Dependency intermittently failing | Timeout, retry with backoff and jitter, circuit breaker, fallback |
| Large payloads in messaging | Claim Check |
| Cross-domain analytics at scale | Lakehouse + Medallion, Data Vault or dimensional marts, semantic layer |
| Many domain teams, central data team bottleneck | Data Mesh (with platform and federated governance) |
| Real-time analytics and reprocessing | Kappa / streaming with replay |
| Consistent business definitions of customer/product | MDM, reference data management, business glossary |
| Reduce blast radius for outages | Cell-based architecture, bulkheads, multi-AZ/region, shuffle sharding |
| Roll out change safely | Feature flags, canary, blue/green, progressive delivery |
| Reduce cognitive load of delivery teams | Platform engineering, golden paths, Team Topologies |
| Third-party access to capabilities | Open APIs, API gateway, OAuth 2.0 / OIDC, developer portal |
| Need strong consistency and relational integrity | RDBMS (or distributed SQL), ACID transactions, optimistic locking |
| Relationship-heavy analysis (fraud, lineage) | Graph database |
| Documenting for different audiences | C4 (engineering), ArchiMate (enterprise), BPMN (process), ADRs (decisions) |
| Decide build vs buy | Core/Context, Wardley mapping, capability heatmap, TCO analysis |

> **💡 Decision takeaway**
>
> Use this cheat sheet to start an assessment, not finish it. Compare fit, alternatives and operational consequences before committing.

**[↑ Explore the guide](#explore-the-guide)** · **[Next: Appendix A: ADR Template →](#appendix-a-adr-template)**

---

<a id="appendix-a-adr-template"></a>

## 📝 Appendix A: ADR Template

`RESOURCE` · `COPYABLE TEMPLATE`


```markdown
# ADR-NNN: <Short title>

- Status: Proposed | Accepted | Superseded by ADR-XXX | Deprecated
- Date: YYYY-MM-DD
- Deciders: <names/roles>

## Context
What forces, constraints, and requirements are at play?

## Options Considered
1. Option A: pros / cons
2. Option B: pros / cons

## Decision
What was chosen and why.

## Consequences
Positive, negative, risks, follow-up actions.
```


**[↑ Explore the guide](#explore-the-guide)**

---

<a id="appendix-b-architecture-principle-template-togaf-style"></a>

## 📝 Appendix B: Architecture Principle Template (TOGAF style)

`RESOURCE` · `COPYABLE TEMPLATE`


```markdown
**Name:** <short, memorable>
**Statement:** <succinct, unambiguous rule>
**Rationale:** <business benefits and reasoning>
**Implications:** <what changes for people, process, technology, cost>
```


**[↑ Explore the guide](#explore-the-guide)**

---

<a id="appendix-c-key-reference-sources"></a>

## 📚 Appendix C: Key Reference Sources

`RESOURCE` · `FURTHER READING`


- Evans, *Domain-Driven Design* (2003); Vernon, *Implementing DDD*
- Fowler, *Patterns of Enterprise Application Architecture*; *Refactoring*
- Hohpe & Woolf, *Enterprise Integration Patterns*
- Nygard, *Release It!*; "Documenting Architecture Decisions"
- Newman, *Building Microservices*; *Monolith to Microservices*
- Kleppmann, *Designing Data-Intensive Applications*
- Richards & Ford, *Fundamentals of Software Architecture*; Ford et al., *Building Evolutionary Architectures*
- Bass, Clements, Kazman, *Software Architecture in Practice*
- Kimball & Ross, *The Data Warehouse Toolkit*; Inmon, *Building the Data Warehouse*; Linstedt, *Building a Scalable Data Warehouse with Data Vault 2.0*
- Dehghani, *Data Mesh*; Reis & Housley, *Fundamentals of Data Engineering*
- DAMA, *DAMA-DMBOK*
- The Open Group: *TOGAF Standard*, *ArchiMate Specification*
- Business Architecture Guild, *BIZBOK Guide*
- Skelton & Pais, *Team Topologies*
- Beyer et al., *Site Reliability Engineering* (Google)
- Forsgren, Humble, Kim, *Accelerate*
- Brown, *The C4 Model*; arc42 documentation template
- OWASP (Top 10, ASVS, API Security); NIST SP 800-207 (Zero Trust)
- Cloud vendor Well-Architected frameworks and cloud design pattern catalogues

**[↑ Explore the guide](#explore-the-guide)**

---

## ✦ Make the next decision count

> **🎯 Put it into practice**
>
> Choose one architecture decision you are facing. Describe the business problem,
> compare a small set of viable patterns, record the consequences and define the
> evidence that will confirm or challenge your choice.

**[Pattern selection](#16-pattern-selection-cheat-sheet)** · **[ADR template](#appendix-a-adr-template)** · **[↑ Back to top](#top)**
