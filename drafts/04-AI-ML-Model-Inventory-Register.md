# AI, Automation & Intelligent Solutions Inventory Register

**Document ID:** AI-GOV-004
**Version:** 1.1
**Classification:** Internal
**Owner:** Head of AI Engineering, Innovation & Digitization Department
**Last Review Date:** [Date]
**Next Review Date:** [Date + 12 months]

---

## 1. Executive Summary

### 1.1 Purpose
This document establishes the framework for maintaining a comprehensive inventory of all AI, Automation, and Intelligent Solutions at Bank ABC. The Inventory Register serves as the authoritative source of truth for all AI and Automation assets, enabling effective governance, risk management, and regulatory compliance.

### 1.2 Objectives
- Maintain a complete and accurate inventory of all AI and Automation assets
- Enable effective lifecycle management and governance
- Support regulatory reporting and audit requirements
- Facilitate risk aggregation and portfolio analysis
- Ensure accountability through clear ownership records
- Track FTE savings and business value from automation

### 1.3 Scope
The Inventory Register includes:
- **AI Assets:** Analytical AI models, GenAI implementations, Agentic AI systems
- **Automation Assets:** RPA bots, Workflow automations, Business process automations
- **Hybrid Assets:** Combined AI + Automation solutions
- Third-party and vendor-provided AI/Automation tools
- Assets in all lifecycle stages (development through retirement)
- Shadow/experimental assets (tracked separately)
- Microsoft Power Platform and Copilot implementations

### 1.4 Organizational Context
- **Owning Department:** Innovation & Digitization Department
- **Inventory Owner:** Head of AI Engineering
- **Data Coordination:** IT Department (Data Management)

### 1.5 Regulatory Alignment
This inventory framework aligns with:
- SR 11-7 model inventory requirements
- PRA SS1/23 model risk management principles
- EU AI Act high-risk AI system registration requirements
- CBB operational resilience and technology risk guidelines

---

## 2. Inventory Governance

### 2.1 Roles and Responsibilities

| Role | Department | Responsibilities |
|------|------------|------------------|
| **Head of AI Engineering** | Innovation & Digitization | Overall accountability for inventory completeness and accuracy; Approve new entries |
| **Business Owner** | Business Units | Ensure business information is accurate; approve changes |
| **Data Scientist** | Innovation & Digitization | Create and maintain AI/ML entries; update during development |
| **Business Analyst** | Innovation & Digitization | Create and maintain Automation entries; update during development |
| **Digital Product Owner** | Innovation & Digitization | Coordinate entry creation; validate business context |
| **IT Data Management** | IT Department | Validate data source information |
| **Model Risk (when established)** | Risk | Validate inventory entries; conduct periodic reviews |

### 2.2 Inventory Maintenance Cadence

| Activity | Frequency | Owner |
|----------|-----------|-------|
| New model registration | At Gate 1 (Discovery) | ML Engineer |
| Entry updates | At each gate passage | ML Engineer / MLOps |
| Quarterly completeness review | Quarterly | AI Engineering Lead |
| Annual inventory audit | Annual | Model Risk / Internal Audit |
| Retirement processing | As needed | AI Engineering |

### 2.3 Inventory Quality Standards

| Standard | Requirement |
|----------|-------------|
| Completeness | All production and development models must be registered |
| Accuracy | All fields must be accurate and current |
| Timeliness | Updates within 5 business days of change |
| Traceability | All changes logged with timestamp and user |
| Accessibility | Searchable and reportable by authorized users |

---

## 3. Model Inventory Schema

### 3.1 Core Identification Fields

| Field | Description | Data Type | Required | Example |
|-------|-------------|-----------|----------|---------|
| **Model ID** | Unique identifier | String | Yes | AI-2024-001 |
| **Model Name** | Descriptive name | String | Yes | Retail NBO Recommendation Engine |
| **Model Version** | Current version number | String | Yes | 2.1.0 |
| **Model Alias** | Alternative names | String | No | NBO Engine, Product Recommender |
| **Description** | Brief description | Text | Yes | Predicts next best offer for retail customers |
| **Parent Model ID** | Link to parent (if variant) | String | No | AI-2023-045 |

### 3.2 Classification Fields

