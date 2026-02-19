# RACI Matrix for AI/ML & Automation Initiatives
## Bank ABC - Innovation & Digitization Department

**Document ID:** AI-GOV-RACI
**Version:** 1.1
**Classification:** Internal
**Owner:** Head of AI Engineering, Innovation & Digitization Department
**Last Review Date:** January 2025
**Next Review Date:** January 2026

---

## Table of Contents

1. [Introduction](#1-introduction)
2. [RACI Definitions](#2-raci-definitions)
3. [Role Definitions](#3-role-definitions)
4. [Governance Activities RACI](#4-governance-activities-raci)
5. [Gate 0: Intake & Prioritization RACI](#5-gate-0-intake--prioritization-raci)
6. [Gate 1: Discovery & Feasibility RACI](#6-gate-1-discovery--feasibility-raci)
7. [Gate 2: Design Phase RACI](#7-gate-2-design-phase-raci)
8. [Gate 3: Build Phase RACI](#8-gate-3-build-phase-raci)
9. [Gate 4: Validation & Testing RACI](#9-gate-4-validation--testing-raci)
10. [Gate 5: Deployment RACI](#10-gate-5-deployment-raci)
11. [Post-Implementation Review RACI](#11-post-implementation-review-raci)
12. [Ongoing Operations & Maintenance RACI](#12-ongoing-operations--maintenance-raci)
13. [Retraining & Enhancement RACI](#13-retraining--enhancement-raci)
14. [Model/Bot Retirement RACI](#14-modelbot-retirement-raci)
15. [Copilot Tools Management RACI](#15-copilot-tools-management-raci)
16. [AI & Automation Hub Management RACI](#16-ai--automation-hub-management-raci)
17. [Initiative Type Variations](#17-initiative-type-variations)
18. [Tier-Based Variations](#18-tier-based-variations)
19. [RACI Governance & Maintenance](#19-raci-governance--maintenance)
20. [Appendices](#20-appendices)

---

## 1. Introduction

### 1.1 Purpose

This document defines roles and responsibilities using the RACI framework for all AI/ML and Automation initiatives at Bank ABC. It provides clarity on who is Responsible, Accountable, Consulted, and Informed for each activity across the complete initiative lifecycle.

### 1.2 Scope

This RACI matrix covers:
- **AI/ML Initiatives**: Analytical AI, Generative AI, Agentic AI, Machine Learning models
- **Automation Initiatives**: RPA (Automation Anywhere), Power Automate (Desktop & Cloud), Business Process Automation, Copilot Studio Agents
- **Hybrid Initiatives**: Solutions combining AI and Automation components
- **Complete Lifecycle**: From intake through retirement
- **Ongoing Operations**: Monitoring, maintenance, retraining, and periodic reviews

### 1.3 Application

- Use this matrix as a reference for clarifying responsibilities on initiatives
- Adjust based on initiative complexity and risk tier (see Section 16)
- Document any exceptions or variations in the Initiative Charter
- Review and update RACI assignments at each gate

### 1.4 Document Conventions

- **Multiple Rs**: Multiple people may be Responsible for execution
- **Single A**: Only one person should be Accountable (final decision authority)
- **C/I flexibility**: Consulted and Informed roles may vary by initiative context
- **Role Absence**: Empty cells indicate the role is not involved in that activity

---

## 2. RACI Definitions

| Code | Term | Definition |
|------|------|------------|
| **R** | **Responsible** | The person(s) who performs the work to complete the task. Multiple people can be Responsible. |
| **A** | **Accountable** | The person who is ultimately answerable for the correct and thorough completion of the task. Only ONE person should be Accountable. This is the final decision maker. |
| **C** | **Consulted** | The person(s) whose input and expertise are sought before a decision or action is taken. Two-way communication. |
| **I** | **Informed** | The person(s) who need to be kept informed of progress or decisions. One-way communication. |

### Key Principles

1. **Every activity must have exactly one "A" (Accountable)**
2. **Every activity should have at least one "R" (Responsible)**
3. **"C" and "I" should be limited to those who genuinely need to be involved**
4. **The person who is "A" can also be "R" for the same activity**

---

## 3. Role Definitions

### 3.1 Core Roles

| Role | Description | Typical Incumbent |
|------|-------------|-------------------|
| **Business Sponsor** | Senior business leader sponsoring the initiative, provides business requirements and funding | Department Head, Division Chief |
| **Business Owner** | Day-to-day business point of contact, defines requirements and validates outcomes | Business Unit Manager, Process Owner |
| **Head of Digital Products** | Senior product leader responsible for backlog management, requirements prioritization, UAT coordination, and business/stakeholder management | Head of Digital Products, Innovation & Digitization |
| **AI Engineering Lead** | Head of AI Engineering team, overall accountability for AI/ML and Automation delivery | Head of AI Engineering |
| **Business Analyst** | Analyzes business requirements, documents processes, bridges business and technical teams | Business Analyst (Innovation & Digitization) |
| **Data Scientist** | Develops AI/ML models, performs data analysis and model training | Data Scientist (when hired) |
| **ML Engineer** | Implements ML pipelines, handles MLOps, model deployment | ML Engineer (when hired) |
| **Automation Developer** | Develops RPA bots, Power Automate flows, automation solutions | Automation Developer (when hired) / Business Analyst |
| **Solution Architect** | Defines solution architecture, makes technology decisions, creates ADRs | Enterprise Architect / AI Engineering Lead |
| **Data Engineer** | Builds data pipelines, manages data infrastructure | IT Department - Data Team |
| **Model Validator** | Performs independent validation of AI/ML models | Model Risk Management / External Validator |
| **QA/Tester** | Tests solutions, validates functionality, performs UAT coordination | Business Analyst / QA Team |
| **IT Security** | Reviews security requirements, conducts security assessments | Information Security Team |
| **Compliance Officer** | Ensures regulatory compliance, reviews compliance requirements | Compliance Department |
| **Risk Manager** | Assesses and manages risks, provides risk perspective | Risk Management Department |
| **IT Infrastructure** | Provides infrastructure, manages environments | IT Department - Infrastructure Team |
| **IT Operations** | Manages production operations, handles incidents | IT Department - Operations Team |
| **Enterprise Architecture** | Reviews architecture alignment, approves architecture decisions | Enterprise Architecture Team |
| **Data Governance** | Ensures data governance compliance, reviews data usage | Data Governance Office |
| **Internal Audit** | Third-line assurance, audit reviews | Internal Audit Department |
| **Steering Committee** | Senior governance body for Tier 1 initiatives | AI & Automation Steering Committee |

### 3.2 Role Abbreviations (Used in RACI Tables)

| Abbreviation | Full Role |
|--------------|-----------|
| **BizSpon** | Business Sponsor |
| **BizOwn** | Business Owner |
| **DigProdHead** | Head of Digital Products |
| **AILead** | AI Engineering Lead |
| **BA** | Business Analyst |
| **DS** | Data Scientist |
| **MLE** | ML Engineer |
| **AutoDev** | Automation Developer |
| **SolArch** | Solution Architect |
| **DataEng** | Data Engineer |
| **ModelVal** | Model Validator |
| **QA** | QA/Tester |
| **ItSec** | IT Security |
| **Comply** | Compliance Officer |
| **Risk** | Risk Manager |
| **ItInfra** | IT Infrastructure |
| **ItOps** | IT Operations |
| **EntArch** | Enterprise Architecture |
| **DataGov** | Data Governance |
| **Audit** | Internal Audit |
| **SteerCom** | Steering Committee |

---

## 4. Governance Activities RACI

### 4.1 Strategic Governance

| Activity | BizSpon | AILead | SteerCom | Comply | Risk | EntArch | Audit |
|----------|---------|--------|----------|--------|------|---------|-------|
| Define AI/ML strategy and roadmap | C | R/A | C | C | C | C | I |
| Approve annual AI/ML budget | A | R | C | I | I | I | I |
| Set governance policies and standards | C | R/A | C | C | C | C | I |
| Review and update governance framework | I | R/A | C | C | C | C | C |
| Approve technology standards | I | R | C | I | I | A | I |
| Define risk appetite for AI/ML initiatives | C | C | A | C | R | I | C |
| Oversee portfolio performance | C | R/A | C | I | I | I | I |

### 4.2 Operational Governance

| Activity | BizSpon | DigProdHead | AILead | BA | SteerCom | Comply | Risk | EntArch |
|----------|---------|-------------|--------|-----|----------|--------|------|---------|
| Manage intake process | I | R | A | R | I | I | I | I |
| Prioritize initiatives | C | R/A | A | R | C* | I | I | I |
| Track initiative progress | I | R | A | R | I | I | I | I |
| Manage initiative risks and issues | C | R | A | R | I | C | C | I |
| Report to Steering Committee | C | R | R/A | R | I | I | I | I |
| Maintain model inventory | I | C | A | R | I | I | I | I |
| Conduct periodic reviews | C | R | A | R | I | C | C | I |

*SteerCom = Consulted for Tier 1 initiatives only

---

## 5. Gate 0: Intake & Prioritization RACI

### 5.1 Use Case Submission

| Activity | BizSpon | BizOwn | DigProdHead | AILead | BA | SteerCom | Comply | Risk |
|----------|---------|---------|-------------|--------|-----|----------|--------|------|
| Identify business problem/opportunity | A | R | C | I | I | I | I | I |
| Complete Use Case Intake Form | C | A | R | C | R | I | I | I |
| Define success metrics | A | R | R | C | C | I | I | I |
| Estimate business benefits | A | R | R | I | C | I | I | I |
| Identify stakeholders | R | R | R | C | C | I | I | I |

### 5.2 Initial Screening

| Activity | BizSpon | BizOwn | AILead | BA | DS | AutoDev | ItSec | Comply | Risk | EntArch | DataGov |
|----------|---------|---------|--------|-----|-----|---------|-------|--------|------|---------|---------|
| Review intake submission | I | I | A | R | C | C | I | I | I | I | I |
| Assess strategic alignment | C | C | R/A | R | I | I | I | I | I | I | I |
| Assess technical feasibility (preliminary) | I | C | R | R | R | R | I | I | I | C | I |
| Identify data availability | I | C | R | R | R | I | I | I | I | I | C |
| Assess regulatory sensitivity | I | C | C | R | I | I | C | R | R | I | C |
| Assess security sensitivity | I | I | C | R | I | I | R | I | C | I | I |
| Determine risk tier (Tier 1/2/3) | I | I | A | R | I | I | C | C | R | I | I |
| Calculate prioritization score | I | C | A | R | I | I | I | I | I | I | I |

### 5.3 Intake Decision

| Activity | BizSpon | AILead | BA | SteerCom | Comply | Risk |
|----------|---------|--------|-----|----------|--------|------|
| Present to decision authority | I | R | R | I* | I* | I* |
| Make intake decision (Approve/Defer/Reject) | I | A** | R | A* | I | I |
| Communicate decision to stakeholders | I | A | R | I | I | I |
| Log decision and rationale | I | A | R | I | I | I |
| Update intake pipeline | I | A | R | I | I | I |

*For Tier 1 initiatives
**AILead accountable for Tier 2/3; SteerCom accountable for Tier 1

---

## 6. Gate 1: Discovery & Feasibility RACI

### 6.1 Requirements Analysis

| Activity | BizSpon | BizOwn | DigProdHead | AILead | BA | DS | AutoDev | DataEng | DataGov |
|----------|---------|---------|-------------|--------|-----|-----|---------|---------|---------|
| Conduct requirements workshops | I | R | R | C | R/A | R | R | I | I |
| Document business requirements | I | R | R | C | R/A | C | C | I | I |
| Define functional requirements | I | R | R | C | R/A | R | R | I | I |
| Define non-functional requirements | I | C | C | R | R/A | R | R | C | I |
| Document as-is process (automation) | I | R | C | C | R/A | I | R | I | I |
| Identify exception scenarios | I | R | R | C | R/A | C | R | I | I |
| Volume and frequency analysis (automation) | I | R | C | C | R/A | I | R | I | I |

### 6.2 Data Assessment

| Activity | BizSpon | BizOwn | AILead | BA | DS | DataEng | ItSec | DataGov |
|----------|---------|---------|--------|-----|-----|---------|-------|---------|
| Identify data sources | I | R | C | R | R | R | I | C |
| Assess data availability | I | C | C | R | R | R | I | C |
| Assess data quality | I | I | C | R | R | R | I | R |
| Evaluate data access requirements | I | C | C | R | R | R | R | R |
| Identify data gaps and remediation | I | C | R/A | R | R | R | I | C |
| Assess PII/sensitive data handling | I | I | C | R | C | I | R | R |
| Document data lineage | I | I | C | R | R | R | I | R |

### 6.3 Technical Feasibility

| Activity | BizSpon | AILead | BA | DS | MLE | AutoDev | SolArch | EntArch |
|----------|---------|--------|-----|-----|-----|---------|---------|---------|
| Conduct proof of concept (if required) | I | R | C | R | R | R | C | I |
| Evaluate ML algorithms (AI initiatives) | I | R | I | R/A | R | I | C | I |
| Evaluate automation approach (RPA initiatives) | I | R | C | I | I | R/A | C | I |
| Assess technical risks | I | R/A | R | R | R | R | C | C |
| Identify technology dependencies | I | R | R | R | R | R | R | C |
| Estimate development effort | I | R/A | R | R | R | R | C | I |
| Recommend approach | I | R/A | R | R | R | R | C | C |

### 6.4 Risk & Compliance Assessment

| Activity | BizSpon | AILead | BA | ItSec | Comply | Risk | DataGov |
|----------|---------|--------|-----|-------|--------|------|---------|
| Identify compliance requirements | I | C | R | C | R/A | C | C |
| Conduct regulatory impact assessment | C | C | R | I | R/A | R | C |
| Identify ethical considerations | C | C | R | I | R | R | C |
| Assess fairness and bias risks (AI) | I | C | R | I | C | R/A | C |
| Document risk mitigation approach | I | R | R | C | C | R/A | I |

### 6.5 Feasibility Decision (Gate 1 Approval)

| Activity | BizSpon | BizOwn | AILead | BA | SteerCom | Risk |
|----------|---------|---------|--------|-----|----------|------|
| Prepare feasibility report | I | C | R | R/A | I | I |
| Present to decision authority | C | C | R | R | I* | I* |
| Make feasibility decision (Go/No-Go) | C | C | A** | R | A* | C |
| Approve resource allocation | A | I | R | C | C* | I |
| Define project charter | I | C | R/A | R | I | I |

*For Tier 1 initiatives
**AILead accountable for Tier 2/3; SteerCom accountable for Tier 1

---

## 7. Gate 2: Design Phase RACI

### 7.1 Solution Design (AI/ML Initiatives)

| Activity | BizOwn | AILead | BA | DS | MLE | SolArch | DataEng | EntArch |
|----------|---------|--------|-----|-----|-----|---------|---------|---------|
| Design overall solution architecture | I | R | C | R | R | R/A | C | C |
| Select ML algorithms and approach | I | R | C | R/A | R | C | I | I |
| Design feature engineering approach | I | C | C | R/A | R | I | C | I |
| Design model training strategy | I | R | C | R/A | R | C | I | I |
| Design explainability approach | C | R | C | R/A | R | C | I | I |
| Design data pipeline architecture | I | R | C | R | R | C | R/A | C |
| Define model performance targets | C | R | R | R/A | R | C | I | I |

### 7.2 Solution Design (Automation Initiatives)

| Activity | BizOwn | AILead | BA | AutoDev | SolArch | DataEng | EntArch |
|----------|---------|--------|-----|---------|---------|---------|---------|
| Design to-be process flow | R | C | R/A | R | C | I | I |
| Design automation architecture | C | R | R | R/A | R/A | C | C |
| Design exception handling approach | R | C | R | R/A | C | I | I |
| Design bot/flow components | I | C | C | R/A | C | I | I |
| Design orchestration and scheduling | I | R | R | R/A | C | I | I |
| Design integration approach | C | R | R | R/A | C | R | C |

### 7.3 Integration & Infrastructure Design

| Activity | AILead | BA | MLE | AutoDev | SolArch | DataEng | ItInfra | EntArch |
|----------|--------|-----|-----|---------|---------|---------|---------|---------|
| Define integration requirements | C | R | R | R | R/A | R | C | C |
| Design API specifications | I | C | R | R | R/A | C | C | C |
| Define infrastructure requirements | C | C | R | R | R | C | R/A | C |
| Design deployment architecture | C | C | R | R | R/A | C | R | C |
| Plan environment strategy (dev/test/prod) | C | C | R | R | R | C | R/A | C |

### 7.4 Security & Compliance Design

| Activity | AILead | BA | MLE | AutoDev | ItSec | Comply | DataGov |
|----------|--------|-----|-----|---------|-------|--------|---------|
| Define security requirements | C | R | R | R | R/A | C | C |
| Design access controls | I | R | R | R | R/A | I | C |
| Design data protection measures | I | R | R | R | R/A | C | R |
| Design audit logging | I | R | R | R | R/A | C | C |
| Design compliance controls | C | R | C | C | C | R/A | C |

### 7.5 Architecture Decision Records

| Activity | AILead | MLE | AutoDev | SolArch | EntArch |
|----------|--------|-----|---------|---------|---------|
| Document architecture decisions (ADRs) | R | R | R | R/A | C |
| Review and approve ADRs | A | I | I | R | A** |
| Maintain ADR repository | R/A | I | I | R | I |

**EntArch approval for decisions impacting enterprise standards

### 7.6 Design Approval (Gate 2)

| Activity | BizOwn | AILead | SolArch | SteerCom | Risk | EntArch |
|----------|---------|--------|---------|----------|------|---------|
| Prepare Solution Design Document | C | R | R/A | I | I | I |
| Review solution design | C | R | R | I* | C* | R |
| Approve solution design | C | A** | R | A* | I | C |
| Approve build phase resource plan | C | A | R | C* | I | I |

*For Tier 1 initiatives
**AILead accountable for Tier 2/3; SteerCom accountable for Tier 1

---

## 8. Gate 3: Build Phase RACI

### 8.1 Environment Setup

| Activity | AILead | DS | MLE | AutoDev | DataEng | ItInfra | ItSec |
|----------|--------|-----|-----|---------|---------|---------|-------|
| Provision development environment | C | I | R | R | C | R/A | C |
| Configure source control | R | R | R | R | I | C | C |
| Setup CI/CD pipeline | C | C | R/A | R | C | R | C |
| Provision test data | C | R | R | R | R/A | R | C |
| Configure secrets management | C | C | R | R | I | R | R/A |

### 8.2 Data Preparation (AI/ML Initiatives)

| Activity | AILead | DS | MLE | DataEng | DataGov |
|----------|--------|-----|-----|---------|---------|
| Build data extraction pipelines | C | R | R | R/A | I |
| Implement data quality checks | C | R | R | R | C |
| Perform data cleaning and preprocessing | C | R/A | R | R | I |
| Implement feature engineering | C | R/A | R | C | I |
| Create feature store (if applicable) | C | R | R/A | R | C |
| Document data transformations | C | R/A | R | R | C |

### 8.3 Model Development (AI/ML Initiatives)

| Activity | AILead | DS | MLE | BA |
|----------|--------|-----|-----|-----|
| Develop model training code | C | R/A | R | I |
| Conduct model experiments | C | R/A | R | I |
| Perform hyperparameter tuning | C | R/A | R | I |
| Implement model explainability | C | R/A | R | C |
| Conduct bias and fairness testing | C | R/A | R | C |
| Select final model | R | R/A | R | C |
| Document Model Card | C | R/A | R | R |

### 8.4 Automation Development (Automation Initiatives)

| Activity | AILead | BA | AutoDev |
|----------|--------|-----|---------|
| Build bot/flow components | C | R | R/A |
| Implement exception handling | C | R | R/A |
| Implement logging and monitoring | R | R | R/A |
| Develop reusable components | C | C | R/A |
| Implement bot orchestration | C | R | R/A |
| Document bot/flow design | C | R/A | R |

### 8.5 Code Quality & Testing

| Activity | AILead | BA | DS | MLE | AutoDev | QA |
|----------|--------|-----|-----|-----|---------|-----|
| Conduct code reviews | R | C | R | R | R | I |
| Write unit tests | C | C | R | R | R | C |
| Perform unit testing | C | R | R | R | R | R |
| Perform integration testing | C | R | R | R | R | R/A |
| Test exception handling | C | R | R | R | R | R |
| Fix defects | C | C | R | R | R | C |

### 8.6 Documentation

| Activity | AILead | BA | DS | MLE | AutoDev |
|----------|--------|-----|-----|-----|---------|
| Create technical documentation | C | R | R | R | R |
| Document code and components | C | C | R/A | R | R |
| Create user/operator guides | C | R/A | C | C | R |
| Update Solution Design Document | C | R/A | R | R | R |
| Prepare validation handoff package | R | R | R | R | R |

---

## 9. Gate 4: Validation & Testing RACI

### 9.1 Model Validation (AI/ML Initiatives)

| Activity | BizOwn | AILead | DS | MLE | ModelVal | Risk |
|----------|---------|--------|-----|-----|----------|------|
| Conduct conceptual soundness review | I | C | C | C | R/A | C |
| Validate data quality | I | C | R | R | R/A | I |
| Validate model performance | I | C | R | R | R/A | C |
| Test model stability | I | C | R | R | R/A | I |
| Conduct sensitivity analysis | I | C | R | R | R/A | I |
| Validate bias and fairness | I | C | R | R | R/A | C |
| Benchmark against alternatives | I | C | R | R | R/A | I |
| Document limitations and assumptions | I | C | R | R | R/A | I |
| Prepare validation report | I | C | C | C | R/A | C |
| Sign-off validation | I | C | I | I | R | A |

### 9.2 Automation Testing (Automation Initiatives)

| Activity | BizOwn | AILead | BA | AutoDev | QA |
|----------|---------|--------|-----|---------|-----|
| Execute functional testing | C | C | R | R | R/A |
| Test exception scenarios | C | C | R | R | R/A |
| Perform volume testing | C | C | R | R | R/A |
| Test recovery procedures | I | C | R | R | R/A |
| Verify logging and monitoring | I | R | R | R | R |
| Peer validation (Tier 2) | I | R | R | R | A |

### 9.3 User Acceptance Testing

| Activity | BizOwn | DigProdHead | AILead | BA | QA |
|----------|---------|-------------|--------|-----|-----|
| Prepare UAT plan and test cases | R | R | C | R/A | R |
| Coordinate UAT execution | R | R/A | C | R | R |
| Execute UAT test cases | R/A | R | I | R | R |
| Document UAT results | R | R | C | R/A | R |
| Sign-off UAT | A | R | I | R | C |

### 9.4 Security & Compliance Testing

| Activity | AILead | MLE | AutoDev | ItSec | Comply |
|----------|--------|-----|---------|-------|--------|
| Conduct security testing | C | R | R | R/A | I |
| Perform vulnerability scanning | C | C | C | R/A | I |
| Test access controls | C | R | R | R/A | I |
| Review compliance controls | C | C | C | C | R/A |
| Document security assessment | C | C | C | R/A | C |
| Sign-off security review | I | I | I | A | C |

### 9.5 Validation Approval (Gate 3)

| Activity | BizOwn | AILead | ModelVal | SteerCom | Risk | Comply |
|----------|---------|--------|----------|----------|------|--------|
| Review validation findings | R | R | R | I* | C | C |
| Address validation findings | C | R | C | I | I | I |
| Approve validation completion | C | A** | C | A* | C | C |
| Approve for production deployment | C | A** | I | A* | C | C |

*For Tier 1 initiatives
**AILead accountable for Tier 2/3; SteerCom accountable for Tier 1

---

## 10. Gate 5: Deployment RACI

### 10.1 Pre-Deployment Preparation

| Activity | BizOwn | AILead | MLE | AutoDev | ItInfra | ItOps |
|----------|---------|--------|-----|---------|---------|-------|
| Prepare deployment runbook | I | R | R/A | R | C | C |
| Provision production infrastructure | I | C | R | R | R/A | C |
| Configure production environment | I | C | R | R | R | R/A |
| Conduct deployment rehearsal | I | R | R | R | C | R |
| Prepare rollback plan | I | R | R/A | R | C | R |
| Complete pre-deployment checklist | I | A | R | R | C | R |

### 10.2 Deployment Execution

| Activity | BizOwn | AILead | MLE | AutoDev | ItInfra | ItOps |
|----------|---------|--------|-----|---------|---------|-------|
| Execute deployment | I | R | R/A | R | R | R |
| Configure monitoring and alerting | I | R | R | R | C | R/A |
| Conduct smoke testing | C | R | R | R | C | R |
| Verify integrations | C | R | R | R | R | R |
| Activate production monitoring | I | R | R | R | C | R/A |

### 10.3 Cutover & Go-Live

| Activity | BizOwn | AILead | MLE | AutoDev | ItOps |
|----------|---------|--------|-----|---------|-------|
| Coordinate cutover activities | R | R/A | R | R | R |
| Execute cutover plan | R | R | R | R | R |
| Verify production functionality | R/A | R | R | R | R |
| Provide hypercare support | R | R | R | R | R |
| Monitor initial production runs | R | R | R | R | R/A |

### 10.4 Production Approval (Gate 4)

| Activity | BizOwn | AILead | SteerCom | ItOps |
|----------|---------|--------|----------|-------|
| Validate deployment success | R | R | I* | R |
| Approve production go-live | A | R** | A* | C |
| Sign-off production release | R | A | I | C |

*For Tier 1 initiatives
**AILead makes recommendation; BizOwn accountable for business approval

---

## 11. Post-Implementation Review RACI

### 11.1 Benefits Realization (Gate 5)

| Activity | BizSpon | BizOwn | DigProdHead | AILead | BA |
|----------|---------|---------|-------------|--------|-----|
| Measure actual benefits vs. expected | C | R/A | R | C | R |
| Assess business impact | R | R/A | R | C | R |
| Document lessons learned | C | R | R | R/A | R |
| Identify improvement opportunities | C | R | R | R | R |

### 11.2 Technical Performance Review

| Activity | BizOwn | AILead | DS | MLE | AutoDev | ItOps |
|----------|---------|--------|-----|-----|---------|-------|
| Review model/bot performance metrics | C | R/A | R | R | R | R |
| Assess technical stability | I | R/A | R | R | R | R |
| Review incident history | I | R/A | C | C | C | R |
| Identify technical improvements | I | R/A | R | R | R | R |

### 11.3 PIR Approval

| Activity | BizSpon | BizOwn | DigProdHead | AILead | SteerCom |
|----------|---------|---------|-------------|--------|----------|
| Prepare PIR report | C | R | R | R/A | I |
| Present PIR findings | C | R | R | R | I* |
| Approve PIR closure | C | R | R | A** | A* |

*For Tier 1 initiatives
**AILead accountable for Tier 2/3; SteerCom accountable for Tier 1

---

## 12. Ongoing Operations & Maintenance RACI

### 12.1 Production Monitoring

| Activity | BizOwn | AILead | DS | MLE | AutoDev | ItOps |
|----------|---------|--------|-----|-----|---------|-------|
| Monitor model/bot performance | C | R | R | R | R | R/A |
| Monitor data drift (AI/ML) | I | R | R/A | R | I | C |
| Monitor prediction quality (AI/ML) | C | R | R/A | R | I | C |
| Monitor bot execution (Automation) | C | R | C | I | R | R/A |
| Monitor system health | I | R | C | C | C | R/A |
| Review monitoring dashboards | C | R | R | R | R | R |
| Respond to monitoring alerts | I | R | R | R | R | R/A |

### 12.2 Incident Management

| Activity | BizOwn | AILead | DS | MLE | AutoDev | ItOps |
|----------|---------|--------|-----|-----|---------|-------|
| Respond to production incidents | C | R | R | R | R | R/A |
| Investigate root cause | I | R | R | R | R | R |
| Implement fixes | I | R | R | R | R | R |
| Document incidents and resolutions | I | R | R | R | R | R/A |
| Conduct incident post-mortems | C | R/A | R | R | R | R |

### 12.3 Maintenance & Support

| Activity | BizOwn | AILead | DS | MLE | AutoDev | ItOps |
|----------|---------|--------|-----|-----|---------|-------|
| Perform routine maintenance | I | R | R | R | R | R/A |
| Apply patches and updates | I | R | R | R | R | R |
| Update documentation | I | R | R | R | R | C |
| Provide user support | R | C | C | C | C | C |
| Handle change requests | R | R | C | C | C | C |

### 12.4 Performance Reporting

| Activity | BizSpon | BizOwn | AILead | BA | SteerCom |
|----------|---------|---------|--------|-----|----------|
| Generate performance reports | I | C | R | R/A | I |
| Analyze performance trends | I | R | R | R | I |
| Report to business stakeholders | I | R/A | R | R | I |
| Report to Steering Committee (Tier 1) | C | C | R | R | I |

### 12.5 Periodic Reviews

| Activity | BizOwn | AILead | DS | MLE | AutoDev | ModelVal | Risk |
|----------|---------|--------|-----|-----|---------|----------|------|
| Conduct quarterly reviews (Tier 1) | R | R/A | R | R | R | C | C |
| Conduct semi-annual reviews (Tier 2) | R | R/A | R | R | R | C | I |
| Conduct annual reviews (Tier 3) | R | R/A | R | R | R | I | I |
| Assess continued appropriateness | R | R | R | R | R | C | C |
| Recommend retraining/updates | C | R | R/A | R | R | I | I |
| Update model inventory | I | R | C | C | C | I | I |

---

## 13. Retraining & Enhancement RACI

### 13.1 Retraining Trigger Assessment (AI/ML)

| Activity | BizOwn | AILead | DS | MLE | ModelVal |
|----------|---------|--------|-----|-----|----------|
| Identify retraining triggers | C | R | R/A | R | I |
| Assess performance degradation | C | R | R/A | R | C |
| Evaluate new data availability | I | R | R/A | R | I |
| Recommend retraining approach | I | R | R/A | R | C |
| Approve retraining initiation | C | A | R | R | I |

### 13.2 Bot/Flow Enhancement (Automation)

| Activity | BizOwn | AILead | BA | AutoDev |
|----------|---------|--------|-----|---------|
| Identify enhancement needs | R | C | R | C |
| Assess process changes | R/A | C | R | C |
| Design enhancements | C | R | R | R/A |
| Approve enhancement scope | A | R | R | C |

### 13.3 Retraining/Enhancement Execution

| Activity | AILead | DS | MLE | AutoDev | ModelVal |
|----------|--------|-----|-----|---------|----------|
| Execute retraining/enhancement | R | R/A | R | R | I |
| Validate retrained model/updated bot | C | R | R | R | R/A |
| Conduct regression testing | R | R | R | R | C |
| Approve for production | A | C | C | C | C** |
| Deploy to production | R | R | R | R | I |

**ModelVal for Tier 1 retraining

### 13.4 Gate Process for Significant Changes

**Note**: Significant retraining or enhancements follow abbreviated gate process:
- **Minor changes**: Fast-track approval (AILead)
- **Moderate changes**: Gates 2, 3, 4 (compressed timeline)
- **Major changes**: Full gate process (Gates 1-5)

---

## 14. Model/Bot Retirement RACI

### 14.1 Retirement Assessment

| Activity | BizSpon | BizOwn | AILead | DS | AutoDev | Risk |
|----------|---------|---------|--------|-----|---------|------|
| Identify retirement candidates | C | R | R/A | R | R | I |
| Assess business impact of retirement | R | R/A | C | I | I | I |
| Assess technical dependencies | I | C | R | R | R | C |
| Evaluate replacement options | C | R | R | R | R | I |
| Recommend retirement decision | I | R | R/A | R | R | C |

### 14.2 Retirement Planning

| Activity | BizOwn | AILead | MLE | AutoDev | ItOps |
|----------|---------|--------|-----|---------|-------|
| Develop retirement plan | C | R | R | R | R |
| Plan data archival | C | R | R | R | C |
| Plan system decommissioning | I | R | R | R | R/A |
| Coordinate with dependent systems | R | R | R | R | R |
| Prepare stakeholder communications | R/A | R | I | I | I |

### 14.3 Retirement Execution

| Activity | BizOwn | AILead | MLE | AutoDev | ItOps |
|----------|---------|--------|-----|---------|-------|
| Execute retirement plan | C | R | R | R | R/A |
| Archive model/bot artifacts | I | R | R | R | R |
| Archive data and documentation | I | R | R | R | R |
| Deactivate production systems | I | R | R | R | R/A |
| Update model inventory | I | R/A | C | C | I |
| Communicate retirement completion | R | R/A | I | I | I |

### 14.4 Retirement Approval

| Activity | BizSpon | BizOwn | AILead | SteerCom |
|----------|---------|---------|--------|----------|
| Approve retirement decision | C | A | R | C* |
| Sign-off retirement completion | C | R | A | I |

*SteerCom for Tier 1 initiatives

---

## 15. Copilot Tools Management RACI

### 15.1 Copilot Provisioning & Licensing

| Activity | DigProdHead | AILead | BA | ItInfra | ItSec | Comply | BizSpon |
|----------|-------------|--------|-----|---------|-------|--------|---------|
| Define Copilot licensing strategy | R | R | C | C | C | C | A |
| Request Copilot licenses (O365, etc.) | R | C | R | R | I | I | A |
| Provision user licenses | I | C | R | R/A | C | I | I |
| Configure tenant settings | I | R | C | R/A | R | C | I |
| Define user eligibility criteria | R | R | R | I | C | R | A |
| Manage license allocation | R/A | C | R | R | I | I | C |
| Track license utilization | R/A | C | R | R | I | I | C |
| Optimize license costs | R/A | C | R | R | I | I | A |

### 15.2 Copilot Governance & Policy Management

| Activity | DigProdHead | AILead | ItSec | Comply | DataGov | BizSpon |
|----------|-------------|--------|-------|--------|---------|---------|
| Define Copilot usage policies | R | R/A | R | R | R | C |
| Configure data protection policies | C | R | R/A | R | R | I |
| Define acceptable use guidelines | R | R | C | R | C | C |
| Configure prompt controls | C | R/A | R | C | C | I |
| Manage data residency settings | I | R | R | R | R/A | I |
| Define sensitive data handling rules | C | R | R | R | R/A | C |
| Review and update policies | R | R/A | R | R | R | C |
| Enforce policy compliance | R | R/A | R | R | C | I |

### 15.3 Copilot User Training & Enablement

| Activity | DigProdHead | AILead | BA | BizOwn | ItInfra |
|----------|-------------|--------|-----|---------|---------|
| Develop Copilot training materials | R/A | R | R | C | I |
| Create usage guidelines and best practices | R/A | R | R | C | I |
| Conduct user onboarding sessions | R/A | C | R | C | C |
| Provide prompt engineering training | R | R/A | R | C | I |
| Develop use case examples | R/A | R | R | R | I |
| Create FAQ and help documentation | R/A | C | R | C | I |
| Conduct train-the-trainer sessions | R/A | C | R | C | I |
| Measure training effectiveness | R/A | C | R | C | I |

### 15.4 Copilot Usage Monitoring & Analytics

| Activity | DigProdHead | AILead | BA | ItSec | Comply | DataGov |
|----------|-------------|--------|-----|-------|--------|---------|
| Monitor usage patterns and adoption | R/A | R | R | C | I | I |
| Track prompt quality and effectiveness | R | R/A | R | I | I | I |
| Analyze user engagement metrics | R/A | C | R | I | I | I |
| Monitor for policy violations | R | R | C | R | R | C |
| Review sensitive data exposure risks | C | R | C | R/A | R | R |
| Generate usage reports and dashboards | R/A | C | R | C | I | I |
| Identify optimization opportunities | R/A | R | R | I | I | I |
| Report usage metrics to leadership | R/A | C | R | I | I | I |

### 15.5 Copilot Support & Issue Resolution

| Activity | DigProdHead | AILead | BA | ItInfra | ItSec |
|----------|-------------|--------|-----|---------|-------|
| Provide first-line user support | R/A | C | R | C | I |
| Troubleshoot technical issues | C | R | R | R/A | C |
| Escalate to Microsoft support | C | R | R | R/A | I |
| Manage incident tickets | R | C | R | R | I |
| Document known issues and workarounds | R | R | R/A | C | I |
| Coordinate with IT for infrastructure issues | R | R/A | C | R | C |
| Communicate service disruptions | R/A | C | R | R | I |
| Track and resolve user feedback | R/A | C | R | I | I |

### 15.6 Copilot Performance & Cost Management

| Activity | DigProdHead | AILead | BA | ItInfra | BizSpon |
|----------|-------------|--------|-----|---------|---------|
| Monitor Copilot performance metrics | R | R/A | R | R | I |
| Track API usage and throttling | C | R/A | C | R | I |
| Analyze cost vs. value metrics | R/A | C | R | I | C |
| Optimize token consumption | C | R/A | R | R | I |
| Review service health and availability | R | R/A | C | R | I |
| Benchmark against industry standards | R/A | R | C | I | C |
| Conduct ROI analysis | R/A | C | R | I | A |
| Recommend service improvements | R/A | R | R | C | C |

---

## 16. AI & Automation Hub Management RACI

### 16.1 Hub Platform Management

| Activity | DigProdHead | AILead | BA | ItInfra | EntArch |
|----------|-------------|--------|-----|---------|---------|
| Define Hub vision and roadmap | R | R/A | C | C | C |
| Design Hub architecture and features | C | R/A | R | R | R |
| Develop and maintain Hub platform | R | R/A | R | R | C |
| Configure Hub access controls | C | R | R | R/A | C |
| Manage Hub infrastructure | I | R | C | R/A | C |
| Deploy Hub updates and enhancements | C | R/A | R | R | C |
| Monitor Hub performance and availability | R | R/A | R | R | I |
| Ensure Hub security and compliance | C | R | C | R | R |

### 16.2 Hub Content & Catalog Management

| Activity | DigProdHead | AILead | BA | DS | AutoDev |
|----------|-------------|--------|-----|-----|---------|
| Curate AI/Automation solution catalog | R/A | R | R | C | C |
| Document available models and bots | C | R | R/A | R | R |
| Maintain use case library | R/A | R | R | C | C |
| Publish best practices and guidelines | R | R/A | R | C | C |
| Create solution templates and accelerators | C | R | R/A | R | R |
| Manage Hub taxonomy and metadata | R/A | R | R | C | C |
| Update model/bot documentation | C | R | R | R | R |
| Retire outdated content | R | R/A | R | C | C |

### 16.3 Hub User Access & Onboarding

| Activity | DigProdHead | AILead | BA | ItSec | BizOwn |
|----------|-------------|--------|-----|-------|--------|
| Define Hub user roles and permissions | R | R/A | R | R | C |
| Manage user access requests | R/A | C | R | R | C |
| Onboard new Hub users | R/A | C | R | I | C |
| Provide Hub orientation training | R/A | C | R | I | C |
| Create user guides and tutorials | R/A | R | R | I | C |
| Manage user directories and profiles | R | C | R | R | I |
| Review and audit user access | R | R | R | R/A | I |
| Deactivate user access when needed | R | C | R | R/A | I |

### 16.4 Hub Usage Analytics & Reporting

| Activity | DigProdHead | AILead | BA | BizSpon | SteerCom |
|----------|-------------|--------|-----|---------|----------|
| Track Hub usage and adoption metrics | R/A | R | R | I | I |
| Monitor most accessed solutions | R/A | R | R | I | I |
| Analyze user engagement patterns | R/A | C | R | I | I |
| Generate Hub analytics reports | R/A | C | R | I | I |
| Measure Hub value and ROI | R/A | R | R | C | I |
| Identify content gaps and needs | R/A | R | R | C | I |
| Report Hub metrics to leadership | R/A | C | R | C | I* |
| Benchmark Hub performance | R/A | R | C | C | I |

*SteerCom for strategic reviews

### 16.5 Hub Support & Community Management

| Activity | DigProdHead | AILead | BA | BizOwn |
|----------|-------------|--------|-----|--------|
| Provide Hub user support | R/A | C | R | C |
| Manage Hub support tickets | R/A | C | R | I |
| Facilitate Hub user community | R/A | R | R | C |
| Organize Hub user forums and events | R/A | C | R | C |
| Collect and prioritize user feedback | R/A | R | R | R |
| Coordinate knowledge sharing sessions | R/A | R | R | C |
| Maintain Hub FAQ and help resources | R/A | C | R | C |
| Recognize and promote Hub champions | R/A | C | C | C |

### 16.6 Hub Integration & Ecosystem Management

| Activity | DigProdHead | AILead | SolArch | ItInfra | EntArch |
|----------|-------------|--------|---------|---------|---------|
| Define Hub integration strategy | R | R/A | R | C | R |
| Integrate Hub with enterprise systems | C | R | R/A | R | R |
| Manage Hub API and SDKs | C | R/A | R | R | C |
| Coordinate with IT on infrastructure | R | R/A | C | R | R |
| Manage third-party tool integrations | R | R/A | R | R | C |
| Ensure Hub interoperability | C | R | R/A | R | R |
| Maintain Hub integration documentation | R | R | R/A | C | C |
| Evaluate new integration opportunities | R/A | R | R | C | C |

### 16.7 Hub Governance & Compliance

| Activity | DigProdHead | AILead | ItSec | Comply | DataGov |
|----------|-------------|--------|-------|--------|---------|
| Define Hub governance policies | R | R/A | R | R | R |
| Ensure Hub regulatory compliance | C | R | R | R/A | R |
| Conduct Hub security assessments | C | R | R/A | C | C |
| Manage Hub data privacy controls | C | R | R | R | R/A |
| Audit Hub access and usage | R | R | R | R | C |
| Review and update Hub policies | R | R/A | R | R | R |
| Report Hub compliance status | R | R | C | R/A | C |
| Manage Hub risk register | C | R/A | C | R | C |

---

## 17. Initiative Type Variations

### 17.1 AI/ML Initiative Specifics

**Additional/Enhanced Roles**:
- Data Scientist (DS) and ML Engineer (MLE) are primary Responsible parties
- Model Validator has significant involvement in validation stage
- Data Engineer more heavily involved in data pipeline activities

**Key Differences**:
- Emphasis on data quality, feature engineering, model performance
- Formal model validation required (independent for Tier 1)
- Model Card documentation mandatory
- Data drift monitoring critical in operations
- Retraining as ongoing lifecycle activity

### 17.2 Automation Initiative Specifics

**Additional/Enhanced Roles**:
- Business Analyst and Automation Developer are primary Responsible parties
- Business Owner has heavier involvement throughout
- IT Operations more involved in bot execution monitoring

**Key Differences**:
- Emphasis on process documentation, exception handling
- Process flow diagrams and SDD are critical artifacts
- Peer validation acceptable for Tier 2 (vs. independent)
- Bot execution monitoring vs. model performance monitoring
- Process change management triggers updates

### 17.3 Hybrid Initiative (AI + Automation)

**Approach**:
- Combine RACIs from both AI/ML and Automation tracks
- Both Data Scientist/ML Engineer AND Automation Developer are Responsible
- Solution Architect plays enhanced coordination role
- Follow strictest governance requirement (typically AI/ML validation approach)

---

## 18. Tier-Based Variations

### 18.1 Tier 1 (High Risk) - Enhanced Governance

**Key Differences**:
- Steering Committee involved in major gate approvals (Gates 0, 2, 3, 4)
- Independent model validation required (external validator for complex models)
- Comprehensive documentation at all stages
- Risk and Compliance consulted throughout
- Quarterly periodic reviews mandatory

### 18.2 Tier 2 (Medium Risk) - Standard Governance

**Key Differences**:
- AI Engineering Lead is primary approval authority
- Peer validation acceptable (internal team member not involved in development)
- Standard documentation requirements
- Semi-annual periodic reviews

### 18.3 Tier 3 (Low Risk) - Streamlined Governance

**Key Differences**:
- Fast-track gate consolidation available
- AI Engineering Lead can delegate approvals
- Self-validation acceptable with peer review
- Abbreviated documentation (focus on essentials)
- Annual periodic reviews

### 18.4 Tier-Specific RACI Adjustments

| Activity | Tier 1 | Tier 2 | Tier 3 |
|----------|--------|--------|--------|
| Gate Approvals | SteerCom (A) | AILead (A) | AILead (A), can delegate |
| Model Validation | ModelVal Independent (R/A) | ModelVal Peer (R/A) | Team Self + Peer (R/A) |
| Risk Consultation | Risk (C) at all gates | Risk (C) at Gates 1, 3 | Risk (I) only |
| Compliance Review | Comply (C) at all gates | Comply (C) at Gates 1, 4 | Comply (I) only |
| Documentation | Comprehensive (all) | Standard (all) | Abbreviated (key only) |
| Periodic Reviews | Quarterly | Semi-annual | Annual |

---

## 19. RACI Governance & Maintenance

### 19.1 RACI Review and Updates

| Activity | AILead | BA | SteerCom |
|----------|--------|-----|----------|
| Review RACI annually | R/A | R | C |
| Update RACI for organizational changes | R/A | R | I |
| Approve RACI updates | A | R | C |
| Communicate RACI changes | R/A | R | I |

### 19.2 RACI Exceptions

**Process for RACI Exceptions**:
1. Proposed exceptions documented in Initiative Charter
2. Rationale provided for deviation from standard RACI
3. Exception approved by AI Engineering Lead (or Steering Committee for Tier 1)
4. Exception documented and tracked
5. Exception reviewed at Post-Implementation Review

### 19.3 Conflict Resolution

**When RACI conflicts arise**:
1. Accountable ("A") party makes final decision
2. If conflict involves Accountable party, escalate to next level:
   - Tier 3: AI Engineering Lead
   - Tier 2: AI Engineering Lead
   - Tier 1: Steering Committee
3. Document resolution and update RACI if systemic issue identified

---

## 20. Appendices

### Appendix A: Quick Reference - Gate Approval Matrix

| Gate | Tier 1 Approval | Tier 2 Approval | Tier 3 Approval |
|------|----------------|----------------|----------------|
| Gate 0: Intake | Steering Committee | AI Engineering Lead | AI Engineering Lead |
| Gate 1: Feasibility | AI Engineering Lead + Risk | AI Engineering Lead | AI Engineering Lead |
| Gate 2: Design | Steering Committee | AI Engineering Lead | AI Engineering Lead (delegable) |
| Gate 3: Validation | Steering Committee + Independent Validation | AI Engineering Lead + Peer Validation | AI Engineering Lead + Self-Validation |
| Gate 4: Production | Steering Committee | AI Engineering Lead | AI Engineering Lead (delegable) |
| Gate 5: PIR | Steering Committee | AI Engineering Lead | AI Engineering Lead |

### Appendix B: Quick Reference - Primary Responsible Parties by Phase

| Phase | AI/ML Primary | Automation Primary | Product Management |
|-------|--------------|-------------------|-------------------|
| Intake | Business Analyst | Business Analyst | Head of Digital Products |
| Discovery | Data Scientist + Business Analyst | Business Analyst + Business Owner | Head of Digital Products (requirements) |
| Design | Data Scientist + ML Engineer + Solution Architect | Automation Developer + Business Analyst + Solution Architect | Head of Digital Products (requirements approval) |
| Build | Data Scientist + ML Engineer | Automation Developer + Business Analyst | Head of Digital Products (stakeholder mgmt) |
| Validation | Model Validator + Data Scientist | QA + Automation Developer | Head of Digital Products (UAT coordination) |
| Deployment | ML Engineer + IT Operations | Automation Developer + IT Operations | Head of Digital Products (stakeholder comms) |
| Operations | ML Engineer + IT Operations + Data Scientist | Automation Developer + IT Operations | Head of Digital Products (benefits tracking) |

### Appendix C: Escalation Paths

| Issue Level | Escalation Path |
|------------|----------------|
| **Level 1**: Task/activity level | Team lead (DS/MLE/AutoDev) |
| **Level 2**: Phase/gate level | AI Engineering Lead |
| **Level 3**: Initiative level | Business Sponsor + AI Engineering Lead |
| **Level 4**: Portfolio/strategic | Steering Committee |
| **Level 5**: Enterprise impact | Executive Management |

### Appendix D: Document References

- **AI/ML Governance Operating Model** (AI-GOV-001)
- **AI Use Case Intake & Prioritization Framework** (AI-GOV-002)
- **AI Initiative Approval & Stage-Gate Process** (AI-GOV-003)
- **AI/ML Development Standards** (AI-ENG-001)
- **Automation Development Standards** (AI-ENG-002)
- **Technology Selection & Decision Framework** (AI-ARCH-001)
- **Model Validation Standards** (AI-VAL-001)

---

## Document Control

**Version History**

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.1 | January 2025 | AI Engineering Team | Added Head of Digital Products role; Added Section 15: Copilot Tools Management RACI; Added Section 16: AI & Automation Hub Management RACI |
| 1.0 | January 2025 | AI Engineering Team | Initial RACI matrix covering AI/ML and Automation initiatives |

**Review and Approval**

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Prepared By | AI Engineering Team | | |
| Reviewed By | Business Analysts | | |
| Approved By | Head of AI Engineering | | |

**Distribution**

This document is distributed to:
- All AI Engineering team members
- Business Analysts
- Business Sponsors and Owners
- IT Department (Infrastructure, Operations, Data, Security)
- Model Risk Management
- Compliance Department
- Risk Management
- Enterprise Architecture
- AI & Automation Steering Committee

---

**Document Classification**: Internal Use
**Document Owner**: Head of AI Engineering, Innovation & Digitization Department
**Next Review Date**: January 2026

**For questions or clarifications on roles and responsibilities, contact:**
- AI Engineering Lead: [Contact Information]
- AI Governance Team: [Contact Information]
