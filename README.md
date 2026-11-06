<div align="center">

**THE ARCHITECTURE FIELD GUIDE**

# Enterprise Architecture

### Patterns. Principles. Better decisions.

A cross-discipline reference handbook for connecting business intent<br>
to systems that are clear, resilient and ready for change.

`41 CHAPTERS` · `12 KNOWLEDGE AREAS` · `5 COPYABLE TEMPLATES`

**[Start learning](#what-is-enterprise-architecture)** · **[Explore the catalogue](#explore-the-guide)** · **[Choose a pattern](#33-pattern-selection-by-problem)** · **[Use a template](#part-xi-reference-architecture-documentation-templates)**

</div>

---

> **✦ The guiding idea**
>
> Good architecture is not a collection of fashionable patterns. It is a series
> of deliberate decisions that connect business outcomes to manageable complexity,
> risk, cost and change.

| 📖 Inside this guide | 🎯 Who it is for | 🗓 Edition |
| :--- | :--- | :--- |
| Enterprise Architecture Patterns, Principles and Best Practices. Technology-neutral guidance with cloud and distributed-systems examples. | Enterprise, Business, Solution, Application, Data, Integration, Security and Platform Architects; Lead Engineers. | **Version 1.0** · Prepared **4 November 2026** |

Use the roadmap for a guided read or the catalogue for a focused design decision.

<a id="explore-the-guide"></a>

## 🧭 Explore the guide

| **01 · FOUNDATIONS** | **02 · BUILDING BLOCKS** | **03 · DECISIONS & DELIVERY** | **04 · PRACTICE & IMPROVEMENT** |
| :--- | :--- | :--- | :--- |
| [Purpose & assessment](#1-purpose-scope-and-how-to-use-this-handbook) | [Applications & domains](#part-ii-solution-and-application-architecture) | [Quality & trade-offs](#part-vii-quality-attributes-and-architecture-trade-offs) | [Anti-patterns](#part-ix-anti-pattern-catalogue) |
| [Enterprise & business](#part-i-enterprise-wide-architecture-foundations) | [Integration](#part-iii-integration-architecture) · [Data](#part-iv-data-architecture) | [Governance & delivery](#part-viii-architecture-governance-and-delivery) | [Pattern selection](#part-x-pattern-selection-and-practical-decision-guides) |
| [Decision framework](#a-five-step-architecture-decision-framework) | [Security & trust](#part-v-security-privacy-and-trust-architecture) | [Review checklist](#28-architecture-review-checklist) | [Templates](#part-xi-reference-architecture-documentation-templates) |
| [Reading roadmap](#a-four-phase-reading-roadmap) | [Platforms & recovery](#part-vi-infrastructure-cloud-and-platform-architecture) | [Decision records](#26-architecture-decision-records-adrs) | [Further reading](#part-xii-further-reading-and-authoritative-references) |

<details>
<summary><strong>📚 Open the complete chapter index</strong></summary>

### Complete chapter index

- [Enterprise Architecture](#enterprise-architecture)
    - [Patterns. Principles. Better decisions.](#patterns-principles-better-decisions)
  - [🧭 Explore the guide](#-explore-the-guide)
    - [Complete chapter index](#complete-chapter-index)
  - [🏛️ What is enterprise architecture?](#️-what-is-enterprise-architecture)
  - [🎯 A five-step architecture decision framework](#-a-five-step-architecture-decision-framework)
  - [🗺️ A four-phase reading roadmap](#️-a-four-phase-reading-roadmap)
    - [Choose a reading route](#choose-a-reading-route)
  - [1. Purpose, scope and how to use this handbook](#1-purpose-scope-and-how-to-use-this-handbook)
    - [1.1 Distinguish the concepts](#11-distinguish-the-concepts)
    - [1.2 Pattern assessment template](#12-pattern-assessment-template)
  - [🏛️ Part I · Enterprise-wide architecture foundations](#️-part-i--enterprise-wide-architecture-foundations)
    - [2. Enterprise architecture principles](#2-enterprise-architecture-principles)
      - [2.1 Business alignment and value](#21-business-alignment-and-value)
      - [2.2 Simplicity and design](#22-simplicity-and-design)
      - [2.3 Data and information](#23-data-and-information)
      - [2.4 Security, privacy and risk](#24-security-privacy-and-risk)
      - [2.5 Resilience and operations](#25-resilience-and-operations)
      - [2.6 Technology, economics and sustainability](#26-technology-economics-and-sustainability)
    - [3. Enterprise architecture frameworks and viewpoints](#3-enterprise-architecture-frameworks-and-viewpoints)
      - [3.1 Common frameworks and methods](#31-common-frameworks-and-methods)
      - [3.2 Architecture viewpoints and models](#32-architecture-viewpoints-and-models)
    - [4. Business architecture patterns](#4-business-architecture-patterns)
      - [4.1 Capability-based planning](#41-capability-based-planning)
      - [4.2 Value stream and customer journey patterns](#42-value-stream-and-customer-journey-patterns)
      - [4.3 Operating model patterns](#43-operating-model-patterns)
      - [4.4 Business process patterns](#44-business-process-patterns)
      - [4.5 Business architecture anti-patterns](#45-business-architecture-anti-patterns)
  - [🧩 Part II · Solution and application architecture](#-part-ii--solution-and-application-architecture)
    - [5. Architectural styles and topologies](#5-architectural-styles-and-topologies)
      - [5.1 Choosing an architectural style](#51-choosing-an-architectural-style)
    - [6. Application architecture principles](#6-application-architecture-principles)
      - [6.1 Structural principles](#61-structural-principles)
      - [6.2 SOLID principles](#62-solid-principles)
    - [7. Domain-driven design patterns](#7-domain-driven-design-patterns)
      - [7.1 Strategic DDD](#71-strategic-ddd)
      - [7.2 Tactical DDD](#72-tactical-ddd)
    - [8. Application design and implementation patterns](#8-application-design-and-implementation-patterns)
      - [8.1 Layering and application structure](#81-layering-and-application-structure)
      - [8.2 Enterprise application patterns](#82-enterprise-application-patterns)
      - [8.3 Object-oriented and component design patterns](#83-object-oriented-and-component-design-patterns)
      - [8.4 Common application patterns](#84-common-application-patterns)
    - [9. API and interface architecture patterns](#9-api-and-interface-architecture-patterns)
      - [9.1 API styles and interaction models](#91-api-styles-and-interaction-models)
      - [9.2 API design principles](#92-api-design-principles)
      - [9.3 API patterns](#93-api-patterns)
      - [9.4 API anti-patterns](#94-api-anti-patterns)
    - [10. Microservices and distributed application patterns](#10-microservices-and-distributed-application-patterns)
      - [10.1 Service decomposition](#101-service-decomposition)
      - [10.2 Service interaction patterns](#102-service-interaction-patterns)
      - [10.3 Distributed transaction and consistency patterns](#103-distributed-transaction-and-consistency-patterns)
      - [10.4 Resilience patterns](#104-resilience-patterns)
      - [10.5 Distributed systems concerns](#105-distributed-systems-concerns)
  - [🔗 Part III · Integration architecture](#-part-iii--integration-architecture)
    - [11. Integration styles](#11-integration-styles)
    - [12. Enterprise Integration Patterns (EIP)](#12-enterprise-integration-patterns-eip)
      - [12.1 Message construction](#121-message-construction)
      - [12.2 Message channels](#122-message-channels)
      - [12.3 Message routing](#123-message-routing)
      - [12.4 Message transformation](#124-message-transformation)
      - [12.5 Message endpoints](#125-message-endpoints)
      - [12.6 Integration contract best practices](#126-integration-contract-best-practices)
      - [12.7 Canonical data model: use with care](#127-canonical-data-model-use-with-care)
  - [🗄️ Part IV · Data architecture](#️-part-iv--data-architecture)
    - [13. Data architecture principles](#13-data-architecture-principles)
    - [14. Data modelling patterns](#14-data-modelling-patterns)
      - [14.1 Modelling levels](#141-modelling-levels)
      - [14.2 Relational modelling patterns](#142-relational-modelling-patterns)
      - [14.3 Data type and physical design practices](#143-data-type-and-physical-design-practices)
    - [15. Data architecture styles and platform patterns](#15-data-architecture-styles-and-platform-patterns)
      - [15.1 Operational data patterns](#151-operational-data-patterns)
      - [15.2 Analytical data platform patterns](#152-analytical-data-platform-patterns)
      - [15.3 Data movement and processing patterns](#153-data-movement-and-processing-patterns)
      - [15.4 Data transformation and modelling patterns](#154-data-transformation-and-modelling-patterns)
      - [15.5 Data mesh principles and practices](#155-data-mesh-principles-and-practices)
      - [15.6 Data governance and management disciplines](#156-data-governance-and-management-disciplines)
      - [15.7 Data consistency and ownership decisions](#157-data-consistency-and-ownership-decisions)
    - [16. Data quality patterns](#16-data-quality-patterns)
  - [🛡️ Part V · Security, privacy and trust architecture](#️-part-v--security-privacy-and-trust-architecture)
    - [17. Security architecture principles](#17-security-architecture-principles)
    - [18. Security patterns](#18-security-patterns)
      - [18.1 Identity and access](#181-identity-and-access)
      - [18.2 Zero Trust and network security](#182-zero-trust-and-network-security)
      - [18.3 Data protection](#183-data-protection)
      - [18.4 Application security patterns](#184-application-security-patterns)
      - [18.5 Security architecture models and methods](#185-security-architecture-models-and-methods)
  - [☁️ Part VI · Infrastructure, cloud and platform architecture](#️-part-vi--infrastructure-cloud-and-platform-architecture)
    - [19. Infrastructure architecture patterns](#19-infrastructure-architecture-patterns)
      - [19.1 Compute and hosting](#191-compute-and-hosting)
      - [19.2 Network architecture](#192-network-architecture)
      - [19.3 Deployment and release patterns](#193-deployment-and-release-patterns)
      - [19.4 Platform engineering patterns](#194-platform-engineering-patterns)
    - [20. Availability, disaster recovery and continuity](#20-availability-disaster-recovery-and-continuity)
      - [20.1 Availability patterns](#201-availability-patterns)
      - [20.2 Recovery concepts](#202-recovery-concepts)
      - [20.3 Resilience engineering practices](#203-resilience-engineering-practices)
  - [⚖️ Part VII · Quality attributes and architecture trade-offs](#️-part-vii--quality-attributes-and-architecture-trade-offs)
    - [21. Quality attribute catalogue](#21-quality-attribute-catalogue)
    - [22. Quality attribute scenarios](#22-quality-attribute-scenarios)
    - [23. Common architecture trade-offs](#23-common-architecture-trade-offs)
  - [📋 Part VIII · Architecture governance and delivery](#-part-viii--architecture-governance-and-delivery)
    - [24. Architecture governance practices](#24-architecture-governance-practices)
    - [25. Architecture artefacts](#25-architecture-artefacts)
    - [26. Architecture Decision Records (ADRs)](#26-architecture-decision-records-adrs)
    - [27. Solution design, application architecture and system design](#27-solution-design-application-architecture-and-system-design)
    - [28. Architecture review checklist](#28-architecture-review-checklist)
      - [Business and scope](#business-and-scope)
      - [Requirements and quality](#requirements-and-quality)
      - [Application and services](#application-and-services)
      - [Data](#data)
      - [Security and privacy](#security-and-privacy)
      - [Resilience and operations](#resilience-and-operations)
      - [Delivery and economics](#delivery-and-economics)
  - [🚧 Part IX · Anti-pattern catalogue](#-part-ix--anti-pattern-catalogue)
    - [29. Enterprise and business anti-patterns](#29-enterprise-and-business-anti-patterns)
    - [30. Application and distributed-system anti-patterns](#30-application-and-distributed-system-anti-patterns)
    - [31. Data anti-patterns](#31-data-anti-patterns)
    - [32. Security and infrastructure anti-patterns](#32-security-and-infrastructure-anti-patterns)
  - [🧭 Part X · Pattern selection and practical decision guides](#-part-x--pattern-selection-and-practical-decision-guides)
    - [33. Pattern selection by problem](#33-pattern-selection-by-problem)
    - [34. Architecture decision sequence](#34-architecture-decision-sequence)
    - [35. Architecture quality gates](#35-architecture-quality-gates)
    - [36. Architecture fitness functions](#36-architecture-fitness-functions)
  - [📝 Part XI · Reference architecture documentation templates](#-part-xi--reference-architecture-documentation-templates)
    - [37. One-page architecture overview](#37-one-page-architecture-overview)
    - [38. Integration contract template](#38-integration-contract-template)
    - [39. Data product template](#39-data-product-template)
    - [40. NFR template](#40-nfr-template)
  - [📚 Part XII · Further reading and authoritative references](#-part-xii--further-reading-and-authoritative-references)
  - [✦ 41. Final guidance: how an experienced architect should apply this catalogue](#-41-final-guidance-how-an-experienced-architect-should-apply-this-catalogue)

</details>

---

<a id="what-is-enterprise-architecture"></a>

## 🏛️ What is enterprise architecture?

Enterprise architecture connects business intent to the capabilities, information,
applications and platforms needed to deliver it. It provides a shared way to make
decisions across teams, rather than treating each system as an isolated project.

This guide takes you from enterprise-wide principles to practical design patterns,
measurable quality attributes, governance and reusable documentation templates.
It is both a reading roadmap and a detailed reference: follow the sequence when
learning, or use the table of contents to jump directly to a design concern.

> **💡 Key insight**
>
> A pattern is a candidate solution, not a requirement. Start with
> the business problem, compare alternatives and test the consequences.

<a id="a-five-step-architecture-decision-framework"></a>

## 🎯 A five-step architecture decision framework

Use this framework to orient your work before exploring the catalogue. The detailed
decision sequence and assessment templates remain in the handbook sections below.

| Step | What to do | Evidence to produce |
| --- | --- | --- |
| 1. Frame the outcome | Identify stakeholders, business capabilities, scope and constraints. | A clear problem statement and measurable success criteria. |
| 2. Define boundaries and quality | Establish responsibilities, data ownership, trust boundaries and measurable NFRs. | Context views, ownership decisions and quality scenarios. |
| 3. Compare solution options | Evaluate styles and patterns against complexity, consistency, delivery and operating needs. | Alternatives, trade-offs and decision rationale. |
| 4. Validate the difficult parts | Test critical assumptions about failure, security, performance, recovery and cost. | Prototype results, control checks and operational evidence. |
| 5. Record and evolve | Capture significant decisions, support ownership and triggers for revisiting the design. | ADRs, fitness functions and an improvement backlog. |

> **✦ Working mindset**
>
> Prefer the simplest design that meets the requirements.
> Distribution, standardisation and reuse all have costs as well as benefits.

<a id="a-four-phase-reading-roadmap"></a>

## 🗺️ A four-phase reading roadmap

The phases describe a learning sequence, not a delivery waterfall. Security,
privacy, data ownership and recovery must influence decisions from the beginning;
their dedicated chapters provide depth rather than a reason to defer them.

| Phase | Focus | Handbook coverage | Practical goal |
| --- | --- | --- | --- |
| 1. Establish foundations | Principles, viewpoints and business architecture. | Purpose and scope; Part I. | Explain the business outcome and the boundaries of the change. |
| 2. Understand the building blocks | Applications, integration, data, security and platforms. | Parts II-VI. | Compare viable patterns and understand their consequences. |
| 3. Make decisions measurable | Quality attributes, trade-offs, governance and delivery. | Parts VII-VIII. | Translate architecture intent into decisions, evidence and review criteria. |
| 4. Apply and improve | Anti-patterns, selection guides, fitness functions, templates and references. | Parts IX-XII and final guidance. | Review a real design, document it proportionately and improve it using evidence. |

### Choose a reading route

- **Learning the discipline:** Read the foundations, then work through the domain
  chapters before using the decision guides and templates.
- **Designing a solution:** Start with the purpose and pattern assessment template,
  consult the relevant domain chapters, then use the quality scenarios and review checklist.
- **Reviewing an existing estate:** Combine the anti-pattern catalogue with the
  ownership, contract, recovery and fitness-function guidance.
- **Leading delivery:** Use the governance, artefact and quality-gate sections to
  agree decision rights and the evidence needed for safe change.

---

<a id="1-purpose-scope-and-how-to-use-this-handbook"></a>

## 1. Purpose, scope and how to use this handbook

This handbook is a structured catalogue of established architecture
principles, architectural styles, solution patterns, application
patterns, data patterns, integration patterns, security patterns,
infrastructure patterns and governance practices.

It is deliberately broad, but it is **not a claim to contain every
pattern ever published**. No authoritative, finite, universally accepted
catalogue exists. Patterns overlap, names vary between authors and
vendors, and new patterns emerge as technology and operating models
change. The catalogue therefore concentrates on widely recognised
patterns and practices, and identifies where a technique is
context-dependent.

<a id="1-1-distinguish-the-concepts"></a>

### 1.1 Distinguish the concepts

| Concept | Meaning | Example |
| --- | --- | --- |
| Principle | A durable rule or direction used to guide decisions | Data is treated as an enterprise asset |
| Standard | A mandatory or preferred specification | APIs use the enterprise OAuth profile |
| Reference architecture | A reusable conceptual structure for a class of solutions | Event-driven integration reference architecture |
| Architectural style | A broad structural approach | Layered, microservices, event-driven |
| Architectural pattern | A recurring structural solution to a system-level problem | Hexagonal architecture, CQRS |
| Design pattern | A reusable solution to a smaller design problem | Strategy, Adapter, Factory |
| Integration pattern | A reusable way to exchange, route or transform information | Publish-subscribe, Content-Based Router |
| Practice | A repeatable engineering or governance activity | Threat modelling, automated architecture fitness tests |
| Anti-pattern | A commonly repeated approach that creates avoidable problems | Distributed monolith |

A pattern is not a product, technology or universal prescription. It
describes a recurring problem, a solution structure and consequences. An
implementation still needs to be designed for the actual requirements
and constraints.

<a id="1-2-pattern-assessment-template"></a>

### 1.2 Pattern assessment template

For every significant pattern considered, document:

1.  **Problem:** What recurring problem are we solving?
2.  **Context:** What business, organisational and technical conditions
    apply?
3.  **Forces:** What competing concerns exist?
4.  **Solution:** What components, responsibilities and interactions are
    introduced?
5.  **Consequences:** What benefits, costs and failure modes follow?
6.  **Applicability:** When is it a good fit?
7.  **Avoid when:** What conditions make it unsuitable?
8.  **Alternatives:** What simpler or competing approaches exist?
9.  **Quality attributes:** Which measurable NFRs does it improve or
    threaten?
10. **Operational model:** Who owns, deploys, monitors, supports and
    recovers it?

---

<a id="part-i-enterprise-wide-architecture-foundations"></a>

## 🏛️ Part I · Enterprise-wide architecture foundations

`PHASE 01` · `FOUNDATIONS` · **Chapters 2–4**

Start with the business problem. These chapters establish the principles, viewpoints and capability boundaries that make later technical choices meaningful.

> **💡 Key insight**
>
> A framework organises architecture work; it does not replace accountable decisions.


<a id="2-enterprise-architecture-principles"></a>

### 2. Enterprise architecture principles

Architecture principles should be few enough to be memorable, specific
enough to influence decisions, and governed through an agreed exception
process. The following are candidate principles; an organisation should
adapt and approve them rather than blindly adopt all of them.

<a id="2-1-business-alignment-and-value"></a>

#### 2.1 Business alignment and value

1.  **Business outcome first:** Architecture exists to enable measurable
    business outcomes, not to maximise technology novelty.
2.  **Capability-led change:** Organise change around business
    capabilities and value streams, not solely around existing
    applications or reporting lines.
3.  **Business ownership:** Business leaders own business outcomes,
    policies and the meaning of business information.
4.  **Traceability:** Significant architectural decisions should trace
    to business objectives, requirements, risks or mandated constraints.
5.  **Outcome measurement:** Define measurable benefits and operational
    outcomes before implementation.
6.  **Process before automation:** Understand and improve the business
    process before digitising or automating it.
7.  **Customer and colleague experience:** Consider the complete
    journey, including exceptions, assisted channels and operational
    handling.

<a id="2-2-simplicity-and-design"></a>

#### 2.2 Simplicity and design

8.  **Simplicity by default:** Prefer the least complex design that
    satisfies the requirements and foreseeable change.
9.  **Reuse before build, with fit assessment:** Reuse enterprise
    capabilities where they genuinely fit; do not force unsuitable
    reuse.
10. **Loose coupling:** Minimise unnecessary dependencies between
    business capabilities, applications, services and data stores.
11. **High cohesion:** Keep closely related responsibilities and rules
    together.
12. **Explicit boundaries:** Make ownership, responsibilities,
    interfaces and data boundaries clear.
13. **Separation of concerns:** Separate responsibilities that change
    for different reasons.
14. **Encapsulation:** Hide internal implementation details behind
    stable contracts.
15. **Design for change:** Isolate volatile decisions and avoid
    unnecessary irreversible commitments.
16. **Avoid accidental distribution:** Do not introduce network
    boundaries unless independent deployment, scaling, ownership,
    resilience or other benefits justify them.

<a id="2-3-data-and-information"></a>

#### 2.3 Data and information

17. **Data is an asset:** Manage data as a business asset throughout its
    lifecycle.
18. **Accountability at source:** Assign accountable owners and stewards
    for important data domains.
19. **Authoritative source clarity:** Identify the authoritative system
    or process for each critical business fact.
20. **Fit-for-purpose quality:** Define quality rules against actual
    use, risk and service-level needs.
21. **Metadata matters:** Manage business definitions, technical
    metadata, lineage, classification and ownership.
22. **Data minimisation:** Collect, retain and expose only the data
    needed for legitimate purposes.
23. **Controlled sharing:** Share data through governed contracts and
    approved access paths.
24. **Meaning before format:** Standardise business meaning and
    semantics before enforcing physical formats.
25. **Lifecycle management:** Define retention, archival, legal hold and
    disposal requirements.

<a id="2-4-security-privacy-and-risk"></a>

#### 2.4 Security, privacy and risk

26. **Secure by design:** Include security and privacy in requirements
    and design from the beginning.
27. **Least privilege:** Grant only the minimum access required for a
    defined purpose and duration.
28. **Verify explicitly:** Authenticate and authorise access based on
    identity, device, resource and contextual risk rather than network
    location alone.
29. **Defence in depth:** Use complementary preventive, detective and
    responsive controls.
30. **Assume failure and compromise:** Design to detect, contain and
    recover from incidents.
31. **Classify and protect:** Apply controls proportionate to
    information sensitivity and business impact.
32. **Auditability:** Preserve appropriate evidence of sensitive access
    and consequential business actions.
33. **Compliance by design:** Translate regulatory and policy
    obligations into traceable architecture controls.

<a id="2-5-resilience-and-operations"></a>

#### 2.5 Resilience and operations

34. **Availability is designed:** Define availability and recovery
    objectives and design to meet them.
35. **Failure isolation:** Limit the blast radius of component,
    dependency and operator failures.
36. **Graceful degradation:** Preserve essential functions when
    non-essential dependencies fail.
37. **Recoverability:** Backups are not sufficient; regularly prove
    restoration and recovery.
38. **Observable by design:** Emit useful logs, metrics, traces, events
    and business-level indicators.
39. **Automate repeatability:** Automate deployment, configuration,
    testing, recovery and routine operations where safe.
40. **Operational ownership:** Every production capability has a named
    support and service ownership model.

<a id="2-6-technology-economics-and-sustainability"></a>

#### 2.6 Technology, economics and sustainability

41. **Technology serves architecture:** Select technologies to meet
    requirements and constraints, not because they are fashionable.
42. **Total cost of ownership:** Assess build, run, change, licensing,
    skills, support, migration and exit costs.
43. **Standardise deliberately:** Standardise common capabilities while
    allowing justified exceptions.
44. **Portability where valuable:** Avoid lock-in where portability has
    material value; do not pay unlimited cost for hypothetical
    portability.
45. **FinOps accountability:** Make cost visible, attributable and
    optimisable.
46. **Sustainable engineering:** Consider resource efficiency,
    lifecycle, energy and environmental impact where material.
47. **Continuous improvement:** Revisit architecture as business
    strategy, technology, risk and evidence change.

<a id="3-enterprise-architecture-frameworks-and-viewpoints"></a>

### 3. Enterprise architecture frameworks and viewpoints

Frameworks are tools for organising architecture work. They are not
architectures and should not become documentation exercises detached
from decisions.

<a id="3-1-common-frameworks-and-methods"></a>

#### 3.1 Common frameworks and methods

| Framework / method | Primary purpose | Typical use |
| --- | --- | --- |
| TOGAF | Enterprise architecture method, content and governance guidance | Architecture development, capability and change governance |
| ArchiMate | Enterprise architecture modelling language | Relationships across motivation, strategy, business, application and technology |
| Zachman Framework | Enterprise architecture classification schema | Organising architectural descriptions by interrogatives and perspectives |
| BIAN | Banking industry reference architecture and service-domain model | Banking capability and service-domain alignment |
| TM Forum ODA | Open digital architecture for communications service providers | Telecoms architecture and component interoperability |
| IT4IT | Reference architecture for managing the business of IT | IT value chain and service management |
| FEAF | Federal enterprise architecture framework | Government architecture |
| SABSA | Business-driven security architecture method | Security requirements, risk and traceability |
| DDD | Domain-driven design approach | Modelling complex business domains in software |
| DAMA-DMBOK | Data management body of knowledge | Data governance and management disciplines |
| ITIL | Service management practices | Service lifecycle and operational management |
| COBIT | Governance and management of enterprise information and technology | Governance, control objectives and performance |

Do not treat these frameworks as interchangeable. For example, ArchiMate
is a modelling language, TOGAF is an architecture framework, and
DAMA-DMBOK is a data-management body of knowledge.

<a id="3-2-architecture-viewpoints-and-models"></a>

#### 3.2 Architecture viewpoints and models

Common views include:

-   **Motivation:** drivers, goals, outcomes, principles, requirements
    and constraints.
-   **Strategy:** capabilities, value streams, resources and courses of
    action.
-   **Business:** actors, roles, organisation, functions, services,
    processes and information.
-   **Application:** applications, components, services, interfaces and
    interactions.
-   **Data / information:** conceptual, logical and physical models;
    ownership and flows.
-   **Technology:** infrastructure, platforms, networks, runtime and
    deployment.
-   **Security:** trust boundaries, identities, data protection, threats
    and controls.
-   **Integration:** APIs, events, messages, contracts, protocols and
    dependencies.
-   **Operations:** support model, SLOs, monitoring, incident response
    and recovery.
-   **Transition:** work packages, migration states, dependencies and
    roadmaps.

Choose views based on stakeholder concerns and decisions. A diagram
should answer a question, not merely decorate a document.

<a id="4-business-architecture-patterns"></a>

### 4. Business architecture patterns

Business architecture describes what the enterprise does and how it
creates value, independent of the detailed technology implementation.

<a id="4-1-capability-based-planning"></a>

#### 4.1 Capability-based planning

A business capability describes what an organisation must be able to do,
not necessarily how it is organised or which system implements it.

Common practices and patterns:

-   Capability map: hierarchical decomposition of business abilities.
-   Capability heat map: assess strategic importance, performance,
    maturity, risk and investment.
-   Capability-based investment: prioritise change by capability gaps
    and outcomes.
-   Capability ownership: assign accountable business owners.
-   Capability-to-application mapping: show which systems enable each
    capability.
-   Capability rationalisation: identify duplication, gaps and
    over-dependence.

**Best practice:** Keep capability names stable and business-oriented.
Do not model capabilities as a copy of the organisational chart or
application inventory.

<a id="4-2-value-stream-and-customer-journey-patterns"></a>

#### 4.2 Value stream and customer journey patterns

-   **Value stream mapping:** identify stages that create value for a
    stakeholder.
-   **Customer journey mapping:** model customer goals, touchpoints,
    channels, pain points and outcomes.
-   **Service blueprint:** connect customer-facing activity to backstage
    processes, systems and support.
-   **Business event modelling:** identify meaningful business state
    changes that trigger work.
-   **Journey orchestration:** coordinate work across channels, people,
    systems and time.
-   **Case management:** manage variable, knowledge-intensive work where
    the exact process path cannot be fully predetermined.

<a id="4-3-operating-model-patterns"></a>

#### 4.3 Operating model patterns

-   **Functional operating model:** organise around specialist
    functions.
-   **Divisional / product operating model:** organise around products,
    markets or business lines.
-   **Shared services:** consolidate common services for consistency and
    scale.
-   **Federated model:** central guardrails with domain-level autonomy.
-   **Centre of Excellence:** central expertise, standards and
    enablement.
-   **Platform operating model:** provide reusable internal capabilities
    as products.
-   **Product-aligned teams:** persistent teams own products or
    capabilities across their lifecycle.
-   **Outsourced / managed service:** transfer defined responsibilities
    under explicit service and control agreements.

Each model creates trade-offs between autonomy, standardisation, scale,
responsiveness and accountability.

<a id="4-4-business-process-patterns"></a>

#### 4.4 Business process patterns

-   **Sequential workflow:** activities execute in a defined order.
-   **Parallel workflow:** independent activities execute concurrently.
-   **Conditional branching:** route based on business rules.
-   **Event-triggered process:** a business event initiates work.
-   **Human-in-the-loop:** a person reviews, approves or completes a
    step.
-   **Exception handling:** explicitly manage rejected, failed,
    incomplete and unusual cases.
-   **Four-eyes principle:** separate initiation and approval for
    sensitive actions.
-   **Maker-checker:** one person prepares an action and another
    authorises it.
-   **Straight-through processing:** automate eligible cases without
    manual intervention.
-   **Case management:** support dynamic paths and human judgement.
-   **Business rules engine:** externalise selected rules for controlled
    change.
-   **Decision management:** separate decision logic, evidence and
    execution.

<a id="4-5-business-architecture-anti-patterns"></a>

#### 4.5 Business architecture anti-patterns

-   Treating an application map as a business capability map.
-   Designing around current departments rather than business outcomes.
-   Automating broken processes without examining them.
-   Creating capabilities with no accountable owner.
-   Measuring activity volume instead of business outcomes.
-   Designing the happy path while leaving exceptions to manual
    workarounds.

---

<a id="part-ii-solution-and-application-architecture"></a>

## 🧩 Part II · Solution and application architecture

`PHASE 02` · `BUILDING BLOCKS` · **Chapters 5–10**

Explore how responsibilities become application boundaries, domain models, interfaces and distributed workflows. Compare the operational cost of a pattern as carefully as its code structure.

> **💡 Key insight**
>
> Independent deployment is valuable only when ownership, contracts and operations support it.


<a id="5-architectural-styles-and-topologies"></a>

### 5. Architectural styles and topologies

An architectural style describes the broad organisation of a system.
Styles can be combined; they are not mutually exclusive.

| Style | Description | Good fit | Main trade-offs |
| --- | --- | --- | --- |
| Monolithic | One deployable application, often sharing a runtime and data store | Small or cohesive systems, early products | Simple deployment initially; growing change and scaling constraints |
| Modular monolith | One deployable unit with explicit internal modules and boundaries | Strong domain cohesion without distribution needs | Requires boundary discipline; shared runtime and release |
| Layered / n-tier | Responsibilities separated into presentation, application, domain and infrastructure layers | Business applications with clear separation of concerns | Can become overly coupled or pass-through layers |
| Client-server | Clients request services from server-side components | Interactive and centralised applications | Server dependency and network latency |
| Service-oriented architecture (SOA) | Business-aligned services exposed through contracts, often with enterprise integration | Large heterogeneous enterprise integration | Governance and middleware can become heavy |
| Microservices | Independently deployable services organised around business capabilities or bounded contexts | Domains needing independent ownership, scaling and release | Distributed data, operations, latency and consistency complexity |
| Event-driven architecture (EDA) | Components react to events through asynchronous communication | Decoupled workflows, integration and streaming | Eventual consistency, event governance and debugging |
| Pipe-and-filter | Data flows through independent transformation stages | ETL, streaming and processing pipelines | Ordering, error handling and replay complexity |
| Hexagonal / ports and adapters | Domain/application core interacts through ports implemented by adapters | Testable domain logic and replaceable infrastructure | Requires disciplined boundary design |
| Microkernel / plug-in | Small core extended by independent plug-ins | Extensible products and platforms | Plug-in compatibility and lifecycle complexity |
| Blackboard | Multiple specialised components contribute to a shared knowledge space | Some AI, signal-processing and problem-solving systems | Shared-state coordination and explainability |
| Peer-to-peer | Nodes act as both clients and servers | Distributed collaboration and decentralised networks | Discovery, trust, consistency and operations |
| Serverless | Managed execution and infrastructure abstraction | Variable workloads, event processing and rapid delivery | Platform constraints, cold starts, observability and cost behaviour |
| Space-based | Processing and data distributed across processing units to reduce central bottlenecks | High-volume, low-latency workloads | Complexity of partitioning and consistency |
| Micro-frontend | Independently delivered frontend sections composed into an experience | Large frontend domains with independent teams | UX consistency, runtime integration and performance |

<a id="5-1-choosing-an-architectural-style"></a>

#### 5.1 Choosing an architectural style

Assess:

-   Business and domain complexity.
-   Required independent deployment and scaling.
-   Team topology, skills and ownership.
-   Data ownership and consistency needs.
-   Availability, latency and throughput targets.
-   Integration landscape and legacy constraints.
-   Security, regulatory and audit requirements.
-   Operational maturity and observability.
-   Cost, licensing and exit strategy.
-   Expected rate and direction of change.

**Default recommendation:** Start with a modular design and introduce
distribution where there is a defensible need. Microservices are an
organisational and operational choice as much as a code-structuring
choice.

<a id="6-application-architecture-principles"></a>

### 6. Application architecture principles

<a id="6-1-structural-principles"></a>

#### 6.1 Structural principles

-   Separation of concerns.
-   High cohesion and low coupling.
-   Explicit module and service boundaries.
-   Dependency inversion.
-   Encapsulation and information hiding.
-   Composition over inheritance where it improves flexibility.
-   Prefer explicit dependencies over hidden global state.
-   Keep business rules independent of delivery and persistence concerns
    where practical.
-   Make side effects visible.
-   Avoid cyclic dependencies.
-   Keep contracts stable and implementation replaceable.
-   Make failure and timeout behaviour explicit.

<a id="6-2-solid-principles"></a>

#### 6.2 SOLID principles

| Principle | Meaning |
| --- | --- |
| Single Responsibility | A module should have one coherent reason to change |
| Open/Closed | Software entities should be extensible without repeatedly modifying stable code |
| Liskov Substitution | Subtypes should preserve the behavioural expectations of their base abstractions |
| Interface Segregation | Consumers should not depend on interfaces they do not use |
| Dependency Inversion | High-level policy should not depend directly on low-level implementation details; both should depend on abstractions |

SOLID is a set of object-oriented design principles, not a complete
architecture method. Apply the intent rather than mechanically creating
interfaces and abstractions everywhere.

<a id="7-domain-driven-design-patterns"></a>

### 7. Domain-driven design patterns

DDD is particularly useful where business rules and domain language are
complex.

<a id="7-1-strategic-ddd"></a>

#### 7.1 Strategic DDD

-   **Domain:** the business problem space.
-   **Core domain:** the area that provides distinctive business
    advantage.
-   **Supporting subdomain:** necessary business capability that
    supports the core.
-   **Generic subdomain:** common capability that may be purchased or
    reused.
-   **Bounded context:** an explicit boundary within which a domain
    model and language have consistent meaning.
-   **Ubiquitous language:** shared terminology used by domain experts
    and delivery teams.
-   **Context map:** describes relationships and integration between
    bounded contexts.
-   **Anti-corruption layer:** protects one model from another model's
    concepts and constraints.
-   **Shared kernel:** a deliberately shared subset of a domain model,
    with coordinated ownership.
-   **Customer-supplier:** upstream and downstream relationship between
    contexts.
-   **Conformist:** downstream adopts the upstream model.
-   **Open-host service:** upstream provides a published integration
    protocol.
-   **Published language:** shared interchange model or schema.

<a id="7-2-tactical-ddd"></a>

#### 7.2 Tactical DDD

-   **Entity:** object with identity and lifecycle.
-   **Value object:** immutable or value-equal concept without
    independent identity.
-   **Aggregate:** consistency boundary containing related domain
    objects.
-   **Aggregate root:** entry point enforcing aggregate invariants.
-   **Repository:** abstraction for retrieving and persisting
    aggregates.
-   **Domain service:** domain operation that does not naturally belong
    to one entity or value object.
-   **Domain event:** fact that something meaningful happened in the
    domain.
-   **Application service:** coordinates a use case without owning core
    domain rules.
-   **Factory:** encapsulates complex creation.
-   **Specification:** encapsulates a business rule or selection
    predicate.
-   **Policy:** represents a rule that governs behaviour.
-   **Module:** groups cohesive domain concepts.

**Important:** An aggregate is not simply a database table or a
collection of every related entity. Keep aggregates small enough to
enforce the invariants that must be consistent together. Cross-aggregate
workflows often require eventual consistency.

<a id="8-application-design-and-implementation-patterns"></a>

### 8. Application design and implementation patterns

<a id="8-1-layering-and-application-structure"></a>

#### 8.1 Layering and application structure

-   **Presentation layer:** handles user or external interaction.
-   **Application layer / service layer:** coordinates use cases and
    transaction boundaries.
-   **Domain layer:** models business concepts, policies and invariants.
-   **Infrastructure layer:** implements persistence, messaging,
    external integrations and technical concerns.
-   **Clean architecture:** dependencies point inward toward policy and
    domain rules.
-   **Onion architecture:** concentric layers with domain at the centre
    and infrastructure at the edge.
-   **Hexagonal architecture:** ports define interactions; adapters
    implement them.
-   **Vertical slice architecture:** organise code by use case or
    feature rather than only technical layer.
-   **Feature folders:** co-locate code that changes together.
-   **Plugin architecture:** extend a stable core through defined
    extension points.

These are related approaches, not exact synonyms. Their common goal is
to protect important policy from volatile implementation details.

<a id="8-2-enterprise-application-patterns"></a>

#### 8.2 Enterprise application patterns

-   Transaction Script.
-   Domain Model.
-   Table Module.
-   Service Layer.
-   Data Mapper.
-   Active Record.
-   Table Data Gateway.
-   Row Data Gateway.
-   Unit of Work.
-   Identity Map.
-   Lazy Load.
-   Data Transfer Object (DTO).
-   Repository.
-   Gateway.
-   Remote Facade.
-   Service Stub.
-   Registry.
-   Value Object.
-   Special Case / Null Object.
-   Separated Interface.
-   Optimistic Offline Lock.
-   Pessimistic Offline Lock.
-   Coarse-Grained Lock.
-   Identity Field.
-   Foreign Key Mapping.
-   Association Table Mapping.
-   Embedded Value.
-   Single Table Inheritance.
-   Class Table Inheritance.
-   Concrete Table Inheritance.

These patterns solve different problems. For example, Active Record
couples domain behaviour to persistence conventions, while Data Mapper
separates them. Neither is universally superior.

<a id="8-3-object-oriented-and-component-design-patterns"></a>

#### 8.3 Object-oriented and component design patterns

**Creational** - Factory Method. - Abstract Factory. - Builder. -
Prototype. - Singleton (use cautiously; hidden global state and test
coupling are risks).

**Structural** - Adapter. - Bridge. - Composite. - Decorator. -
Facade. - Flyweight. - Proxy.

**Behavioural** - Chain of Responsibility. - Command. - Interpreter. -
Iterator. - Mediator. - Memento. - Observer. - State. - Strategy. -
Template Method. - Visitor.

<a id="8-4-common-application-patterns"></a>

#### 8.4 Common application patterns

-   MVC (Model-View-Controller).
-   MVP (Model-View-Presenter).
-   MVVM (Model-View-ViewModel).
-   Front Controller.
-   Page Controller.
-   Presentation Model.
-   Backend for Frontend (BFF).
-   API Facade.
-   Gateway Aggregation.
-   Service Locator (use cautiously).
-   Dependency Injection.
-   Interceptor / Middleware.
-   Pipeline.
-   Policy-based authorisation.
-   Idempotent command handler.
-   Validation pipeline.
-   Specification.
-   Result type / explicit error model.
-   Functional core, imperative shell.

<a id="9-api-and-interface-architecture-patterns"></a>

### 9. API and interface architecture patterns

<a id="9-1-api-styles-and-interaction-models"></a>

#### 9.1 API styles and interaction models

-   REST / resource-oriented HTTP APIs.
-   RPC, including gRPC.
-   GraphQL.
-   SOAP / WS-\* where legacy or standards requirements justify it.
-   Webhooks.
-   WebSocket for bidirectional communication.
-   Server-Sent Events for server-to-client streaming.
-   Asynchronous request-reply.
-   Batch interfaces and file-based exchange.
-   Event and message contracts.

Choose based on consumer needs, interaction semantics, latency,
payloads, governance and operational support. Do not expose GraphQL,
REST or gRPC merely because it is fashionable.

<a id="9-2-api-design-principles"></a>

#### 9.2 API design principles

-   Design from consumer use cases.
-   Define resource and domain semantics clearly.
-   Use consistent naming, status codes and error structures.
-   Define pagination, filtering, sorting and field selection.
-   Use explicit validation and error contracts.
-   Support idempotency for retryable state-changing operations where
    appropriate.
-   Apply authentication, authorisation, throttling and quotas.
-   Set request size, timeout and rate limits.
-   Version deliberately and prefer compatible evolution.
-   Publish machine-readable contracts and examples.
-   Test compatibility and consumer expectations.
-   Avoid leaking persistence schemas as public contracts.
-   Do not use HTTP methods as a substitute for business semantics.
-   Define correlation and trace identifiers.

<a id="9-3-api-patterns"></a>

#### 9.3 API patterns

-   API Gateway.
-   Backend for Frontend.
-   Gateway Aggregation.
-   API Composition.
-   API Proxy.
-   Anti-corruption Layer.
-   Facade.
-   Adapter.
-   Strangler Fig routing.
-   Consumer-driven contract testing.
-   API versioning.
-   Expand-and-contract schema evolution.
-   Idempotency key.
-   Rate limiting and quota.
-   Pagination: offset, cursor/keyset and continuation token.
-   Long-running operation resource / job status.
-   Webhook subscription and delivery.
-   GraphQL federation (with ownership and composition governance).

<a id="9-4-api-anti-patterns"></a>

#### 9.4 API anti-patterns

-   Chatty APIs requiring many round trips.
-   One universal API for unrelated consumers.
-   Leaking internal database structures.
-   Breaking changes without migration.
-   Unbounded list endpoints.
-   Synchronous chains across many services.
-   Retrying non-idempotent writes without protection.
-   Treating API Gateway as a substitute for domain boundaries.
-   Duplicating business rules in multiple API layers.

<a id="10-microservices-and-distributed-application-patterns"></a>

### 10. Microservices and distributed application patterns

<a id="10-1-service-decomposition"></a>

#### 10.1 Service decomposition

-   Decompose by bounded context or business capability.
-   Align service boundaries with cohesive data and behaviour.
-   Use business transactions and invariants to inform boundaries.
-   Avoid one service per database table.
-   Avoid splitting tightly coupled operations merely to achieve a
    microservice count.
-   Prefer independently deployable services with clear ownership.
-   Make synchronous and asynchronous dependencies explicit.

<a id="10-2-service-interaction-patterns"></a>

#### 10.2 Service interaction patterns

-   Synchronous request-response.
-   Asynchronous messaging.
-   Publish-subscribe.
-   Event notification.
-   Event-carried state transfer.
-   Request-reply over messaging.
-   Scatter-gather.
-   Fan-out / fan-in.
-   Competing consumers.
-   Sequential convoy.
-   Pipes and filters.
-   Content-based routing.
-   Claim check for large payloads.
-   Message bridge.
-   Message translator.
-   Dead-letter channel.
-   Priority queue.
-   Resequencer.
-   Message filter.
-   Idempotent receiver.
-   Transactional outbox.
-   Inbox / deduplication.
-   Change Data Capture (CDC).

<a id="10-3-distributed-transaction-and-consistency-patterns"></a>

#### 10.3 Distributed transaction and consistency patterns

-   **Saga choreography:** participants react to events and progress a
    multi-step business transaction.
-   **Saga orchestration:** a coordinator directs the steps and tracks
    workflow state.
-   **Transactional outbox:** persist business change and outgoing event
    record atomically, then publish asynchronously.
-   **Inbox / idempotent consumer:** record processed message
    identifiers to suppress duplicate effects.
-   **Compensating transaction:** perform a business action that
    semantically counteracts a prior action.
-   **Process manager:** maintain state and coordinate a long-running
    process.
-   **Two-phase commit:** coordinate a distributed transaction where
    participants and infrastructure support the protocol; consider
    blocking and availability implications.
-   **TCC (Try-Confirm-Cancel):** reserve resources and later confirm or
    cancel.
-   **Optimistic concurrency:** detect conflicting updates using
    versions or tokens.
-   **Pessimistic locking:** prevent concurrent conflicting work through
    locks.
-   **Eventual consistency:** replicas or services converge after
    asynchronous propagation.
-   **Read-your-writes / session consistency:** provide a consistency
    guarantee within a user or session context where needed.

Do not promise exactly-once business effects simply because a broker
offers an exactly-once feature. End-to-end semantics depend on the
source, broker, consumer, database and external side effects. Design for
duplicates, retries and replay.

<a id="10-4-resilience-patterns"></a>

#### 10.4 Resilience patterns

-   Timeout.
-   Retry with bounded exponential backoff and jitter.
-   Circuit Breaker.
-   Bulkhead.
-   Rate Limiter.
-   Load Shedding.
-   Queue-Based Load Leveling.
-   Backpressure.
-   Health Endpoint Monitoring.
-   Fail Fast.
-   Fallback.
-   Graceful Degradation.
-   Leader Election.
-   Lease / heartbeat.
-   Scheduler-Agent-Supervisor.
-   Hedged Requests (only where safe and appropriate).
-   Replication and failover.
-   Retry budget.

**Important:** Retries can amplify overload. Use timeouts, bounded
attempts, jitter, idempotency and retry budgets. Do not retry permanent
business validation failures.

<a id="10-5-distributed-systems-concerns"></a>

#### 10.5 Distributed systems concerns

Every distributed architecture should explicitly address:

-   Partial failure.
-   Network partitions and latency.
-   Duplicate, delayed and out-of-order messages.
-   Clock skew and timestamp semantics.
-   Concurrent updates and lost writes.
-   Data ownership and consistency.
-   Service discovery and endpoint changes.
-   Backward and forward compatibility.
-   Observability across process boundaries.
-   Secrets and identity between workloads.
-   Deployment ordering and compatibility.
-   Replay, reprocessing and poison messages.

---

<a id="part-iii-integration-architecture"></a>

## 🔗 Part III · Integration architecture

`PHASE 02` · `BUILDING BLOCKS` · **Chapters 11–12**

Choose interaction styles according to business semantics, then design message construction, routing, transformation and delivery behaviour explicitly.

> **💡 Key insight**
>
> Commands request actions; events describe facts. Contracts must make that distinction clear.


<a id="11-integration-styles"></a>

### 11. Integration styles

| Style | Characteristics | Appropriate use |
| --- | --- | --- |
| Point-to-point | Direct connection between systems | Small, stable number of integrations |
| Shared database | Systems integrate through common tables | Usually legacy or tightly controlled cases; creates ownership coupling |
| File transfer | Scheduled exchange through files | Batch, partner and legacy integration |
| Shared messaging broker | Producers and consumers exchange messages | Asynchronous enterprise integration |
| API-led integration | Systems expose governed APIs | Synchronous queries and commands |
| Event-driven integration | Consumers react to published facts | Decoupled state-change propagation |
| Enterprise Service Bus | Central mediation, routing and transformation | Existing enterprise integration estates where justified |
| iPaaS | Managed integration and workflow capabilities | SaaS and enterprise application integration |
| Data integration | Bulk or incremental data movement | Analytics, reporting and data platforms |
| CDC integration | Propagate committed database changes | Replication and integration where source semantics are understood |

Avoid assuming one integration style should handle every interaction. A
user waiting for confirmation, a scheduled reconciliation and a domain
event have different interaction needs.

<a id="12-enterprise-integration-patterns-eip"></a>

### 12. Enterprise Integration Patterns (EIP)

<a id="12-1-message-construction"></a>

#### 12.1 Message construction

-   Message.
-   Command Message.
-   Document Message.
-   Event Message.
-   Request-Reply.
-   Correlation Identifier.
-   Message Sequence.
-   Message Expiration.
-   Format Indicator.
-   Claim Check.

<a id="12-2-message-channels"></a>

#### 12.2 Message channels

-   Point-to-Point Channel.
-   Publish-Subscribe Channel.
-   Datatype Channel.
-   Invalid Message Channel.
-   Dead Letter Channel.
-   Guaranteed Delivery.
-   Channel Adapter.
-   Messaging Bridge.

<a id="12-3-message-routing"></a>

#### 12.3 Message routing

-   Content-Based Router.
-   Message Filter.
-   Dynamic Router.
-   Recipient List.
-   Splitter.
-   Aggregator.
-   Resequencer.
-   Routing Slip.
-   Process Manager.
-   Scatter-Gather.

<a id="12-4-message-transformation"></a>

#### 12.4 Message transformation

-   Message Translator.
-   Envelope Wrapper.
-   Content Enricher.
-   Content Filter.
-   Claim Check.
-   Normalizer.
-   Canonical Data Model.

<a id="12-5-message-endpoints"></a>

#### 12.5 Message endpoints

-   Messaging Gateway.
-   Messaging Mapper.
-   Transactional Client.
-   Polling Consumer.
-   Event-Driven Consumer.
-   Competing Consumers.
-   Message Dispatcher.
-   Selective Consumer.
-   Idempotent Receiver.

<a id="12-6-integration-contract-best-practices"></a>

#### 12.6 Integration contract best practices

-   Give each event a clear business meaning and owner.
-   Distinguish a command (request to do something) from an event (fact
    that something happened).
-   Use stable identifiers, event type, schema version, occurrence time
    and correlation/causation identifiers.
-   Define ordering scope explicitly; global ordering is expensive and
    rarely necessary.
-   Partition by the key that defines the required ordering boundary.
-   Make consumers idempotent.
-   Define retry, poison-message and dead-letter handling.
-   Make replay and reprocessing safe.
-   Govern schema evolution and compatibility.
-   Avoid publishing sensitive data unnecessarily.
-   Document delivery guarantees and operational ownership.
-   Do not treat a database row change as a meaningful business event
    without domain interpretation.

<a id="12-7-canonical-data-model-use-with-care"></a>

#### 12.7 Canonical data model: use with care

A canonical model can reduce pairwise transformation complexity in a
large integration estate, but it can become a central bottleneck and
lowest-common-denominator schema. Use bounded canonical models where
they create clear value; do not force every domain into one enterprise
mega-schema.

---

<a id="part-iv-data-architecture"></a>

## 🗄️ Part IV · Data architecture

`PHASE 02` · `BUILDING BLOCKS` · **Chapters 13–16**

Connect business meaning and accountable ownership to data models, platforms, movement, quality and lifecycle management.

> **💡 Key insight**
>
> A controlled copy is useful only when authority, freshness, reconciliation and deletion are explicit.


<a id="13-data-architecture-principles"></a>

### 13. Data architecture principles

1.  Business meaning and ownership precede physical technology.
2.  Identify systems of record and authoritative sources for critical
    facts.
3.  Separate operational data needs from analytical data needs where
    their workload and lifecycle differ.
4.  Model data at conceptual, logical and physical levels.
5.  Define data quality rules with owners and measurable thresholds.
6.  Treat metadata, lineage and classification as first-class assets.
7.  Minimise duplication, but recognise that controlled replication can
    improve decoupling, performance and availability.
8.  Make data contracts explicit between producers and consumers.
9.  Govern access at the appropriate layer and enforce controls close to
    the data.
10. Apply retention, archival and deletion consistently across copies
    and derived data.
11. Make data products discoverable, trustworthy, secure and usable.
12. Preserve provenance and auditability for consequential data
    transformations.
13. Choose storage based on access patterns, consistency, latency, scale
    and lifecycle.
14. Do not confuse physical centralisation with logical ownership.
15. Define freshness and quality expectations for each consumer use
    case.

<a id="14-data-modelling-patterns"></a>

### 14. Data modelling patterns

<a id="14-1-modelling-levels"></a>

#### 14.1 Modelling levels

-   **Conceptual model:** major business concepts and relationships.
-   **Logical model:** attributes, identifiers, relationships,
    cardinality and business constraints.
-   **Physical model:** tables, columns, data types, indexes, partitions
    and storage structures.
-   **Canonical / interchange model:** shared representation for a
    specific integration boundary.
-   **Dimensional model:** facts and dimensions for analytical
    consumption.
-   **Data vault model:** hubs, links and satellites for historised
    integration and auditability.
-   **Normalised model:** reduce update anomalies and represent
    transactional data.
-   **Denormalised model:** optimise read and analytical access patterns
    where justified.
-   **Graph model:** nodes, edges and properties for highly connected
    data.
-   **Document model:** aggregate-oriented semi-structured records.
-   **Key-value model:** lookup by key.
-   **Time-series model:** measurements indexed by time.
-   **Wide-column model:** sparse, distributed data access patterns.
-   **Event model:** immutable facts representing state changes.

<a id="14-2-relational-modelling-patterns"></a>

#### 14.2 Relational modelling patterns

-   One-to-one, one-to-many and many-to-many relationships.
-   Surrogate key and natural key.
-   Composite key.
-   Bridge / associative table.
-   Supertype-subtype.
-   Table-per-hierarchy.
-   Table-per-type.
-   Effective-dated records.
-   Slowly Changing Dimensions (Types 0--6, depending on the chosen
    model and implementation).
-   Temporal tables / bitemporal modelling.
-   Soft delete and tombstone (with explicit retention and privacy
    implications).
-   Audit history.
-   Status history.
-   Hierarchical data: adjacency list, closure table, nested set,
    materialised path.
-   Reference data and code sets.
-   Master data and golden record.

<a id="14-3-data-type-and-physical-design-practices"></a>

#### 14.3 Data type and physical design practices

-   Use types that reflect semantics and valid ranges.
-   Avoid storing dates, quantities and numeric values as arbitrary
    strings.
-   Use decimal types for exact financial quantities; define scale and
    rounding rules.
-   Choose identifiers based on lifecycle, distribution and
    interoperability needs.
-   Understand UUID storage, index locality and sequential-key
    trade-offs for the selected database.
-   Index based on query patterns and selectivity, not intuition alone.
-   Consider partitioning or clustering only where measured workload and
    pruning behaviour justify it.
-   Avoid excessive indexes on write-heavy tables.
-   Define constraints for integrity where supported and appropriate.
-   Avoid overusing JSON/VARIANT for attributes that need strong
    relational semantics, constraints or frequent joins.
-   Preserve source identifiers and provenance in integrated datasets.

<a id="15-data-architecture-styles-and-platform-patterns"></a>

### 15. Data architecture styles and platform patterns

<a id="15-1-operational-data-patterns"></a>

#### 15.1 Operational data patterns

-   OLTP relational database.
-   Operational Data Store (ODS).
-   Master Data Management (MDM).
-   Reference Data Management.
-   Transactional database per service.
-   Shared operational database (with explicit ownership and coupling
    controls).
-   Read replica.
-   Materialised view.
-   Search index.
-   Cache.
-   Database sharding.
-   Partitioning.
-   Multi-region replication.
-   Database-per-tenant.
-   Schema-per-tenant.
-   Row-level tenant isolation.

<a id="15-2-analytical-data-platform-patterns"></a>

#### 15.2 Analytical data platform patterns

-   Enterprise Data Warehouse (EDW).
-   Data mart.
-   Operational Data Store.
-   Data lake.
-   Lakehouse.
-   Data lakehouse with open table formats.
-   Medallion architecture (Bronze / Silver / Gold).
-   Lambda architecture (batch plus speed layer).
-   Kappa architecture (stream-processing-centric).
-   Data mesh.
-   Data fabric.
-   Data hub.
-   Federated query.
-   Logical data warehouse.
-   Semantic layer.
-   Feature store.
-   Vector data store (for embedding/vector retrieval use cases).

These are not all competing alternatives. For example, a lakehouse is a
platform architecture, medallion is a data organisation pattern, and
data mesh is an organisational and ownership approach.

<a id="15-3-data-movement-and-processing-patterns"></a>

#### 15.3 Data movement and processing patterns

-   ETL.
-   ELT.
-   Batch ingestion.
-   Micro-batch ingestion.
-   Streaming ingestion.
-   Change Data Capture.
-   Log-based replication.
-   Snapshot ingestion.
-   Full refresh.
-   Incremental load.
-   Watermark-based extraction.
-   High-water mark.
-   Backfill.
-   Replay.
-   Late-arriving data handling.
-   Deduplication.
-   Schema-on-read.
-   Schema-on-write.
-   Data federation.
-   Data virtualisation.
-   Data sharing.
-   Reverse ETL.
-   Data synchronisation.
-   Reconciliation and control totals.

<a id="15-4-data-transformation-and-modelling-patterns"></a>

#### 15.4 Data transformation and modelling patterns

-   Staging layer.
-   Persistent staging.
-   One Big Table (use selectively).
-   Star schema.
-   Snowflake schema.
-   Fact constellation.
-   Transaction fact.
-   Periodic snapshot fact.
-   Accumulating snapshot fact.
-   Conformed dimensions.
-   Shared dimensions.
-   Data Vault hubs, links and satellites.
-   Anchor modelling.
-   Entity resolution.
-   Record linkage.
-   Survivorship rules.
-   Semantic model.
-   Aggregate tables.
-   Materialised views.
-   Data quality quarantine.

<a id="15-5-data-mesh-principles-and-practices"></a>

#### 15.5 Data mesh principles and practices

Data mesh is an organisational and architectural approach commonly
described through four principles:

1.  Domain-oriented decentralised data ownership.
2.  Data as a product.
3.  Self-serve data platform.
4.  Federated computational governance.

Practical data product expectations:

-   Named domain owner and product owner.
-   Explicit consumers and supported use cases.
-   Discoverable catalogue entry.
-   Business definitions and technical schema.
-   Data contract and compatibility policy.
-   Quality dimensions and measurable SLOs.
-   Freshness and availability expectations.
-   Lineage and provenance.
-   Classification and access policy.
-   Support and incident process.
-   Versioning and deprecation.
-   Cost visibility.
-   Clear lifecycle and retirement process.

A data product is not simply a table, dashboard or pipeline. It is a
governed, supported data asset with an intentional consumer interface
and operational expectations.

<a id="15-6-data-governance-and-management-disciplines"></a>

#### 15.6 Data governance and management disciplines

DAMA-DMBOK commonly organises data management into knowledge areas
including:

-   Data Governance.
-   Data Architecture.
-   Data Modelling and Design.
-   Data Storage and Operations.
-   Data Security.
-   Data Integration and Interoperability.
-   Document and Content Management.
-   Reference and Master Data.
-   Data Warehousing and Business Intelligence.
-   Metadata Management.
-   Data Quality.

Associated practices:

-   Data owner, data steward and data custodian roles.
-   Business glossary.
-   Data catalogue.
-   Metadata repository.
-   Data lineage.
-   Critical data elements.
-   Classification and handling.
-   Access certification.
-   Data quality rules and scorecards.
-   Data issue management.
-   Retention and disposal.
-   Privacy impact assessment.
-   Data sharing agreements.
-   Data contract governance.
-   Model governance where applicable.

<a id="15-7-data-consistency-and-ownership-decisions"></a>

#### 15.7 Data consistency and ownership decisions

For every data flow, decide:

-   Who owns the source fact?
-   Which system is authoritative for updates?
-   Is the consumer querying live data, a replica, a projection or a
    snapshot?
-   What consistency and freshness are required?
-   Is replication justified by scale, availability, decoupling, latency
    or analytical workload?
-   How are changes, deletes and corrections propagated?
-   How are drift and reconciliation detected?
-   Who resolves conflicting updates?
-   What is the retention and deletion behaviour of downstream copies?

**Avoid two extremes:** duplicating data without a clear purpose, and
forcing every consumer to query one operational database. Controlled
copies and projections are legitimate when ownership, freshness,
reconciliation and lifecycle are explicit.

<a id="16-data-quality-patterns"></a>

### 16. Data quality patterns

-   Validation at ingestion.
-   Validation at transformation.
-   Contract validation.
-   Schema validation.
-   Referential integrity checks.
-   Uniqueness and duplicate detection.
-   Completeness checks.
-   Validity and conformity checks.
-   Accuracy verification against trusted sources.
-   Timeliness and freshness monitoring.
-   Reconciliation and balancing.
-   Anomaly detection.
-   Quarantine and remediation.
-   Data quality scorecards.
-   Data observability.
-   SLO-based quality management.

Quality dimensions should be selected based on data use. A single
generic quality score can conceal important defects.

---

<a id="part-v-security-privacy-and-trust-architecture"></a>

## 🛡️ Part V · Security, privacy and trust architecture

`PHASE 02` · `BUILDING BLOCKS` · **Chapters 17–18**

Make identity, trust boundaries, information protection and verification part of the design. Use these chapters alongside every other domain, not only at review time.

> **💡 Key insight**
>
> Security controls need evidence of enforcement, not just a place in an architecture diagram.


<a id="17-security-architecture-principles"></a>

### 17. Security architecture principles

-   Identify and protect critical assets.
-   Establish trust boundaries.
-   Authenticate users, workloads and devices.
-   Authorise each resource operation.
-   Apply least privilege and separation of duties.
-   Use strong identity lifecycle management.
-   Protect data at rest, in transit and in use where feasible.
-   Centralise policy where appropriate, but enforce controls at
    resource boundaries.
-   Log and monitor security-relevant activity.
-   Design for detection, containment and recovery.
-   Threat model significant changes and integrations.
-   Secure software supply chains and deployment pipelines.
-   Rotate and protect credentials and secrets.
-   Test controls, not just document them.

<a id="18-security-patterns"></a>

### 18. Security patterns

<a id="18-1-identity-and-access"></a>

#### 18.1 Identity and access

-   Identity Provider (IdP).
-   Federated Identity.
-   Single Sign-On (SSO).
-   Multi-Factor Authentication (MFA).
-   OAuth 2.0 authorisation.
-   OpenID Connect authentication.
-   SAML federation.
-   Workload identity.
-   Managed identity.
-   Role-Based Access Control (RBAC).
-   Attribute-Based Access Control (ABAC).
-   Policy-Based Access Control (PBAC).
-   Relationship-Based Access Control (ReBAC).
-   Just-in-Time access.
-   Privileged Access Management (PAM).
-   Separation of duties.
-   Entitlement review and access recertification.
-   Delegated authorisation and scoped tokens.

<a id="18-2-zero-trust-and-network-security"></a>

#### 18.2 Zero Trust and network security

-   Zero Trust Architecture.
-   Explicit verification.
-   Least-privilege access.
-   Assume breach.
-   Micro-segmentation.
-   Software-defined perimeter.
-   Secure service-to-service identity.
-   Mutual TLS.
-   Private endpoints and controlled ingress/egress.
-   Network zones and trust boundaries.
-   Web Application Firewall.
-   API protection and threat detection.
-   DNS security and egress controls.

Zero Trust is not a product or a single network design. It is a security
model focused on protecting resources and evaluating access explicitly.

<a id="18-3-data-protection"></a>

#### 18.3 Data protection

-   Encryption at rest and in transit.
-   Envelope encryption.
-   Key management and rotation.
-   Tokenisation.
-   Masking.
-   Dynamic data masking.
-   Static masking for non-production.
-   Pseudonymisation.
-   Anonymisation (subject to re-identification risk).
-   Data loss prevention.
-   Secrets management.
-   Data classification and handling.
-   Field-level protection.
-   Row-level and column-level security.
-   Confidential computing where justified.

<a id="18-4-application-security-patterns"></a>

#### 18.4 Application security patterns

-   Input validation.
-   Output encoding.
-   Parameterised queries.
-   Content Security Policy.
-   CSRF protection.
-   Secure session management.
-   Rate limiting.
-   Secure error handling.
-   Threat modelling.
-   Security headers.
-   Dependency and vulnerability scanning.
-   Software bill of materials (SBOM).
-   Signed artefacts.
-   Secure build pipeline.
-   Runtime protection and detection.

<a id="18-5-security-architecture-models-and-methods"></a>

#### 18.5 Security architecture models and methods

-   CIA triad: confidentiality, integrity, availability.
-   STRIDE threat modelling.
-   Attack trees.
-   PASTA threat analysis.
-   NIST Cybersecurity Framework.
-   NIST SP 800-207 Zero Trust Architecture.
-   SABSA.
-   ISO/IEC 27001 information security management.
-   OWASP ASVS and OWASP Top 10 as application security references.

Use the relevant current editions and organisational regulatory
obligations when establishing control baselines.

---

<a id="part-vi-infrastructure-cloud-and-platform-architecture"></a>

## ☁️ Part VI · Infrastructure, cloud and platform architecture

`PHASE 02` · `BUILDING BLOCKS` · **Chapters 19–20**

Evaluate hosting, networks, release strategies and platform capabilities against workload needs. Treat availability and recovery as business-service characteristics.

> **💡 Key insight**
>
> A backup is not proof of recoverability; restoration and recovery must be exercised.


<a id="19-infrastructure-architecture-patterns"></a>

### 19. Infrastructure architecture patterns

<a id="19-1-compute-and-hosting"></a>

#### 19.1 Compute and hosting

-   Virtual machines.
-   Containers.
-   Kubernetes orchestration.
-   Platform as a Service.
-   Function as a Service.
-   Serverless event processing.
-   Managed application platforms.
-   Batch compute.
-   High-performance compute.
-   Edge compute.
-   Hybrid cloud.
-   Multi-cloud.
-   Private cloud.
-   Cloud landing zone.
-   Multi-account / subscription architecture.
-   Deployment stamps.
-   Cell-based architecture.
-   Multi-tenant hosting.

<a id="19-2-network-architecture"></a>

#### 19.2 Network architecture

-   Hub-and-spoke.
-   Virtual network segmentation.
-   Shared services network.
-   Transit gateway / network hub.
-   DMZ.
-   Private connectivity.
-   VPN.
-   Dedicated private circuits.
-   Service mesh.
-   API gateway ingress.
-   Egress proxy.
-   DNS-based service discovery.
-   Network micro-segmentation.
-   Zero-trust access.

<a id="19-3-deployment-and-release-patterns"></a>

#### 19.3 Deployment and release patterns

-   Blue-green deployment.
-   Canary release.
-   Rolling deployment.
-   Recreate deployment.
-   A/B testing.
-   Feature toggles.
-   Progressive delivery.
-   Immutable infrastructure.
-   Infrastructure as Code.
-   GitOps.
-   Configuration as code.
-   Deployment rings.
-   Expand-and-contract database migration.
-   Shadow traffic.
-   Dark launch.
-   Rollback and roll-forward strategies.

<a id="19-4-platform-engineering-patterns"></a>

#### 19.4 Platform engineering patterns

-   Internal Developer Platform (IDP).
-   Golden paths.
-   Self-service infrastructure.
-   Reusable service templates.
-   Platform as a product.
-   Paved roads with governed exceptions.
-   Policy as code.
-   Environment provisioning automation.
-   Developer portals and service catalogues.
-   Standardised CI/CD pipelines.
-   Observability platform.
-   Secrets and identity platform.
-   Shared runtime capabilities.
-   Platform SLOs and product ownership.

A platform should reduce cognitive load and improve delivery outcomes.
It should not become a mandatory central gate for every engineering
decision.

<a id="20-availability-disaster-recovery-and-continuity"></a>

### 20. Availability, disaster recovery and continuity

<a id="20-1-availability-patterns"></a>

#### 20.1 Availability patterns

-   Active-active.
-   Active-passive.
-   Multi-AZ / multi-zone.
-   Multi-region.
-   Hot standby.
-   Warm standby.
-   Pilot light.
-   Cold standby.
-   Read replica and failover.
-   Quorum-based replication.
-   Load balancing.
-   Health-based routing.
-   Automated failover.
-   Cell-based isolation.
-   Bulkhead isolation.

<a id="20-2-recovery-concepts"></a>

#### 20.2 Recovery concepts

-   **RTO:** maximum targeted time to restore a service after
    disruption.
-   **RPO:** maximum targeted data loss measured in time.
-   **MTTR:** mean time to repair or recover.
-   **MTBF:** mean time between failures.
-   **SLA:** contractual or externally committed service level.
-   **SLI:** measured indicator of service behaviour.
-   **SLO:** target for an SLI over a defined period.
-   **Error budget:** allowed unreliability implied by an SLO.

Define these per business service and dependency, not only per
infrastructure component.

<a id="20-3-resilience-engineering-practices"></a>

#### 20.3 Resilience engineering practices

-   Dependency mapping.
-   Failure Mode and Effects Analysis (FMEA).
-   Fault-tree analysis.
-   Chaos engineering.
-   Game days.
-   Disaster recovery exercises.
-   Backup restore tests.
-   Capacity and load testing.
-   Dependency failure simulation.
-   Runbooks and playbooks.
-   Incident command and communications.
-   Post-incident review without blame.
-   Recovery validation and data reconciliation.

---

<a id="part-vii-quality-attributes-and-architecture-trade-offs"></a>

## ⚖️ Part VII · Quality attributes and architecture trade-offs

`PHASE 03` · `DECISIONS & DELIVERY` · **Chapters 21–23**

Turn broad aspirations into measurable quality scenarios. Use the trade-off catalogue to explain what each option improves and what it makes harder.

> **💡 Key insight**
>
> A quality requirement is actionable when its operating conditions and response measures are defined.


<a id="21-quality-attribute-catalogue"></a>

### 21. Quality attribute catalogue

Architecture quality must be measurable. Avoid vague requirements such
as "high performance" or "high availability".

| Attribute | Questions and example measures |
| --- | --- |
| Availability | Uptime, successful request ratio, service hours |
| Reliability | Failure rate, recovery success, consistency |
| Performance | p50/p95/p99 latency, throughput, queue delay |
| Scalability | Behaviour as users, data or workload increase |
| Elasticity | Time and accuracy of scaling response |
| Security | Control coverage, vulnerabilities, access violations |
| Privacy | Data minimisation, retention, access and consent compliance |
| Resilience | Recovery time, blast radius, dependency tolerance |
| Maintainability | Change lead time, complexity, defect rate |
| Modifiability | Cost and risk of a representative change |
| Testability | Automation coverage, isolation and repeatability |
| Interoperability | Contract compatibility and integration effort |
| Portability | Effort to move workloads or data |
| Observability | Ability to explain system behaviour from telemetry |
| Operability | Support effort, deployment safety, incident resolution |
| Usability | Task success, error rate, accessibility |
| Accessibility | Conformance to relevant accessibility standards |
| Data quality | Completeness, accuracy, validity, uniqueness, timeliness |
| Cost efficiency | Cost per transaction, workload, customer or data product |
| Sustainability | Energy/resource use and lifecycle impact |

<a id="22-quality-attribute-scenarios"></a>

### 22. Quality attribute scenarios

Write NFRs in a testable form:

-   **Source:** who or what initiates the stimulus?
-   **Stimulus:** what happens?
-   **Environment:** under what operating conditions?
-   **Response:** what must the architecture do?
-   **Response measure:** how will success be measured?

Example:

> During the agreed peak period, when request volume reaches 2,000
> requests per second, 99% of read requests shall complete within 300 ms
> at the service boundary, with no loss of committed transactions.

This is more useful than "the system must be fast and scalable".

<a id="23-common-architecture-trade-offs"></a>

### 23. Common architecture trade-offs

| Decision | Option A | Option B | Main trade-off |
| --- | --- | --- | --- |
| Interaction | Synchronous | Asynchronous | Immediate response and simplicity vs decoupling and eventual completion |
| Architecture | Modular monolith | Microservices | Simpler operations vs independent deployment and scaling |
| Data | Shared database | Database per service | Simpler transactions vs ownership and deployment autonomy |
| Consistency | Strong consistency | Eventual consistency | Immediate coordination vs availability and decoupling |
| Integration | API | Event | Request/response semantics vs propagation of facts |
| Processing | Batch | Streaming | Efficiency and simplicity vs low-latency continuous processing |
| Storage | Normalised | Denormalised | Update integrity vs read optimisation |
| Deployment | Central platform | Team autonomy | Standardisation vs local flexibility |
| Cloud | Single cloud | Multi-cloud | Simplicity and depth vs portability and provider diversity |
| Governance | Centralised | Federated | Consistency vs domain autonomy |
| Reuse | Shared service | Domain-owned capability | Economies of scale vs coupling and release coordination |

No row has a universally correct answer. Record the decision,
constraints and evidence.

---

<a id="part-viii-architecture-governance-and-delivery"></a>

## 📋 Part VIII · Architecture governance and delivery

`PHASE 03` · `DECISIONS & DELIVERY` · **Chapters 24–28**

Agree decision rights, record significant choices and scale documentation to risk. Use the review checklist to connect architecture intent to delivery and operations.

> **💡 Key insight**
>
> Governance should enable sound decisions without becoming approval overhead for every implementation detail.


<a id="24-architecture-governance-practices"></a>

### 24. Architecture governance practices

-   Enterprise architecture principles and standards.
-   Architecture repository and catalogue.
-   Architecture capability and maturity assessment.
-   Architecture review board (ARB), where useful.
-   Design authority and delegated decision rights.
-   Solution architecture review.
-   Security and privacy review.
-   Data architecture review.
-   Technology standards and approved patterns.
-   Exception and waiver management.
-   Architecture compliance assessment.
-   Technical debt register.
-   Architecture risk register.
-   Technology lifecycle and obsolescence management.
-   Reference architectures and reusable building blocks.
-   Architecture runway and transition planning.

Governance should enable good decisions and manage material risk. It
should not require central approval for every low-risk implementation
detail.

<a id="25-architecture-artefacts"></a>

### 25. Architecture artefacts

A proportionate architecture pack may include:

1.  Business context and problem statement.
2.  Business outcomes and success measures.
3.  Scope, assumptions, constraints and dependencies.
4.  Stakeholders and concerns.
5.  Business capability and process impact.
6.  Functional requirements and use cases.
7.  Quality attribute scenarios and NFRs.
8.  Context diagram.
9.  Solution overview and component responsibilities.
10. Application architecture and deployment views.
11. Integration contracts, API and event definitions.
12. Data ownership, models, flows and lineage.
13. Security, privacy and threat model.
14. Resilience, availability and DR design.
15. Operational model, SLOs and support ownership.
16. Technology selection and rationale.
17. Options considered and trade-off analysis.
18. Architecture Decision Records.
19. Risks, mitigations and residual risks.
20. Migration, transition and decommissioning plan.
21. Cost model and FinOps considerations.
22. Architecture compliance and verification approach.

Not every initiative needs a large document. The artefacts should be
scaled to risk, complexity, novelty and change impact.

<a id="26-architecture-decision-records-adrs"></a>

### 26. Architecture Decision Records (ADRs)

An ADR captures a significant decision and why it was made.

Recommended structure:

``` text
# ADR-XXXX: <Decision title>

Status: Proposed | Accepted | Rejected | Superseded
Date:
Decision owners:

## Context
What problem, drivers, constraints and requirements led to this decision?

## Decision
What are we choosing?

## Options considered
What credible alternatives were assessed?

## Rationale
Why does the selected option best meet the requirements?

## Consequences
Benefits, limitations, risks, operational impacts and costs.

## Quality attributes
Which NFRs are affected and how?

## Related decisions
Links to dependent or superseding ADRs.
```

Record consequential decisions close to the time they are made. Do not
use ADRs to document every minor coding choice.

<a id="27-solution-design-application-architecture-and-system-design"></a>

### 27. Solution design, application architecture and system design

These terms overlap in practice, but can be separated by their primary
question.

| Discipline / artefact | Primary question | Typical content |
| --- | --- | --- |
| Solution architecture | What end-to-end solution meets the business need? | Scope, options, systems, integrations, data, security, NFRs, transition |
| Application architecture | How are application responsibilities and components structured? | Application boundaries, modules, services, dependencies, APIs, patterns |
| System design | How will the system behave and be implemented at detailed technical level? | Components, sequences, data structures, algorithms, concurrency, failure handling, deployment details |

The appropriate level of detail depends on the project. A solution
design should not duplicate every low-level implementation detail, and a
system design should not leave critical business or cross-system
decisions unresolved.

<a id="28-architecture-review-checklist"></a>

### 28. Architecture review checklist

<a id="business-and-scope"></a>

#### Business and scope

-   Is the business problem and desired outcome explicit?
-   Are stakeholders and affected capabilities identified?
-   Are scope, assumptions, constraints and dependencies clear?
-   Are business processes and exception paths understood?

<a id="requirements-and-quality"></a>

#### Requirements and quality

-   Are functional requirements traceable?
-   Are NFRs measurable and prioritised?
-   Are volumes, concurrency, growth and latency understood?
-   Are RTO, RPO, availability and service hours defined?

<a id="application-and-services"></a>

#### Application and services

-   Are responsibilities and boundaries clear?
-   Are boundaries aligned with business capabilities or bounded
    contexts?
-   Is coupling justified and visible?
-   Are synchronous and asynchronous interactions chosen deliberately?
-   Are contracts stable and versioned?
-   Are failure modes and idempotency addressed?

<a id="data"></a>

#### Data

-   Are data owners and authoritative sources identified?
-   Are conceptual, logical and physical models appropriate?
-   Is data duplication justified?
-   Are consistency, freshness, quality and lineage defined?
-   Are classification, access, retention and deletion addressed?

<a id="security-and-privacy"></a>

#### Security and privacy

-   Are identities and trust boundaries explicit?
-   Is least privilege enforced?
-   Are sensitive data flows identified?
-   Are encryption, key management and audit controls addressed?
-   Has threat modelling been completed where warranted?

<a id="resilience-and-operations"></a>

#### Resilience and operations

-   Are critical dependencies identified?
-   Are timeout, retry, circuit breaker and bulkhead decisions
    justified?
-   Are observability and alerting sufficient?
-   Are backup, restore and DR tested?
-   Are support ownership and runbooks defined?

<a id="delivery-and-economics"></a>

#### Delivery and economics

-   Is the deployment model clear?
-   Are migrations and rollback/roll-forward strategies safe?
-   Are cost drivers understood?
-   Are platform standards reused where appropriate?
-   Are operational skills and support costs understood?
-   Are exit and decommissioning plans addressed?

---

<a id="part-ix-anti-pattern-catalogue"></a>

## 🚧 Part IX · Anti-pattern catalogue

`PHASE 04` · `PRACTICE & IMPROVEMENT` · **Chapters 29–32**

Use these warning signs to challenge an existing design or a proposed change. Look for the underlying forces and consequences rather than judging by labels alone.

> **💡 Key insight**
>
> A familiar pattern can still be the wrong choice for the business and operating context.


<a id="29-enterprise-and-business-anti-patterns"></a>

### 29. Enterprise and business anti-patterns

-   **Technology-led solution looking for a problem:** choosing a
    platform before defining the business outcome.
-   **Architecture by committee:** decisions made by consensus without
    clear accountability.
-   **Big design up front:** attempting to predict every detail before
    evidence exists.
-   **Ivory tower architecture:** architecture disconnected from
    delivery and operations.
-   **Architecture theatre:** diagrams and governance with no influence
    on outcomes.
-   **Capability duplication:** multiple teams build overlapping
    capabilities without a reason.
-   **Premature standardisation:** forcing a single solution where
    domain needs differ.
-   **Unmanaged exceptions:** local deviations accumulate without
    visibility.

<a id="30-application-and-distributed-system-anti-patterns"></a>

### 30. Application and distributed-system anti-patterns

-   **Big ball of mud:** no meaningful modular boundaries.
-   **Distributed monolith:** services are separate deployments but
    require coordinated changes and synchronous availability.
-   **Nano-services:** excessive fragmentation with little business or
    operational value.
-   **Shared database coupling:** independent services directly modify
    each other's tables.
-   **Chatty service:** excessive fine-grained network calls.
-   **Synchronous call chain:** long dependency chains amplify latency
    and failures.
-   **God service / God object:** one component owns too many
    responsibilities.
-   **Anemic domain model:** domain behaviour is scattered through
    procedural services when complex invariants need a domain model.
-   **Over-engineered domain model:** rich abstractions for simple CRUD
    requirements.
-   **Generic repository for everything:** abstractions obscure
    important query and persistence behaviour.
-   **Retry storm:** uncontrolled retries increase an outage.
-   **Poison message loop:** an unprocessable message is retried
    indefinitely.
-   **Event explosion:** events are published without clear business
    meaning or consumers.
-   **Distributed transaction by assumption:** assuming multiple
    database writes are atomic.
-   **Exactly-once illusion:** relying on broker claims without handling
    end-to-end duplicates and external side effects.

<a id="31-data-anti-patterns"></a>

### 31. Data anti-patterns

-   **Data swamp:** data lake without ownership, quality, metadata or
    discoverability.
-   **Shadow data platform:** uncontrolled copies and pipelines outside
    governance.
-   **One giant canonical model:** central schema becomes a bottleneck.
-   **Enterprise control-table coupling:** every data product depends on
    one shared control mechanism without clear need.
-   **Unowned data product:** no domain accountability or consumer
    support.
-   **Dashboard as data product:** presentation is mistaken for a
    governed data interface.
-   **ETL spaghetti:** pipelines with hidden dependencies and no
    lineage.
-   **Source-system reporting overload:** analytical queries damage
    operational workloads.
-   **Over-normalised analytics:** models are difficult for consumers to
    use.
-   **Over-denormalised operations:** update anomalies and inconsistent
    facts.
-   **Unbounded historical retention:** cost and privacy risk
    accumulate.
-   **Copy without reconciliation:** replicas drift without detection.
-   **Schema drift by accident:** upstream changes silently break
    consumers.

<a id="32-security-and-infrastructure-anti-patterns"></a>

### 32. Security and infrastructure anti-patterns

-   Security perimeter as the only trust control.
-   Shared privileged accounts.
-   Long-lived unmanaged secrets.
-   Broad service permissions.
-   Unencrypted sensitive data.
-   Logging sensitive payloads or credentials.
-   Publicly exposed management interfaces.
-   Multi-cloud without a business or risk rationale.
-   Kubernetes for workloads that do not need orchestration.
-   Serverless without cost, timeout and observability controls.
-   Active-active without conflict and data consistency design.
-   Backups that have never been restored.
-   Autoscaling without downstream capacity limits.
-   Monitoring without actionable alerts or ownership.

---

<a id="part-x-pattern-selection-and-practical-decision-guides"></a>

## 🧭 Part X · Pattern selection and practical decision guides

`PHASE 04` · `PRACTICE & IMPROVEMENT` · **Chapters 33–36**

Move from a problem to candidate patterns, decision evidence and repeatable checks. Use the selection guide as a starting point, not an automatic prescription.

> **💡 Key insight**
>
> Validate important assumptions before they become expensive dependencies.


<a id="33-pattern-selection-by-problem"></a>

### 33. Pattern selection by problem

| Problem | Candidate patterns | Validate before choosing |
| --- | --- | --- |
| Legacy modernisation | Strangler Fig, Anti-corruption Layer, Branch by Abstraction | Data ownership, cutover and coexistence |
| Complex business rules | DDD, Bounded Context, Aggregate, Specification | Domain complexity and expert availability |
| Independent team delivery | Modular architecture, bounded contexts, microservices | Team autonomy and operational maturity |
| Slow read workload | Cache-Aside, CQRS read model, materialised view, index | Staleness tolerance and invalidation |
| Long-running process | Saga, Process Manager, workflow engine | Compensation, timeout and human intervention |
| Reliable DB-to-event publishing | Transactional Outbox, CDC | Atomicity and event semantics |
| Duplicate message delivery | Idempotent Consumer, Inbox | Stable message identity and retention |
| Downstream overload | Queue-Based Load Leveling, Backpressure, Rate Limiting | Queue growth and latency objectives |
| Unreliable dependency | Timeout, Circuit Breaker, Bulkhead, Fallback | Safe fallback and recovery behaviour |
| API for different channels | BFF, API Composition | Duplication and ownership |
| Analytics at scale | Lakehouse, EDW, Data Mart, Medallion | Governance, workload and data product needs |
| Cross-domain data ownership | Data Mesh principles, Data Products | Domain capability and federated governance |
| Data replication | CDC, event propagation, batch replication | Source semantics, deletes, ordering and reconciliation |
| Strong access isolation | RBAC, ABAC, policy enforcement, tenant isolation | Entitlement model and audit requirements |
| Safe releases | Canary, Blue-Green, Feature Flags | Data compatibility and rollback strategy |
| Regional disaster recovery | Warm standby, Active-Passive, Active-Active | RTO/RPO, data replication and cost |

<a id="34-architecture-decision-sequence"></a>

### 34. Architecture decision sequence

A useful decision sequence is:

1.  Clarify the business outcome and stakeholders.
2.  Identify business capabilities and process boundaries.
3.  Establish functional requirements and measurable NFRs.
4.  Identify data ownership and authoritative sources.
5.  Identify trust boundaries, security and regulatory constraints.
6.  Define application and integration responsibilities.
7.  Compare viable architectural styles and patterns.
8.  Assess failure modes, operational model and recovery.
9.  Assess cost, skills, delivery risk and lifecycle.
10. Record decisions, assumptions, alternatives and residual risks.
11. Validate through prototypes, tests, threat modelling and operational
    exercises.
12. Revisit decisions when evidence or constraints change.

<a id="35-architecture-quality-gates"></a>

### 35. Architecture quality gates

Use risk-based gates rather than identical approval steps for every
change.

| Gate | Evidence |
| --- | --- |
| Concept / initiation | Problem, outcome, scope, options and major constraints |
| Architecture | Target structure, boundaries, contracts, NFRs and major decisions |
| Detailed design | Sequences, data design, failure handling, security controls |
| Build readiness | Test strategy, deployment, observability, ownership |
| Production readiness | Load, security, recovery, support, SLOs and runbooks |
| Post-implementation | Outcome measures, incidents, cost, technical debt and lessons |

<a id="36-architecture-fitness-functions"></a>

### 36. Architecture fitness functions

A fitness function is an automated or repeatable check that evaluates an
architectural characteristic.

Examples:

-   No dependency from domain modules to infrastructure implementation
    packages.
-   No cyclic dependencies between bounded contexts.
-   All APIs publish an OpenAPI contract.
-   All events have schema ownership and compatibility checks.
-   All production services emit correlation identifiers and required
    telemetry.
-   No production workload uses unapproved public ingress.
-   All sensitive data stores enforce approved encryption and access
    controls.
-   All services define an owner, SLO and support route.
-   All deployable components have an SBOM and vulnerability scan.
-   Data products publish freshness and quality measurements.
-   Infrastructure changes are represented as reviewed code.
-   Recovery tests meet the agreed RTO/RPO.

Fitness functions should check meaningful architecture constraints.
Avoid turning every preference into a brittle automated rule.

---

<a id="part-xi-reference-architecture-documentation-templates"></a>

## 📝 Part XI · Reference architecture documentation templates

`PHASE 04` · `PRACTICE & IMPROVEMENT` · **Chapters 37–40**

Use these copyable templates to make outcomes, contracts, ownership and NFRs visible. Complete the fields that matter for the scope and risk of the initiative.

> **💡 Key insight**
>
> A useful architecture pack explains decisions and responsibilities; its value is not its page count.


<a id="37-one-page-architecture-overview"></a>

### 37. One-page architecture overview

``` text
# Architecture Overview

## Business outcome
## Scope and exclusions
## Stakeholders
## Business capabilities affected
## Context and external actors
## Solution components and responsibilities
## Key interactions and contracts
## Data ownership and flows
## Security and privacy
## Quality attributes / NFRs
## Deployment and operational model
## Key decisions and alternatives
## Risks and mitigations
## Transition and delivery approach
## Success measures
```

<a id="38-integration-contract-template"></a>

### 38. Integration contract template

``` text
# Integration Contract

Name:
Producer / owner:
Consumer(s):
Purpose:
Interaction: API | Event | Message | File | CDC
Business semantics:
Schema / contract:
Identity and authorisation:
Data classification:
Delivery and ordering:
Idempotency:
Timeout and retry:
Error and dead-letter handling:
Versioning and compatibility:
SLO / freshness:
Monitoring and alerting:
Replay / recovery:
Retention:
Support owner:
Deprecation process:
```

<a id="39-data-product-template"></a>

### 39. Data product template

``` text
# Data Product

Name and domain:
Business purpose:
Product owner:
Data owner / steward:
Consumers and use cases:
Authoritative source(s):
Data contract:
Business glossary:
Classification:
Access policy:
Quality dimensions and rules:
Freshness SLO:
Availability SLO:
Lineage:
Ingestion and transformation:
Versioning and compatibility:
Operational support:
Cost allocation:
Retention and deletion:
Known limitations:
Deprecation plan:
```

<a id="40-nfr-template"></a>

### 40. NFR template

``` text
# Non-functional requirement

ID:
Attribute:
Business rationale:
Priority:
Stimulus:
Operating environment:
Expected response:
Measure and threshold:
Measurement location:
Test method:
Owner:
Dependencies and assumptions:
```

---

<a id="part-xii-further-reading-and-authoritative-references"></a>

## 📚 Part XII · Further reading and authoritative references

`PHASE 04` · `PRACTICE & IMPROVEMENT` · **References & further reading**

Follow the references for deeper treatment of methods, standards and pattern catalogues. Check relevant editions and organisational obligations when applying them.

> **💡 Key insight**
>
> Reference material informs judgement; it does not make every listed technique mandatory.


The following sources underpin significant portions of this handbook.
They are reference catalogues and standards, not evidence that every
listed pattern is mandatory or appropriate in every enterprise.

1.  **The Open Group --- TOGAF and enterprise architecture resources**\
    https://www.opengroup.org/togaf

2.  **The Open Group --- ArchiMate**\
    https://www.opengroup.org/archimate-forum/archimate-overview

3.  **Microsoft Azure Architecture Center --- Cloud design patterns**\
    https://learn.microsoft.com/azure/architecture/patterns\
    Broad, technology-neutral descriptions with Azure implementation
    examples.

4.  **AWS Prescriptive Guidance --- Cloud design patterns**\
    https://docs.aws.amazon.com/prescriptive-guidance/latest/cloud-design-patterns/\
    Includes Anti-corruption Layer, Circuit Breaker, Event Sourcing,
    Hexagonal Architecture, Publish-subscribe, Retry, Saga, Strangler
    Fig and Transactional Outbox.

5.  **Martin Fowler --- Patterns of Enterprise Application Architecture
    catalogue**\
    https://martinfowler.com/eaaCatalog/\
    Established enterprise application patterns for domain logic,
    persistence, presentation, distribution and concurrency.

6.  **Martin Fowler --- Patterns in Enterprise Software**\
    https://martinfowler.com/articles/enterprisePatterns.html\
    Survey of enterprise application, integration and domain pattern
    catalogues.

7.  **Enterprise Integration Patterns --- Gregor Hohpe and Bobby
    Woolf**\
    https://www.enterpriseintegrationpatterns.com/\
    Foundational catalogue for messaging channels, message construction,
    routing, transformation and endpoints.

8.  **DAMA-DMBOK --- Data Management Body of Knowledge**\
    https://www.damadmbok.org/dmbok-framework\
    Structured reference for data governance, architecture, modelling,
    integration, metadata, quality and other data management
    disciplines.

9.  **NIST SP 800-207 --- Zero Trust Architecture**\
    https://csrc.nist.gov/pubs/sp/800/207/final\
    Foundational description of Zero Trust Architecture.

10. **NIST SP 1800-35 --- Implementing a Zero Trust Architecture**\
    https://pages.nist.gov/zero-trust-architecture/\
    Practical implementation guidance and example architectures.

11. **Domain-Driven Design**\
    Eric Evans, *Domain-Driven Design: Tackling Complexity in the Heart
    of Software* (2003).

12. **Implementing Domain-Driven Design**\
    Vaughn Vernon (2013).

13. **Design Patterns: Elements of Reusable Object-Oriented Software**\
    Erich Gamma, Richard Helm, Ralph Johnson and John Vlissides (1994).

14. **Release It!**\
    Michael T. Nygard. Resilience and stability patterns for production
    systems.

15. **Building Microservices**\
    Sam Newman. Microservice boundaries, integration, deployment and
    operational trade-offs.

16. **Fundamentals of Software Architecture**\
    Mark Richards and Neal Ford. Architectural characteristics, styles,
    decisions and trade-offs.

17. **The Data Warehouse Toolkit**\
    Ralph Kimball and Margy Ross. Dimensional modelling patterns.

18. **Designing Data-Intensive Applications**\
    Martin Kleppmann. Distributed data systems, replication,
    partitioning, transactions and stream processing.

19. **BIAN --- Banking Industry Architecture Network**\
    https://bian.org/\
    Banking reference architecture and service-domain resources.

20. **OWASP**\
    https://owasp.org/\
    Application security guidance and verification resources.

---

<a id="41-final-guidance-how-an-experienced-architect-should-apply-this-catalogue"></a>

## ✦ 41. Final guidance: how an experienced architect should apply this catalogue

A seasoned architect does not try to use the largest number of patterns.
They:

1.  Understand the business problem before selecting technology.
2.  Identify the smallest set of architectural decisions that materially
    affect outcomes.
3.  Select patterns based on explicit forces and quality attributes.
4.  Understand the operational and organisational cost of each pattern.
5.  Keep domain ownership and data accountability clear.
6.  Prefer simple, reversible decisions until evidence justifies
    complexity.
7.  Make failure, security, privacy and recovery part of the initial
    design.
8.  Record alternatives, assumptions and consequences.
9.  Validate architecture through implementation, measurement and
    operational exercises.
10. Evolve architecture as the business and evidence change.

**The measure of good architecture is not how many patterns it uses. It
is how effectively it enables business outcomes while managing
complexity, risk, cost and change.**

---

> **🎯 Put it into practice**
>
> Apply the assessment template to one real architecture decision. State the
> problem, compare credible options, record the trade-offs and define how you will
> validate the result.

**[↑ Explore the guide](#explore-the-guide)** · **[Pattern assessment](#1-2-pattern-assessment-template)** · **[Review checklist](#28-architecture-review-checklist)**