| Field | Description | Data Type | Required | Options/Format |
|-------|-------------|-----------|----------|----------------|
| **Asset Category** | Primary category | Enum | Yes | AI, Automation, Hybrid |
| **AI Type** (if AI/Hybrid) | AI sub-category | Enum | Conditional | Analytical AI, GenAI, Agentic AI |
| **Automation Type** (if Automation/Hybrid) | Automation sub-category | Enum | Conditional | RPA, Workflow, Business Process Automation |
| **Model/Bot Category** | Technique | Enum | Yes | Classification, Regression, NLP, LLM, RAG, Agent, Bot, Flow, Ensemble, Other |
| **Algorithm/Platform** | Specific technology | String | Yes | XGBoost, GPT-4, UiPath, Power Automate, etc. |
| **Risk Tier** | Risk classification | Enum | Yes | Tier 1, Tier 2, Tier 3 |
| **Materiality** | Business materiality | Enum | Yes | High, Medium, Low |
| **Customer-Facing** | Direct customer interaction | Boolean | Yes | Yes/No |
| **Decision/Action Automation** | Level of automation | Enum | Yes | Full Auto, Human-Assisted, Recommendation Only |

### 3.2.1 Automation-Specific Classification Fields

| Field | Description | Data Type | Required (if Automation) | Options/Format |
|-------|-------------|-----------|-------------------------|----------------|
| **Automation Platform** | Platform used | Enum | Yes | Power Automate, UiPath, Copilot Studio, Custom |
| **Attended/Unattended** | Bot execution mode | Enum | Yes (if RPA) | Attended, Unattended, Hybrid |
| **Transaction Volume** | Daily transaction volume | Enum | Yes | Low (<100), Medium (100-1000), High (>1000) |
| **FTE Equivalent** | FTE hours saved annually | Decimal | Yes | Hours/year |
| **Process Owner** | Business process owner | String | Yes | Name and role |
| **Schedule** | Run schedule | String | Yes (if unattended) | Cron expression or description |

### 3.3 GenAI-Specific Fields

| Field | Description | Data Type | Required (if GenAI) | Options/Format |
|-------|-------------|-----------|---------------------|----------------|
| **Foundation Model** | Base LLM used | String | Yes | GPT-4, Claude 3, Llama 2, Custom |
| **Foundation Model Provider** | LLM vendor | Enum | Yes | Azure OpenAI, AWS Bedrock, Self-hosted, Other |
| **RAG Enabled** | Uses retrieval augmentation | Boolean | Yes | Yes/No |
| **Vector Database** | Vector store used | String | Conditional | Qdrant, Pinecone, pgvector, OpenSearch |
| **Embedding Model** | Embedding model used | String | Conditional | text-embedding-ada-002, Titan, Custom |
| **Prompt Version** | Current prompt template version | String | Yes | v1.2.3 |
| **Guardrails Enabled** | Content filtering active | Boolean | Yes | Yes/No |
| **Human Review Required** | Output review requirement | Enum | Yes | Always, Conditional, Never |

### 3.4 Agentic AI-Specific Fields

| Field | Description | Data Type | Required (if Agentic) | Options/Format |
|-------|-------------|-----------|----------------------|----------------|
| **Autonomy Level** | Agent autonomy classification | Enum | Yes | L1-Assisted, L2-Supervised, L3-Monitored, L4-Autonomous |
| **Agent Framework** | Framework used | String | Yes | MS Foundry, LangChain, Custom |
| **Platform** | Deployment platform | Enum | Yes | MS Copilot, Power Automate, Copilot Studio, Custom |
| **Tool/API Access** | Systems agent can access | Text | Yes | List of APIs and tools |
| **Action Boundaries** | Defined action limits | Text | Yes | Description of boundaries |
| **Override Mechanism** | Human intervention method | String | Yes | Real-time, Async, Kill switch |
| **Multi-Agent** | Part of multi-agent system | Boolean | Yes | Yes/No |
| **Parent Agent ID** | Orchestrating agent (if applicable) | String | No | AI-2024-AGT-001 |

### 3.5 Business Context Fields

