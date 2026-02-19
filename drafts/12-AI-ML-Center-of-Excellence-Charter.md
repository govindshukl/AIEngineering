# AI/ML Center of Excellence Charter

## Bank ABC - Innovation & Digitization Department

**Document ID:** AI-GOV-012
**Version:** 1.0
**Classification:** Internal
**Last Updated:** January 2025
**Document Owner:** Head of AI Engineering
**Review Cycle:** Annual

---

## Table of Contents

1. [Executive Summary](#1-executive-summary)
2. [Purpose & Mission](#2-purpose--mission)
3. [Scope & Ownership](#3-scope--ownership)
4. [Organizational Structure](#4-organizational-structure)
5. [Roles & Responsibilities](#5-roles--responsibilities)
6. [Governance & Decision Authority](#6-governance--decision-authority)
7. [Operating Model](#7-operating-model)
8. [Services Catalog](#8-services-catalog)
9. [Federated Champion Network](#9-federated-champion-network)
10. [Success Metrics & KPIs](#10-success-metrics--kpis)
11. [Framework Integration](#11-framework-integration)
12. [Resource & Budget Model](#12-resource--budget-model)
13. [Evolution Roadmap](#13-evolution-roadmap)
14. [Appendices](#14-appendices)

---

## 1. Executive Summary

### 1.1 Charter Statement

This Charter establishes the **AI/ML Center of Excellence (CoE)** as the central governing body for all Artificial Intelligence, Machine Learning, and Intelligent Automation initiatives at Bank ABC. The CoE operates under the Innovation & Digitization Department with a mandate to accelerate responsible AI adoption while ensuring regulatory compliance and risk management.

### 1.2 Strategic Mandate

The AI/ML CoE is empowered to:

- **Set Standards**: Define and enforce AI/ML development, deployment, and operational standards
- **Enable Innovation**: Provide platforms, tools, and reusable assets to accelerate AI adoption
- **Manage Risk**: Oversee model risk management and regulatory compliance
- **Build Capability**: Develop AI literacy and technical skills across the organization
- **Drive Value**: Ensure AI initiatives deliver measurable business outcomes

### 1.3 Operating Principles

| Principle | Description |
|-----------|-------------|
| **Lean Core, Federated Reach** | Small central team with embedded champions across business units |
| **Enabler, Not Bottleneck** | Streamlined processes with tiered approval based on risk |
| **Responsible AI** | Ethics, fairness, and transparency embedded in all activities |
| **Business-First** | Technology decisions driven by business value, not novelty |
| **Continuous Learning** | Adaptive approach with regular retrospectives and improvements |

---

## 2. Purpose & Mission

### 2.1 Mission Statement

> To enable Bank ABC to become an AI-driven organization by establishing world-class governance, providing scalable infrastructure, and building organization-wide AI capability—while ensuring full regulatory compliance and responsible AI practices.

### 2.2 Vision

By 2027, Bank ABC will:
- Have AI embedded in 50% of core business processes
- Achieve top-quartile efficiency through intelligent automation
- Maintain zero critical regulatory findings related to AI/ML
- Be recognized as an AI leader in the Bahrain banking sector

### 2.3 Strategic Objectives

| Objective | Target | Timeline |
|-----------|--------|----------|
| Establish foundational governance framework | 11 core documents approved | Q1 2025 |
| Launch AI/Automation Hub | Platform operational | Q2 2025 |
| Certify 100% of AI practitioners | Internal certification program | Q4 2025 |
| Achieve 30+ production AI use cases | Active model inventory | Q4 2026 |
| Reduce model deployment time by 50% | MLOps maturity Level 3 | Q4 2026 |

---

## 3. Scope & Ownership

### 3.1 In-Scope Activities

The CoE has ownership and accountability for:

#### 3.1.1 AI Governance & Policy
- AI/ML Governance Framework (11 core documents)
- AI Ethics and Responsible AI Policy
- Model Risk Management Standards
- Regulatory compliance (CBB, Basel, SR 11-7, PRA SS1/23)
- AI/ML Steering Committee coordination

#### 3.1.2 Model Risk Management
- Model Inventory Register maintenance
- Model validation standards and oversight
- Risk tier classification (Tier 1/2/3)
- Ongoing monitoring framework
- Model retirement governance

#### 3.1.3 Reusable AI Assets & Infrastructure
- AI/Automation Hub platform
- MLOps infrastructure (CI/CD, model registry, monitoring)
- Feature stores and curated datasets
- Pre-approved model templates
- Approved vendor integrations

#### 3.1.4 Copilot & GenAI Governance
- O365 Copilot provisioning and policies
- Generative AI usage guidelines
- Prompt engineering standards
- GenAI risk controls and monitoring

#### 3.1.5 Specialized AI Domains
- Fraud detection and financial crime AI
- Agentic AI initiatives
- Customer-facing AI solutions
- High-risk model oversight

#### 3.1.6 AI Capability Building
- AI literacy programs (all levels)
- Technical training curriculum
- AI Champion network enablement
- Internal certification program
- Community of Practice facilitation

### 3.2 Out-of-Scope Activities

The CoE does **not** own:

| Activity | Owner | CoE Role |
|----------|-------|----------|
| Business case development | Business Sponsor | Consulted |
| Production infrastructure operations | IT Operations | Consulted |
| Cybersecurity controls | Information Security | Consulted |
| Data quality management | Data Governance | Consulted |
| Vendor contract negotiation | Procurement | Consulted |
| Audit execution | Internal Audit | Informed |

### 3.3 Shared Ownership Model

| Activity | CoE | Partner | Collaboration Model |
|----------|-----|---------|---------------------|
| Model development | Standards, templates | BU Data Scientists | CoE reviews, BU builds |
| Data pipeline creation | Architecture standards | Data Engineering | Joint design reviews |
| Security testing | AI-specific testing | InfoSec | Combined test protocols |
| Change management | AI training content | L&D | Joint program delivery |
| Vendor selection | Technical evaluation | Procurement | Combined RFP process |

---

## 4. Organizational Structure

### 4.1 Reporting Line

```
┌─────────────────────────────────────────────────────────────┐
│                    Chief Digital Officer                     │
│               (Innovation & Digitization)                    │
└──────────────────────────┬──────────────────────────────────┘
                           │
┌──────────────────────────▼──────────────────────────────────┐
│                   AI/ML Steering Committee                   │
│     (Strategic oversight, Tier 1 approvals, escalations)    │
└──────────────────────────┬──────────────────────────────────┘
                           │
┌──────────────────────────▼──────────────────────────────────┐
│               AI/ML Center of Excellence                     │
│                    (Core Team: 5 FTEs)                       │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌────────┐ │
│  │   CoE   │ │   AI    │ │  Model  │ │   AI    │ │   AI   │ │
│  │  Lead   │ │Architect│ │  Risk   │ │ Product │ │Trainer │ │
│  │         │ │         │ │Specialist│ │ Manager │ │        │ │
│  └─────────┘ └─────────┘ └─────────┘ └─────────┘ └────────┘ │
└──────────────────────────┬──────────────────────────────────┘
                           │
        ┌──────────┬───────┴───────┬──────────┬──────────┐
        │          │               │          │          │
┌───────▼───┐ ┌────▼────┐ ┌────────▼───┐ ┌────▼────┐ ┌───▼────┐
│  Retail   │ │Corporate│ │  Treasury  │ │   Ops   │ │  Risk  │
│  Banking  │ │ Banking │ │            │ │         │ │& Comply│
│  Champion │ │ Champion│ │  Champion  │ │ Champion│ │Champion│
└───────────┘ └─────────┘ └────────────┘ └─────────┘ └────────┘
```

### 4.2 Core Team Composition

| Role | FTE | Grade | Primary Focus |
|------|-----|-------|---------------|
| CoE Lead | 1.0 | AVP/VP | Strategy, governance, stakeholder management |
| AI Architect | 1.0 | Senior | Technical standards, MLOps, platform architecture |
| Model Risk Specialist | 1.0 | Senior | Validation oversight, inventory, compliance |
| AI Product Manager | 1.0 | Mid-Senior | Hub management, use case intake, prioritization |
| AI Trainer/Enabler | 0.5-1.0 | Mid | Literacy programs, champion network, community |

**Total Core Team:** 4.5-5.0 FTEs

### 4.3 Extended Team (Virtual/Matrix)

| Role | Source | Allocation | Engagement Model |
|------|--------|------------|------------------|
| Data Scientists | BU Teams | As needed | Project-based assignment |
| ML Engineers | IT/Digital | 2 FTEs dedicated | Permanent allocation |
| Data Engineers | Data Team | 1 FTE dedicated | Permanent allocation |
| Solution Architects | Enterprise Arch | As needed | Design reviews |
| QA Engineers | IT QA | As needed | Testing phases |

---

## 5. Roles & Responsibilities

### 5.1 CoE Lead (Head of AI Engineering)

**Accountability:** Overall success of AI/ML initiatives and CoE operations

| Responsibility | Deliverables |
|----------------|--------------|
| Strategic leadership | AI/ML strategy and roadmap |
| Governance ownership | Framework maintenance and evolution |
| Stakeholder management | Executive reporting, steering committee |
| Regulatory liaison | CBB engagement, audit coordination |
| Team leadership | CoE team development and performance |
| Budget management | CoE budget and investment cases |

**Decision Authority:**
- Tier 2 initiative final approval
- CoE resource allocation
- Vendor/technology recommendations
- Policy exception escalation

### 5.2 AI Architect

**Accountability:** Technical excellence and platform reliability

| Responsibility | Deliverables |
|----------------|--------------|
| Architecture standards | Reference architectures, design patterns |
| MLOps platform | CI/CD pipelines, model registry, monitoring |
| Technology roadmap | Platform evolution, tool selection |
| Technical review | Solution architecture reviews (all tiers) |
| Integration standards | API standards, data contracts |
| Security architecture | AI-specific security patterns |

**Decision Authority:**
- Technology stack decisions
- Architecture pattern approval
- Technical debt prioritization
- Platform feature roadmap

### 5.3 Model Risk Specialist

**Accountability:** Model risk management and regulatory compliance

| Responsibility | Deliverables |
|----------------|--------------|
| Model inventory | Accurate, complete model register |
| Validation oversight | Validation standards, validator qualification |
| Risk classification | Tier assignment and review |
| Monitoring framework | Performance thresholds, drift detection |
| Regulatory compliance | CBB/Basel alignment, audit readiness |
| Retirement governance | Decommissioning approvals |

**Decision Authority:**
- Risk tier classification
- Validation pass/fail recommendations
- Monitoring threshold alerts
- Model retirement recommendations

### 5.4 AI Product Manager

**Accountability:** Use case pipeline and Hub platform value delivery

| Responsibility | Deliverables |
|----------------|--------------|
| Use case intake | Intake queue management, triage |
| Prioritization | Business case review, stack ranking |
| Hub management | Platform roadmap, feature releases |
| Asset curation | Template library, component catalog |
| Adoption metrics | Usage tracking, value realization |
| Stakeholder comms | Progress reporting, showcases |

**Decision Authority:**
- Use case prioritization recommendations
- Hub feature prioritization
- Asset library curation
- Communication content

### 5.5 AI Trainer/Enabler

**Accountability:** Organization-wide AI capability building

| Responsibility | Deliverables |
|----------------|--------------|
| Training curriculum | Learning paths (Levels 1-4) |
| Certification program | Assessment design, certification tracking |
| Champion enablement | Champion training, ongoing support |
| Community management | CoP facilitation, knowledge sharing |
| Content development | Training materials, guides, playbooks |
| Adoption support | Change management, onboarding |

**Decision Authority:**
- Curriculum content
- Certification criteria
- Community event agenda
- Training delivery methods

---

## 6. Governance & Decision Authority

### 6.1 Decision Rights Matrix

| Decision Type | Tier 3 | Tier 2 | Tier 1 |
|---------------|--------|--------|--------|
| Initiative approval | CoE Lead | CoE Lead | Steering Committee |
| Architecture approval | AI Architect | AI Architect + Review | Steering Committee |
| Production deployment | CoE Lead | CoE Lead + Risk | Steering Committee |
| Exception requests | CoE Lead | Steering Committee | Steering Committee |
| Model retirement | Model Risk Spec | CoE Lead | Steering Committee |
| Budget allocation (< $50K) | CoE Lead | CoE Lead | - |
| Budget allocation (> $50K) | - | Steering Committee | Steering Committee |

### 6.2 Escalation Matrix

| Issue Type | Level 1 | Level 2 | Level 3 |
|------------|---------|---------|---------|
| Technical blockers | AI Architect | CoE Lead | CTO |
| Resource conflicts | CoE Lead | CDO | ExCo |
| Regulatory concerns | Model Risk Spec | CoE Lead + Compliance | Risk Committee |
| Stakeholder disputes | CoE Lead | CDO | ExCo |
| Security incidents | AI Architect | CISO | Risk Committee |

### 6.3 Meeting Cadence

| Forum | Frequency | Chair | Participants | Purpose |
|-------|-----------|-------|--------------|---------|
| CoE Daily Standup | Daily | CoE Lead | Core team | Task coordination |
| CoE Weekly Review | Weekly | CoE Lead | Core + Extended team | Progress, blockers |
| Champion Sync | Bi-weekly | AI Trainer | All Champions | Updates, feedback |
| Technical Review Board | Bi-weekly | AI Architect | Architects, Leads | Design approvals |
| Steering Committee | Monthly | CDO | Executives, CoE Lead | Strategic decisions |
| Community of Practice | Monthly | AI Trainer | All AI practitioners | Knowledge sharing |
| Quarterly Business Review | Quarterly | CoE Lead | CDO, BU Heads | Value delivery |

---

## 7. Operating Model

### 7.1 Service Delivery Model

```
┌─────────────────────────────────────────────────────────────────┐
│                      DEMAND CHANNELS                             │
├─────────────┬─────────────┬─────────────┬───────────────────────┤
│   Direct    │   Champion  │   Hub Self- │    Strategic          │
│   Request   │   Intake    │   Service   │    Initiatives        │
└──────┬──────┴──────┬──────┴──────┬──────┴──────────┬────────────┘
       │             │             │                  │
       └─────────────┴─────────────┴──────────────────┘
                            │
                   ┌────────▼────────┐
                   │   INTAKE &      │
                   │   TRIAGE        │
                   │  (AI Product    │
                   │   Manager)      │
                   └────────┬────────┘
                            │
         ┌──────────────────┼──────────────────┐
         │                  │                  │
    ┌────▼────┐       ┌─────▼─────┐      ┌─────▼─────┐
    │ Tier 3  │       │  Tier 2   │      │  Tier 1   │
    │ Fast    │       │  Standard │      │ Strategic │
    │ Track   │       │  Track    │      │  Track    │
    └────┬────┘       └─────┬─────┘      └─────┬─────┘
         │                  │                  │
         │            ┌─────▼─────┐      ┌─────▼─────┐
         │            │ CoE Lead  │      │ Steering  │
         │            │ Approval  │      │ Committee │
         │            └─────┬─────┘      └─────┬─────┘
         │                  │                  │
         └──────────────────┼──────────────────┘
                            │
                   ┌────────▼────────┐
                   │   DELIVERY      │
                   │   (Stage-Gate)  │
                   └────────┬────────┘
                            │
                   ┌────────▼────────┐
                   │   OPERATIONS    │
                   │   & MONITORING  │
                   └─────────────────┘
```

### 7.2 Engagement Models

#### Direct Engagement (CoE-Led)
- **When:** Tier 1 strategic initiatives, cross-BU programs
- **Model:** CoE team leads delivery with BU resources
- **Timeline:** 3-12 months
- **Examples:** Enterprise fraud platform, Agentic AI pilot

#### Embedded Support (CoE-Assisted)
- **When:** Tier 2 initiatives, complex requirements
- **Model:** BU leads with CoE architect/specialist embedded
- **Timeline:** 1-6 months
- **Examples:** Credit scoring model refresh, chatbot implementation

#### Self-Service (CoE-Enabled)
- **When:** Tier 3 initiatives, standard patterns
- **Model:** BU uses CoE templates, tools; Champion provides support
- **Timeline:** 1-8 weeks
- **Examples:** Dashboard analytics, simple automation

#### Advisory Only
- **When:** Exploration, feasibility, vendor evaluation
- **Model:** CoE provides guidance, BU executes
- **Timeline:** As needed
- **Examples:** Technology POCs, vendor demos

### 7.3 SLA Commitments

| Service | SLA | Measurement |
|---------|-----|-------------|
| Use case intake response | 2 business days | Time to initial triage |
| Tier classification | 5 business days | Time to risk assessment |
| Architecture review (Tier 3) | 5 business days | Time to approval/feedback |
| Architecture review (Tier 2) | 10 business days | Time to approval/feedback |
| Champion support response | 1 business day | Time to acknowledge |
| Production incident response | 4 hours (P1), 1 day (P2) | Time to engage |
| Training request fulfillment | 10 business days | Time to schedule |

---

## 8. Services Catalog

### 8.1 Governance Services

| Service | Description | Requestor | Delivery |
|---------|-------------|-----------|----------|
| Use Case Intake | Submission and triage of AI initiatives | Any BU | AI Product Manager |
| Risk Classification | Tier 1/2/3 assessment | Intake process | Model Risk Specialist |
| Gate Reviews | Stage-gate approval coordination | Project teams | CoE Lead |
| Policy Guidance | AI policy interpretation | Any stakeholder | CoE Lead |
| Exception Processing | Policy exception requests | Project teams | CoE Lead |
| Audit Support | Regulatory and internal audit coordination | Audit teams | Model Risk Specialist |

### 8.2 Technical Services

| Service | Description | Requestor | Delivery |
|---------|-------------|-----------|----------|
| Architecture Review | Solution design validation | Project teams | AI Architect |
| MLOps Onboarding | Pipeline and registry setup | Development teams | AI Architect |
| Model Registry | Model versioning and metadata | Development teams | AI Architect |
| Template Provisioning | Pre-approved model templates | Development teams | AI Architect |
| Feature Store Access | Curated feature provisioning | Data Scientists | AI Architect |
| Monitoring Setup | Model monitoring configuration | Operations | AI Architect |

### 8.3 Risk Management Services

| Service | Description | Requestor | Delivery |
|---------|-------------|-----------|----------|
| Model Inventory Registration | Adding models to registry | Development teams | Model Risk Specialist |
| Validation Coordination | Independent validation scheduling | Project teams | Model Risk Specialist |
| Performance Monitoring | Drift and degradation alerts | Model owners | Model Risk Specialist |
| Revalidation Scheduling | Periodic revalidation planning | Model Risk Specialist | Model Risk Specialist |
| Retirement Processing | Model decommissioning | Model owners | Model Risk Specialist |

### 8.4 Enablement Services

| Service | Description | Requestor | Delivery |
|---------|-------------|-----------|----------|
| AI Awareness Training | Level 1 training for all staff | HR/L&D | AI Trainer |
| Practitioner Training | Levels 2-4 technical training | Individuals, Managers | AI Trainer |
| Certification Assessment | Internal AI certification | Individuals | AI Trainer |
| Champion Onboarding | New champion orientation | BU Heads | AI Trainer |
| Custom Workshops | Tailored team sessions | BU Champions | AI Trainer |
| CoP Facilitation | Monthly knowledge sharing | Community | AI Trainer |

### 8.5 Platform Services

| Service | Description | Requestor | Delivery |
|---------|-------------|-----------|----------|
| Hub Access | Platform onboarding | Champions, Teams | AI Product Manager |
| Copilot Provisioning | O365 Copilot license requests | Managers | AI Product Manager |
| Asset Publishing | Adding solutions to Hub catalog | Development teams | AI Product Manager |
| Usage Analytics | Adoption and usage reports | BU Heads | AI Product Manager |

---

## 9. Federated Champion Network

### 9.1 Champion Model Overview

The Champion Network extends CoE reach into business units while maintaining lean central operations.

```
┌─────────────────────────────────────────────────────────────────┐
│                        Core CoE                                  │
│            (Standards, Platform, Risk, Training)                 │
└───────────────────────────┬─────────────────────────────────────┘
                            │
                            │ Dotted-line reporting
                            │ Monthly sync
                            │ Shared metrics
                            │
    ┌───────────┬───────────┼───────────┬───────────┬────────────┐
    │           │           │           │           │            │
┌───▼───┐   ┌───▼───┐   ┌───▼───┐   ┌───▼───┐   ┌───▼───┐   ┌───▼───┐
│Retail │   │Corp   │   │Treasury│  │ Ops   │   │ Risk  │   │Digital│
│Banking│   │Banking│   │        │  │       │   │&Comply│   │Channel│
│Champion│  │Champion│  │Champion│  │Champion│  │Champion│  │Champion│
└───┬───┘   └───┬───┘   └───┬───┘   └───┬───┘   └───┬───┘   └───┬───┘
    │           │           │           │           │            │
    ▼           ▼           ▼           ▼           ▼            ▼
┌───────┐   ┌───────┐   ┌───────┐   ┌───────┐   ┌───────┐   ┌───────┐
│ BU AI │   │ BU AI │   │ BU AI │   │ BU AI │   │ BU AI │   │ BU AI │
│ Teams │   │ Teams │   │ Teams │   │ Teams │   │ Teams │   │ Teams │
└───────┘   └───────┘   └───────┘   └───────┘   └───────┘   └───────┘
```

### 9.2 Champion Selection Criteria

| Criterion | Requirement |
|-----------|-------------|
| Role Level | Senior Analyst / Manager or above |
| Domain Knowledge | Deep understanding of BU processes |
| Technical Aptitude | Level 2+ AI literacy (or commitment to achieve) |
| Influence | Respect and credibility within BU |
| Time Commitment | Minimum 20% allocation to Champion role |
| Tenure | 12+ months in current BU |

### 9.3 Champion Responsibilities

| Category | Responsibilities |
|----------|------------------|
| **Demand Management** | Collect and prioritize AI use cases from BU |
| | Submit use cases through intake process |
| | Maintain local BU AI pipeline |
| **Standards Adoption** | Ensure BU compliance with CoE standards |
| | Conduct local design reviews (Tier 3) |
| | Escalate non-compliance issues |
| **Knowledge Transfer** | Cascade CoE training to BU teams |
| | Facilitate local AI awareness sessions |
| | Share CoP learnings with BU |
| **Support & Enablement** | First-line support for Copilot users |
| | Guide teams on Hub usage |
| | Answer policy questions (or escalate) |
| **Feedback & Improvement** | Report challenges to CoE |
| | Propose standard improvements |
| | Participate in retrospectives |

### 9.4 Champion Authority

| Authority | Tier 3 | Tier 2 | Tier 1 |
|-----------|--------|--------|--------|
| Use case screening | Approve | Recommend | Recommend |
| Local design review | Approve | Participate | - |
| Copilot access request | Approve | Approve | Approve |
| Training scheduling | Approve | Approve | Approve |
| Exception request | Escalate | Escalate | Escalate |

### 9.5 Champion Enablement

| Support | Description | Frequency |
|---------|-------------|-----------|
| Onboarding Program | 2-day intensive orientation | On appointment |
| Champion Playbook | Procedures, templates, FAQs | Continuous access |
| Bi-weekly Sync | Updates, Q&A, peer learning | Every 2 weeks |
| Quarterly Workshop | Deep-dive training, strategy alignment | Quarterly |
| Slack/Teams Channel | Real-time peer support | Always available |
| CoE Office Hours | Direct access to CoE specialists | Weekly |

### 9.6 Champion Performance Metrics

| Metric | Target | Measurement |
|--------|--------|-------------|
| Use cases submitted | 2+ per quarter | Intake system |
| Training cascade completion | 80% BU coverage | LMS tracking |
| Support ticket resolution | < 2 days average | Ticketing system |
| BU satisfaction score | > 4.0 / 5.0 | Quarterly survey |
| CoE event participation | 80% attendance | Event tracking |

---

## 10. Success Metrics & KPIs

### 10.1 Strategic KPIs

| KPI | Baseline | Year 1 Target | Year 2 Target | Measurement |
|-----|----------|---------------|---------------|-------------|
| Active AI use cases in production | 5 | 15 | 30 | Model inventory |
| AI-influenced revenue (%) | 0% | 5% | 15% | Finance attribution |
| Process automation coverage | 10% | 25% | 40% | Process mapping |
| Regulatory findings (AI-related) | - | 0 critical | 0 critical | Audit reports |
| AI practitioner certification | 0 | 50 | 100 | Certification records |

### 10.2 Operational KPIs

| KPI | Target | Frequency | Owner |
|-----|--------|-----------|-------|
| Intake-to-production cycle time (Tier 3) | < 8 weeks | Monthly | AI Product Manager |
| Intake-to-production cycle time (Tier 2) | < 16 weeks | Monthly | AI Product Manager |
| Model validation pass rate (first attempt) | > 80% | Quarterly | Model Risk Specialist |
| MLOps pipeline availability | > 99.5% | Monthly | AI Architect |
| Model drift alerts addressed | < 48 hours | Monthly | Model Risk Specialist |
| Training satisfaction score | > 4.2 / 5.0 | Per session | AI Trainer |

### 10.3 Adoption KPIs

| KPI | Target | Frequency | Owner |
|-----|--------|-----------|-------|
| Hub monthly active users | 200+ | Monthly | AI Product Manager |
| Copilot adoption rate | 70% of licenses | Monthly | AI Product Manager |
| Reusable asset utilization | 60% of new projects | Quarterly | AI Architect |
| CoP session attendance | 40+ participants | Monthly | AI Trainer |
| Champion network NPS | > 50 | Quarterly | AI Trainer |

### 10.4 Efficiency KPIs

| KPI | Target | Frequency | Owner |
|-----|--------|-----------|-------|
| Time saved through automation | 10,000+ hours/year | Quarterly | AI Product Manager |
| Cost per deployed model | Decreasing trend | Quarterly | CoE Lead |
| Model reuse rate | > 30% | Quarterly | AI Architect |
| Self-service resolution rate | > 60% | Monthly | AI Trainer |

---

## 11. Framework Integration

### 11.1 Alignment with Governance Documents

| Document | CoE Role | Integration Point |
|----------|----------|-------------------|
| 01 - Operating Model | Owner | CoE is the operational arm |
| 02 - Use Case Intake | Owner | AI Product Manager manages intake |
| 03 - Stage-Gate Process | Facilitator | CoE chairs gate reviews |
| 04 - Model Inventory | Owner | Model Risk Specialist maintains |
| 05 - Compliance Matrix | Contributor | CoE ensures alignment |
| 06 - Development Standards | Owner | AI Architect defines standards |
| 07 - Automation Standards | Owner | AI Architect defines standards |
| 08 - Technology Selection | Contributor | AI Architect evaluates technology |
| 09 - Model Validation | Owner | Model Risk Specialist oversees |
| 10 - Monitoring Standards | Owner | AI Architect/Model Risk Specialist |
| 11 - Security Standards | Contributor | AI Architect collaborates with InfoSec |
| RACI Matrix | Subject | CoE roles throughout |

### 11.2 RACI Alignment

CoE roles map to the RACI Matrix as follows:

| CoE Role | RACI Abbreviation |
|----------|-------------------|
| CoE Lead | AILead |
| AI Architect | SolArch (AI-specific) |
| Model Risk Specialist | ModelVal |
| AI Product Manager | DigProdHead / BA |
| AI Trainer | New role (to be added) |
| Champions | New role (to be added) |

### 11.3 Steering Committee Interface

| Activity | CoE Role | Steering Committee Role |
|----------|----------|------------------------|
| Tier 1 initiative approval | Present recommendation | Approve/reject |
| Quarterly progress review | Present metrics | Review and guide |
| Policy changes | Draft and propose | Approve |
| Budget requests | Prepare business case | Approve |
| Escalations | Present issue | Decide resolution |
| Annual strategy | Draft roadmap | Approve direction |

---

## 12. Resource & Budget Model

### 12.1 Core Team Investment

| Role | Annual Cost (Approx.) | Funding Source |
|------|----------------------|----------------|
| CoE Lead | $XXX,XXX | Digital/Innovation budget |
| AI Architect | $XXX,XXX | Digital/Innovation budget |
| Model Risk Specialist | $XXX,XXX | Risk/Digital shared |
| AI Product Manager | $XXX,XXX | Digital/Innovation budget |
| AI Trainer (0.5-1.0 FTE) | $XX,XXX | L&D/Digital shared |
| **Total Core Team** | $XXX,XXX | - |

### 12.2 Platform & Tools Budget

| Category | Annual Budget | Items |
|----------|---------------|-------|
| MLOps Platform | $XXX,XXX | Azure ML, MLflow, monitoring |
| AI/Automation Hub | $XX,XXX | Platform hosting, licensing |
| Copilot Licenses | $XXX,XXX | O365 Copilot, GitHub Copilot |
| Training Tools | $XX,XXX | LMS, content development |
| External Training | $XX,XXX | Vendor certifications |
| **Total Platform** | $XXX,XXX | - |

### 12.3 Chargeback Model

| Initiative Type | Cost Model | Charged To |
|-----------------|------------|------------|
| Tier 1 (Strategic) | Central funding | Digital budget |
| Tier 2 (Standard) | 50/50 split | Digital + BU budget |
| Tier 3 (Self-service) | BU funded | BU budget |
| Platform/Hub | Central funding | Digital budget |
| Training | Central funding | L&D budget |

### 12.4 Annual Budget Cycle

| Period | Activity |
|--------|----------|
| Q3 | Gather demand forecast from Champions |
| Q3 | Draft annual budget proposal |
| Q4 | Present to Steering Committee |
| Q4 | Finalize budget allocation |
| Q1-Q4 | Monthly budget tracking and reporting |
| Q2 | Mid-year budget review |

---

## 13. Evolution Roadmap

### 13.1 Maturity Model

| Stage | Characteristics | Target State |
|-------|-----------------|--------------|
| **Stage 1: Foundation** | Governance framework, core team, basic platform | Q1 2025 |
| **Stage 2: Enablement** | Hub launched, Champion network active, training programs | Q2-Q3 2025 |
| **Stage 3: Scale** | 20+ production use cases, self-service dominant | Q4 2025 - Q2 2026 |
| **Stage 4: Optimization** | MLOps Level 3, automated governance, AI-driven CoE | Q3-Q4 2026 |
| **Stage 5: Innovation** | Leading edge AI (Agentic, multimodal), industry leadership | 2027+ |

### 13.2 Capability Roadmap

| Quarter | Governance | Platform | Capability |
|---------|------------|----------|------------|
| Q1 2025 | Framework v1.0 approved | MLOps foundation | Core team hired |
| Q2 2025 | Gate process operational | Hub v1.0 launch | Champion network live |
| Q3 2025 | Model inventory populated | Feature store v1.0 | Level 1-2 training deployed |
| Q4 2025 | Automated compliance checks | Hub v2.0 (self-service) | Certification program |
| Q1 2026 | Agentic AI framework | GenAI guardrails | Advanced training (Level 4) |
| Q2 2026 | Continuous validation | AutoML capabilities | AI literacy 100% coverage |

### 13.3 Team Evolution

| Phase | Core Team | Extended Model |
|-------|-----------|----------------|
| Year 1 | 5 FTEs | 6 Champions, 3 dedicated resources |
| Year 2 | 6-7 FTEs | 8 Champions, 5 dedicated resources |
| Year 3 | 7-8 FTEs | 10 Champions, federated specialists |

---

## 14. Appendices

### Appendix A: Glossary

| Term | Definition |
|------|------------|
| **Champion** | BU-embedded AI advocate with dotted-line to CoE |
| **CoE** | Center of Excellence |
| **CoP** | Community of Practice |
| **Gate** | Decision checkpoint in the stage-gate process |
| **Hub** | AI/Automation Hub - self-service platform |
| **MLOps** | Machine Learning Operations |
| **Tier** | Risk classification level (1=High, 2=Medium, 3=Low) |

### Appendix B: Related Documents

| Document | Location |
|----------|----------|
| AI/ML Governance Operating Model | Document 01 |
| Use Case Intake Framework | Document 02 |
| Stage-Gate Process | Document 03 |
| Model Inventory Register | Document 04 |
| RACI Matrix | RACI-Matrix.md |
| INDEX | INDEX.md |

### Appendix C: Charter Approval

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Chief Digital Officer | | | |
| Head of Risk | | | |
| Head of Compliance | | | |
| CoE Lead | | | |

### Appendix D: Revision History

| Version | Date | Description | Author |
|---------|------|-------------|--------|
| 1.0 | January 2025 | Initial charter | AI Engineering Team |

---

*This Charter is effective upon approval by the signatories listed in Appendix C and shall be reviewed annually or upon significant organizational changes.*