| Field | Description | Data Type | Required | Example |
|-------|-------------|-----------|----------|---------|
| **Business Unit** | Owning business unit | Enum | Yes | Retail Banking, Corporate Banking, Treasury, Operations |
| **Use Case Name** | Business use case | String | Yes | Next Best Offer Recommendations |
| **Use Case ID** | Link to intake record | String | Yes | UC-2024-001 |
| **Business Problem** | Problem being solved | Text | Yes | Improve product adoption through personalized recommendations |
| **Business Outcome** | Expected/achieved outcome | Text | Yes | 15% increase in product adoption |
| **Strategic Initiative** | Linked strategy | String | No | Digital Transformation 2024 |

### 3.6 Ownership and Contacts

| Field | Description | Data Type | Required | Example |
|-------|-------------|-----------|----------|---------|
| **Business Owner** | Business accountable owner | String | Yes | John Smith (VP Retail Products) |
| **Business Owner Email** | Contact email | Email | Yes | john.smith@bankabc.com |
| **Model Developer** | Primary developer | String | Yes | Jane Doe (ML Engineer) |
| **Developer Email** | Contact email | Email | Yes | jane.doe@bankabc.com |
| **Validator** | Person who validated | String | Yes | Bob Johnson (Senior ML Engineer) |
| **Validator Email** | Contact email | Email | Yes | bob.johnson@bankabc.com |
| **Support Team** | Operational support team | String | Yes | AI Engineering - MLOps |
| **Support Email** | Team email | Email | Yes | ai-mlops@bankabc.com |

### 3.7 Lifecycle Status Fields

| Field | Description | Data Type | Required | Options/Format |
|-------|-------------|-----------|----------|----------------|
| **Status** | Current lifecycle status | Enum | Yes | Discovery, Design, Development, Validation, Production, Monitoring, Retired |
| **Current Gate** | Last passed gate | Enum | Yes | Gate 0-5 |
| **Gate 0 Date** | Intake approval date | Date | Yes | YYYY-MM-DD |
| **Gate 1 Date** | Feasibility approval date | Date | Conditional | YYYY-MM-DD |
| **Gate 2 Date** | Design approval date | Date | Conditional | YYYY-MM-DD |
| **Gate 3 Date** | Validation approval date | Date | Conditional | YYYY-MM-DD |
| **Gate 4 Date** | Production approval date | Date | Conditional | YYYY-MM-DD |
| **Gate 5 Date** | PIR completion date | Date | Conditional | YYYY-MM-DD |
| **Production Date** | Go-live date | Date | Conditional | YYYY-MM-DD |
| **Retirement Date** | Retirement date | Date | Conditional | YYYY-MM-DD |

### 3.8 Data Fields

| Field | Description | Data Type | Required | Example |
|-------|-------------|-----------|----------|---------|
| **Primary Data Sources** | Main data sources | Text | Yes | Core Banking, CRM, Transaction History |
| **Data Lineage Link** | Link to data lineage documentation | URL | Yes | [Data Catalog Link] |
| **PII Involved** | Contains PII | Boolean | Yes | Yes/No |
| **PII Types** | Types of PII processed | Text | Conditional | Name, Account Number, Transaction Data |
| **Data Residency** | Data storage location | String | Yes | Bahrain, AWS eu-west-1 |
| **Cross-Border Data** | Data crosses borders | Boolean | Yes | Yes/No |
| **Training Data Date Range** | Training data period | String | Yes | 2022-01-01 to 2023-12-31 |
| **Training Data Volume** | Approximate data size | String | Yes | 10M records, 50GB |
| **Feature Count** | Number of features | Integer | Yes | 150 |

### 3.9 Technical Infrastructure Fields

| Field | Description | Data Type | Required | Example |
|-------|-------------|-----------|----------|---------|
| **Platform** | Deployment platform | Enum | Yes | AWS SageMaker, AWS Bedrock, Azure, On-premises |
| **Serving Infrastructure** | Model serving approach | String | Yes | SageMaker Endpoint, Lambda, ECS, API Gateway |
| **Compute Type** | Compute resources | String | Yes | ml.m5.xlarge, Lambda 512MB |
| **Container Image** | Docker image reference | String | Yes | ecr.aws/bankabc/nbo-model:2.1.0 |
| **Model Artifact Location** | Storage location | String | Yes | s3://bankabc-models/nbo/v2.1.0/ |
| **API Endpoint** | Production endpoint | URL | Conditional | https://api.bankabc.com/ai/nbo/v2 |
| **Repository** | Code repository | URL | Yes | https://github.com/bankabc/nbo-model |
| **CI/CD Pipeline** | Pipeline reference | String | Yes | Jenkins: nbo-model-pipeline |

### 3.10 Performance and Monitoring Fields

| Field | Description | Data Type | Required | Example |
|-------|-------------|-----------|----------|---------|
| **Primary Metric** | Key performance metric | String | Yes | AUC-ROC |
| **Primary Metric Value** | Current metric value | Decimal | Yes | 0.85 |
| **Baseline Metric Value** | Baseline at deployment | Decimal | Yes | 0.83 |
| **Performance Threshold** | Alert threshold | String | Yes | AUC < 0.80 |
| **Monitoring Dashboard** | Link to dashboard | URL | Yes | [Grafana/CloudWatch Link] |
| **Alerting Configuration** | Alert setup reference | String | Yes | PagerDuty: nbo-model-alerts |
| **SLA - Availability** | Availability target | Percentage | Yes | 99.9% |
| **SLA - Latency P99** | Latency target | Milliseconds | Yes | 200ms |
| **Last Performance Review** | Date of last review | Date | Yes | YYYY-MM-DD |
| **Next Performance Review** | Scheduled review date | Date | Yes | YYYY-MM-DD |

### 3.11 Validation and Compliance Fields

| Field | Description | Data Type | Required | Example |
|-------|-------------|-----------|----------|---------|
| **Last Validation Date** | Most recent validation | Date | Yes | YYYY-MM-DD |
| **Next Validation Due** | Next scheduled validation | Date | Yes | YYYY-MM-DD |
| **Validation Type** | Type of validation | Enum | Yes | Independent, Peer, Self |
| **Validation Report Link** | Link to validation report | URL | Yes | [Document Link] |
| **Open Findings Count** | Current open findings | Integer | Yes | 2 |
| **Critical Findings** | Open critical findings | Integer | Yes | 0 |
| **Regulatory Applicability** | Applicable regulations | Text | Yes | SR 11-7, CBB Technology Risk |
| **Compliance Status** | Current compliance status | Enum | Yes | Compliant, Non-Compliant, Under Review |

### 3.12 Documentation Links

| Field | Description | Data Type | Required |
|-------|-------------|-----------|----------|
| **Model Card Link** | Link to model card | URL | Yes |
| **Solution Design Link** | Link to design document | URL | Yes |
| **Architecture Decision Records** | Links to ADRs | URL | Yes |
| **Runbook Link** | Link to deployment runbook | URL | Yes |
| **Training Documentation** | Link to training docs | URL | No |
| **API Documentation** | Link to API docs | URL | Conditional |

### 3.13 Dependencies and Relationships

| Field | Description | Data Type | Required | Example |
|-------|-------------|-----------|----------|---------|
| **Upstream Dependencies** | Models/systems this depends on | Text | Yes | Feature Store, Customer 360 |
| **Downstream Consumers** | Models/systems that depend on this | Text | Yes | Marketing Campaign Engine, Mobile App |
| **Integration Points** | Systems integrated with | Text | Yes | Core Banking API, CRM, Data Lake |
| **Related Models** | Related or predecessor models | Text | No | AI-2023-001 (v1.0) |

### 3.14 Audit Trail Fields

| Field | Description | Data Type | Required |
|-------|-------------|-----------|----------|
| **Created Date** | Record creation date | Timestamp | Yes |
| **Created By** | User who created record | String | Yes |
| **Last Modified Date** | Last update date | Timestamp | Yes |
| **Last Modified By** | User who last updated | String | Yes |
| **Change History** | Log of all changes | Text/Link | Yes |

---

## 4. Model ID Naming Convention

### 4.1 Standard Format

```
AI-[YEAR]-[TYPE]-[SEQUENCE]
```

| Component | Description | Format | Example |
|-----------|-------------|--------|---------|
| AI | Prefix | Fixed | AI |
| YEAR | Year of registration | YYYY | 2024 |
| TYPE | Model type code | 3 chars | ANA, GEN, AGT, HYB |
| SEQUENCE | Sequential number | 3 digits | 001 |

### 4.2 Type Codes

| Code | Type |
|------|------|
| ANA | Analytical AI |
| GEN | GenAI |
| AGT | Agentic AI |
| HYB | Hybrid |
| EXP | Experimental (sandbox) |

### 4.3 Examples
- `AI-2024-ANA-001` - First Analytical AI model registered in 2024
- `AI-2024-GEN-005` - Fifth GenAI model registered in 2024
- `AI-2024-AGT-002` - Second Agentic AI model registered in 2024

---

## 5. Model Versioning

### 5.1 Version Format

```
MAJOR.MINOR.PATCH
```

| Component | When to Increment | Example |
|-----------|-------------------|---------|
| MAJOR | Algorithm/approach change, breaking changes | 1.0.0 → 2.0.0 |
| MINOR | Feature changes, significant retraining | 1.0.0 → 1.1.0 |
| PATCH | Bug fixes, routine retraining | 1.0.0 → 1.0.1 |

### 5.2 Version Governance

| Version Change | Gate Requirement | Inventory Action |
|----------------|------------------|------------------|
| PATCH | Streamlined Gate 3-4 | Update version, dates |
| MINOR | Gate 2-4 | Update version, may update other fields |
| MAJOR | Full gates (1-5) | New inventory entry (link to parent) |

---

## 6. Status Lifecycle

### 6.1 Status Definitions

| Status | Definition | Inventory Actions |
|--------|------------|-------------------|
| **Discovery** | Feasibility assessment in progress | Entry created at Gate 0 |
| **Design** | Solution design in progress | Update after Gate 1 |
| **Development** | Model build in progress | Update after Gate 2 |
| **Validation** | Validation and testing in progress | Update during Gate 3 |
| **Production** | Model deployed and operational | Update after Gate 4 |
| **Monitoring** | Ongoing operations (same as Production) | Production with active monitoring |
| **Under Review** | Periodic review or revalidation | Temporary status during reviews |
| **Suspended** | Temporarily disabled | Manual status change |
| **Retired** | Permanently decommissioned | Final status after retirement |

### 6.2 Status Transition Diagram

```
                                    ┌─────────────┐
                                    │  SUSPENDED  │◄─────────────────────┐
                                    └──────┬──────┘                      │
                                           │                             │
                                           ▼                             │
┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐
│DISCOVERY │──▶│  DESIGN  │──▶│DEVELOPMT │──▶│VALIDATION│──▶│PRODUCTION│──▶│ RETIRED  │
└──────────┘   └──────────┘   └──────────┘   └──────────┘   └─────┬────┘   └──────────┘
     │              │              │              │                │
     │              │              │              │                │
     └──────────────┴──────────────┴──────────────┘                │
                           │                                       │
                           ▼                                       │
                    ┌──────────────┐                               │
                    │   CANCELLED  │◄──────────────────────────────┘
                    └──────────────┘                    (early termination)
```

---

## 7. Inventory Reports

### 7.1 Standard Reports

| Report | Description | Frequency | Audience |
|--------|-------------|-----------|----------|
| **Portfolio Summary** | High-level inventory statistics | Monthly | AI Steering Committee |
| **Risk Distribution** | Models by risk tier | Monthly | AI Steering Committee, Risk |
| **Validation Status** | Upcoming and overdue validations | Weekly | AI Engineering Lead |
| **Performance Summary** | Models with performance alerts | Weekly | AI Engineering |
| **Compliance Status** | Compliance status by model | Monthly | Compliance, Risk |
| **Lifecycle Status** | Models by lifecycle stage | Monthly | AI Engineering |

### 7.2 Portfolio Summary Report Template

**AI/ML Model Portfolio Summary - [Month Year]**

| Metric | Count | Change vs Last Month |
|--------|-------|---------------------|
| Total Models in Inventory | | |
| Production Models | | |
| Models in Development | | |
| Models Retired (YTD) | | |

**By Risk Tier:**
| Tier | Production | Development | Total |
|------|------------|-------------|-------|
| Tier 1 (High) | | | |
| Tier 2 (Medium) | | | |
| Tier 3 (Low) | | | |

**By AI Type:**
| Type | Production | Development | Total |
|------|------------|-------------|-------|
| Analytical AI | | | |
| GenAI | | | |
| Agentic AI | | | |
| Hybrid | | | |

**By Business Unit:**
| Business Unit | Production | Development |
|---------------|------------|-------------|
| Retail Banking | | |
| Corporate Banking | | |
| Treasury | | |
| Operations | | |

**Validation Status:**
| Status | Count |
|--------|-------|
| Validations Due Next 30 Days | |
| Overdue Validations | |
| Open Critical Findings | |
| Open Major Findings | |

### 7.3 Risk Distribution Report Template

| Model ID | Model Name | Risk Tier | Business Unit | Status | Next Validation |
|----------|------------|-----------|---------------|--------|-----------------|
| | | | | | |

### 7.4 Validation Status Report Template

**Upcoming Validations (Next 90 Days):**
| Model ID | Model Name | Risk Tier | Validation Due | Validator | Status |
|----------|------------|-----------|----------------|-----------|--------|
| | | | | | |

**Overdue Validations:**
| Model ID | Model Name | Risk Tier | Original Due Date | Days Overdue | Action Required |
|----------|------------|-----------|-------------------|--------------|-----------------|
| | | | | | |

---

## 8. Inventory Maintenance Procedures

### 8.1 New Model Registration

| Step | Action | Owner | Timeline |
|------|--------|-------|----------|
| 1 | Create new entry at Gate 0 approval | ML Engineer | Within 2 days of Gate 0 |
| 2 | Assign Model ID | AI Engineering Lead | Immediate |
| 3 | Complete core identification fields | ML Engineer | Gate 0 |
| 4 | Complete business context fields | Business Owner | Gate 0 |
| 5 | Complete remaining fields | ML Engineer | Progressive through gates |
| 6 | Review and validate entry | AI Engineering Lead | At Gate 4 |

### 8.2 Entry Update Triggers

| Trigger | Required Updates | Owner |
|---------|------------------|-------|
| Gate passage | Status, gate dates, related fields | ML Engineer |
| Retraining | Version, training data fields, performance | ML Engineer |
| Performance degradation | Performance fields, findings | MLOps Engineer |
| Ownership change | Owner fields | AI Engineering Lead |
| Validation completion | Validation fields, findings | Validator |
| Retirement | Status, retirement date | AI Engineering |

### 8.3 Data Quality Checks

| Check | Frequency | Action if Failed |
|-------|-----------|------------------|
| Completeness (required fields) | Weekly automated | Flag to owner |
| Consistency (status vs dates) | Weekly automated | Flag to owner |
| Staleness (no update > 90 days for production) | Weekly automated | Flag to owner |
| Orphan check (no owner) | Monthly | Escalate to AI Eng Lead |
| Duplicate check | Monthly | Merge or archive |

---

## 9. Integration Points

### 9.1 System Integrations

| System | Integration Type | Data Flow |
|--------|-----------------|-----------|
| Use Case Intake System | Bi-directional | Use case data, status updates |
| Model Registry (technical) | Bi-directional | Model artifacts, versions |
| Monitoring Platform | Inbound | Performance metrics |
| Incident Management | Inbound | Incident references |
| Risk Management System | Outbound | Risk data for aggregation |
| Audit System | Outbound | Audit trail export |

### 9.2 API Endpoints (if system-based)

| Endpoint | Method | Purpose |
|----------|--------|---------|
| /models | GET | List all models (with filters) |
| /models/{id} | GET | Get single model details |
| /models | POST | Create new model entry |
| /models/{id} | PUT | Update model entry |
| /models/{id}/status | PATCH | Update status only |
| /reports/{type} | GET | Generate report |

---

## 10. Access Control

### 10.1 Access Roles

| Role | View | Create | Edit | Delete | Admin |
|------|------|--------|------|--------|-------|
| AI Engineering Lead | All | Yes | All | Yes | Yes |
| ML Engineer | All | Yes | Own | No | No |
| MLOps Engineer | All | No | Ops fields | No | No |
| Business Owner | Own BU | No | Business fields | No | No |
| Risk/Compliance | All | No | Validation fields | No | No |
| Internal Audit | All | No | No | No | No |
| Executive (read-only) | Summary | No | No | No | No |

### 10.2 Sensitive Field Access

| Field Category | Standard Access | Restricted Access |
|----------------|-----------------|-------------------|
| Core identification | All roles | - |
| Business context | All roles | - |
| Technical details | AI Engineering, MLOps | Business (summary only) |
| Performance data | AI Engineering, Risk | Business (summary only) |
| Validation findings | AI Engineering, Risk, Audit | Business (summary only) |

---

## 11. Shadow IT and Experimental Models

### 11.1 Shadow AI Detection
- Quarterly survey to business units
- Technology scanning for unauthorized AI tools
- Cloud cost analysis for unusual ML spend
- Network monitoring for external AI API calls

### 11.2 Experimental/Sandbox Inventory

Experimental models are tracked with:
- Model ID prefix: `AI-[YEAR]-EXP-[SEQ]`
- Status: Experimental
- Reduced documentation requirements
- 90-day auto-expiry (must promote or archive)

### 11.3 Promotion Process

| Step | Action | Gate Equivalent |
|------|--------|-----------------|
| 1 | Complete standard intake form | Gate 0 |
| 2 | Convert to standard Model ID | - |
| 3 | Complete full inventory entry | - |
| 4 | Follow standard stage-gates | Gate 1+ |

---

## 12. Archival and Retention

### 12.1 Retention Requirements

| Record Type | Retention Period | Rationale |
|-------------|------------------|-----------|
| Active model entries | Indefinite | Operational |
| Retired model entries | 7 years post-retirement | Regulatory |
| Audit trail | 7 years | Regulatory |
| Cancelled models | 3 years | Operational |
| Experimental (archived) | 1 year | Operational |

### 12.2 Archival Process

| Step | Action | Owner |
|------|--------|-------|
| 1 | Verify model retired | AI Engineering |
| 2 | Complete retirement documentation | AI Engineering |
| 3 | Export full record to archive | System/AI Engineering |
| 4 | Remove from active views | System/AI Engineering |
| 5 | Maintain searchable in archive | System |

---

## 13. Templates and Forms

### 13.1 New Model Registration Form
*[See Appendix A for complete form]*

### 13.2 Model Update Form
*[See Appendix B for complete form]*

### 13.3 Retirement Request Form
*[See Appendix C for complete form]*

---

## Appendix A: Model Inventory Entry Template

### Core Information
| Field | Value |
|-------|-------|
| Model ID | |
| Model Name | |
| Model Version | |
| Description | |
| AI Type | |
| Model Category | |
| Algorithm | |
| Risk Tier | |

### Business Context
| Field | Value |
|-------|-------|
| Business Unit | |
| Use Case Name | |
| Business Owner | |
| Business Owner Email | |

### Technical Information
| Field | Value |
|-------|-------|
| Model Developer | |
| Developer Email | |
| Platform | |
| Repository | |

### Status
| Field | Value |
|-------|-------|
| Status | |
| Current Gate | |
| Production Date | |

### Documentation
| Field | Value |
|-------|-------|
| Model Card Link | |
| Solution Design Link | |
| Monitoring Dashboard | |

---

## Appendix B: Model Inventory Update Log Template

| Date | Field Updated | Old Value | New Value | Updated By | Reason |
|------|---------------|-----------|-----------|------------|--------|
| | | | | | |

---

## Appendix C: Model Retirement Checklist

| Item | Completed | Date | Notes |
|------|-----------|------|-------|
| Downstream consumers notified | ☐ | | |
| Alternative solution confirmed | ☐ | | |
| Final performance snapshot captured | ☐ | | |
| Documentation archived | ☐ | | |
| Model artifacts archived | ☐ | | |
| Infrastructure decommissioned | ☐ | | |
| Status updated to Retired | ☐ | | |
| Retirement date recorded | ☐ | | |

---

## Document Control

### Related Documents
- AI, Automation & Intelligent Solutions Governance Operating Model (AI-GOV-001)
- AI, Automation & Intelligent Solutions Intake & Prioritization Framework (AI-GOV-002)
- AI & Automation Initiative Approval & Stage-Gate Process (AI-GOV-003)
- Compliance Traceability Matrix (AI-GOV-CTM)
- Model Documentation Standard (AI-ENG-001)
- Automation Documentation Standard (AI-ENG-002)

### Approval History

| Version | Date | Author | Approver | Changes |
|---------|------|--------|----------|---------|
| 1.0 | [Date] | [Author] | [Approver] | Initial release |
| 1.1 | [Date] | [Author] | [Approver] | Added Automation scope; Updated org structure |
