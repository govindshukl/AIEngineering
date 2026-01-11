# AI, Automation & Intelligent Solutions Use Case Intake & Prioritization Framework

**Document ID:** AI-GOV-002
**Version:** 1.1
**Classification:** Internal
**Owner:** Head of AI Engineering, Innovation & Digitization Department
**Last Review Date:** [Date]
**Next Review Date:** [Date + 12 months]

---

## 1. Executive Summary

### 1.1 Purpose
This framework establishes the standardized process for submitting, evaluating, and prioritizing AI, Automation, and Intelligent Solutions initiatives at Bank ABC. It serves as the "front door" for all AI and Automation requests, ensuring consistent assessment, appropriate resource allocation, and alignment with strategic objectives.

### 1.2 Objectives
- Provide a structured intake process for AI, Automation, and Hybrid use case requests
- Enable consistent evaluation and prioritization across all submissions
- Ensure appropriate risk assessment occurs early in the lifecycle
- Optimize resource allocation across competing initiatives
- Maintain transparency and clear communication with stakeholders
- Support high volume (30+ use cases annually) with streamlined processes
- Coordinate effectively with IT Department for data access requirements

### 1.3 Scope
This framework applies to:
- **AI/ML Requests:** Analytical AI, GenAI, Agentic AI
- **Automation Requests:** RPA, Workflow Automation, Business Process Automation
- **Hybrid Requests:** Combined AI + Automation solutions
- Enhancement requests for existing AI or Automation capabilities
- Third-party AI/Automation solution evaluations
- Proof of Concept (PoC) and pilot requests
- Microsoft Power Platform and Copilot initiatives

### 1.4 Organizational Context
- **Owning Department:** Innovation & Digitization Department
- **Primary Decision Maker:** Head of AI Engineering
- **Data Coordination:** IT Department (Data Management)

---

## 2. Intake Process Overview

### 2.1 Process Flow Diagram

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   SUBMISSION    │───▶│   SCREENING     │───▶│   ASSESSMENT    │───▶│   DECISION      │
│                 │    │                 │    │                 │    │                 │
│ Business submits│    │ AI Eng initial  │    │ Full evaluation │    │ Approve/Defer/  │
│ intake form     │    │ review          │    │ and scoring     │    │ Reject          │
│                 │    │                 │    │                 │    │                 │
│ SLA: Immediate  │    │ SLA: 2 days     │    │ SLA: 5 days     │    │ SLA: 3 days     │
└─────────────────┘    └─────────────────┘    └─────────────────┘    └─────────────────┘
        │                      │                      │                      │
        │                      ▼                      ▼                      ▼
        │               ┌─────────────┐        ┌─────────────┐        ┌─────────────┐
        │               │ Incomplete? │        │ More info   │        │ Approved    │
        │               │ Return to   │        │ required?   │        │ ──▶ Gate 1  │
        │               │ submitter   │        │ Request     │        │             │
        │               └─────────────┘        └─────────────┘        │ Deferred    │
        │                                                             │ ──▶ Backlog │
        │                                                             │             │
        │                                                             │ Rejected    │
        │                                                             │ ──▶ Archive │
        └─────────────────────────────────────────────────────────────┴─────────────┘
```

### 2.2 Process Participants

| Role | Department | Responsibilities in Intake Process |
|------|------------|-----------------------------------|
| Business Requestor | Business Units | Submits intake form, provides clarifications, attends assessment |
| Business Sponsor | Business Units | Validates business case, confirms resource commitment |
| Head of AI Engineering | Innovation & Digitization | Initial screening, assessment coordination, final decision (Tier 2/3) |
| Digital Product Owner | Innovation & Digitization | Requirements clarification, prioritization input |
| Data Scientist | Innovation & Digitization | Technical feasibility assessment (AI) |
| Business Analyst | Innovation & Digitization | Process analysis, requirements refinement, Automation feasibility |
| IT Data Management | IT Department | Data availability and quality assessment |
| Risk/Compliance Rep | Risk/Compliance | Regulatory and compliance assessment |
| AI & Automation Steering Committee | Cross-functional | Final decision for Tier 1 use cases |

### 2.3 Service Level Agreements

| Stage | SLA | Escalation if Breached |
|-------|-----|------------------------|
| Initial Screening | 2 business days | AI Engineering Lead |
| Information Request Response | 5 business days | Business Sponsor |
| Full Assessment | 5 business days from complete submission | AI Engineering Lead |
| Decision Communication | 3 business days from assessment | AI Engineering Lead |
| **Total (Submission to Decision)** | **10 business days** | AI Steering Committee |

---

## 3. Use Case Request Form

### 3.1 Requestor Information

| Field | Description | Required |
|-------|-------------|----------|
| Requestor Name | Person submitting the request | Yes |
| Requestor Role/Title | Job title | Yes |
| Business Unit | Department/Division | Yes |
| Contact Email | Primary contact | Yes |
| Contact Phone | For urgent communications | Yes |
| Business Sponsor | Executive sponsor for the initiative | Yes |
| Submission Date | Auto-populated | Yes |

### 3.2 Use Case Definition

| Field | Description | Required |
|-------|-------------|----------|
| Use Case Name | Descriptive name for the initiative | Yes |
| Problem Statement | Clear description of the business problem being addressed (2-3 paragraphs) | Yes |
| Current State | How is this problem handled today? What are the pain points? | Yes |
| Proposed AI/ML Solution | High-level description of the proposed AI approach (if known) | No |
| Expected Outcomes | Specific, measurable outcomes expected | Yes |
| Success Metrics | How will success be measured? (KPIs) | Yes |
| Target Users | Who will use or be affected by this solution? | Yes |
| Customer Impact | Does this directly or indirectly affect customers? How? | Yes |

### 3.3 Initiative Type Classification

| Field | Options | Required |
|-------|---------|----------|
| **Initiative Category** | AI / Automation / Hybrid | Yes |
| Primary AI Type (if AI/Hybrid) | Analytical AI / GenAI / Agentic AI | Conditional |
| Primary Automation Type (if Automation/Hybrid) | RPA / Workflow Automation / Business Process Automation | Conditional |
| Sub-Type (if known) | Classification, Regression, NLP, Computer Vision, LLM, RAG, Agent, Bot, Flow, etc. | No |
| Autonomy Level (for Agentic/Unattended) | L1-Assisted / L2-Supervised / L3-Monitored / L4-Autonomous | Conditional |
| Customer-Facing | Yes / No | Yes |
| Decision/Action Automation | Full Auto / Human-Assisted / Recommendation Only | Yes |

### 3.3.1 Automation-Specific Classification (if Automation or Hybrid)

| Field | Options | Required |
|-------|---------|----------|
| Automation Platform | Power Automate / UiPath / Custom / Other | Yes (if Automation) |
| Attended/Unattended | Attended / Unattended / Hybrid | Yes (if RPA) |
| Process Complexity | Simple (Linear) / Medium (Branching) / Complex (Multi-system) | Yes (if Automation) |
| Transaction Volume | Low (<100/day) / Medium (100-1000/day) / High (>1000/day) | Yes (if Automation) |

### 3.4 GenAI-Specific Information (if applicable)

| Field | Description | Required |
|-------|-------------|----------|
| Foundation Model Preference | Specific model requirements or preferences | No |
| Prompt Engineering Scope | Estimated complexity of prompt engineering required | No |
| RAG Requirements | Will retrieval-augmented generation be needed? | Yes (if GenAI) |
| Content Generation Type | Text, Code, Image, Multi-modal | Yes (if GenAI) |
| Output Control Requirements | Filtering, guardrails, human review needs | Yes (if GenAI) |

### 3.5 Agentic AI-Specific Information (if applicable)

| Field | Description | Required |
|-------|-------------|----------|
| Agent Scope | What actions can the agent take? | Yes (if Agentic) |
| Tool/API Access | What systems/APIs will the agent interact with? | Yes (if Agentic) |
| Action Boundaries | What limits on autonomous actions? | Yes (if Agentic) |
| Human Oversight Model | When/how will humans intervene? | Yes (if Agentic) |
| Platform Preference | MS Copilot / Power Automate / MS Foundry / Custom | No |

### 3.6 Data Requirements

| Field | Description | Required |
|-------|-------------|----------|
| Data Sources | List known data sources required | Yes |
| Data Availability | Available / Partially Available / Not Available / Unknown | Yes |
| Data Volume | Estimated data volume | No |
| PII Involvement | Does the use case involve PII or sensitive data? | Yes |
| Data Quality Assessment | Known data quality issues or concerns | No |
| External/Alternative Data | Is third-party or alternative data required? | Yes |
| Cross-Border Data | Will data cross jurisdictional boundaries? | Yes |

### 3.7 Business Case

| Field | Description | Required |
|-------|-------------|----------|
| Strategic Alignment | Which strategic objectives does this support? | Yes |
| Estimated Benefits | Quantified benefits (revenue, cost savings, efficiency) | Yes |
| Benefit Realization Timeline | When will benefits materialize? | Yes |
| Investment Request | Estimated investment required (if known) | No |
| Ongoing Operational Cost | Estimated annual run cost | No |
| Dependencies | Other projects or initiatives this depends on | No |

### 3.8 Preliminary Risk Assessment

| Risk Factor | Low | Medium | High | Unknown |
|-------------|-----|--------|------|---------|
| Financial Impact | ☐ | ☐ | ☐ | ☐ |
| Regulatory Sensitivity | ☐ | ☐ | ☐ | ☐ |
| Customer Impact | ☐ | ☐ | ☐ | ☐ |
| Data Sensitivity | ☐ | ☐ | ☐ | ☐ |
| Reputational Risk | ☐ | ☐ | ☐ | ☐ |
| Technical Complexity | ☐ | ☐ | ☐ | ☐ |

### 3.9 Timeline and Resources

| Field | Description | Required |
|-------|-------------|----------|
| Desired Go-Live Date | Target production date | No |
| Business Driver for Timeline | Why this timeline? (regulatory, competitive, etc.) | Conditional |
| Business Resources Available | Business SMEs, testing support, etc. | Yes |
| Constraints | Known constraints or blockers | No |

---

## 4. Initial Screening Criteria

### 4.1 Screening Checklist

The AI Engineering team evaluates each submission against the following criteria:

| Criterion | Pass | Fail | Action if Fail |
|-----------|------|------|----------------|
| Form completeness | All required fields populated | Missing required fields | Return for completion |
| Problem clarity | Problem statement is clear and specific | Vague or unclear problem | Request clarification |
| AI appropriateness | AI/ML is appropriate solution for the problem | Non-AI solution more suitable | Redirect to appropriate team |
| Strategic alignment | Aligns with one or more strategic objectives | No strategic alignment | Reject or request justification |
| Sponsor validation | Executive sponsor confirmed | No sponsor | Return to identify sponsor |
| Feasibility indication | Initial data and technical feasibility plausible | Clearly infeasible | Reject with explanation |
| Duplicate check | Not duplicate of existing initiative | Duplicate exists | Merge or redirect |

### 4.2 Screening Outcomes

| Outcome | Criteria | Next Step |
|---------|----------|-----------|
| **Proceed to Assessment** | All screening criteria pass | Schedule full assessment |
| **Request More Information** | Minor gaps or clarifications needed | Return to requestor with specific questions |
| **Redirect** | Better suited for non-AI solution | Transfer to appropriate team |
| **Reject** | Fundamentally unsuitable or infeasible | Archive with explanation |

---

## 5. Full Assessment Process

### 5.1 Assessment Dimensions

#### 5.1.1 Strategic Value Assessment
- Alignment with Bank ABC strategic priorities
- Revenue generation or cost reduction potential
- Competitive advantage implications
- Customer experience improvement
- Operational efficiency gains

#### 5.1.2 Technical Feasibility Assessment
- Data availability and quality
- Technical complexity and approach viability
- Infrastructure and platform readiness
- Integration requirements
- Skill and resource availability

#### 5.1.3 Risk Assessment
- Preliminary risk tier classification
- Regulatory and compliance implications
- Data privacy and security considerations
- Ethical and fairness concerns
- Operational and reputational risks

#### 5.1.4 Implementation Assessment
- Resource requirements (AI Engineering, Data, Business)
- Timeline feasibility
- Dependencies and constraints
- Change management needs

### 5.2 Assessment Meeting

**Participants:**
- AI Engineering Lead (Chair)
- AI Solutions Architect
- Data Engineering Representative
- Risk/Compliance Representative
- Business Requestor
- Business Sponsor (for Tier 1/2)

**Agenda:**
1. Use case presentation by requestor (15 min)
2. Technical feasibility discussion (15 min)
3. Data assessment discussion (10 min)
4. Risk assessment discussion (10 min)
5. Clarifying questions (10 min)
6. Closed session: Scoring and recommendation (15 min)

---

## 6. Prioritization Scoring Model

### 6.1 Scoring Criteria and Weights

| Dimension | Weight | Criteria |
|-----------|--------|----------|
| **Strategic Value** | 30% | See 6.2 |
| **Business Impact** | 25% | See 6.3 |
| **Feasibility** | 25% | See 6.4 |
| **Risk-Adjusted Score** | 20% | See 6.5 |

### 6.2 Strategic Value Scoring (30%)

| Score | Criteria |
|-------|----------|
| 5 | Direct enabler of top strategic priority; Board/Executive mandate |
| 4 | Strong alignment with strategic objectives; significant competitive advantage |
| 3 | Moderate strategic alignment; supports departmental goals |
| 2 | Weak strategic alignment; tactical improvement |
| 1 | No clear strategic alignment; nice-to-have |

### 6.3 Business Impact Scoring (25%)

| Score | Criteria |
|-------|----------|
| 5 | >$[X]M annual benefit; transformational impact |
| 4 | $[Y]M-$[X]M annual benefit; significant impact |
| 3 | $[Z]K-$[Y]M annual benefit; moderate impact |
| 2 | <$[Z]K annual benefit; minor efficiency gain |
| 1 | Unquantified or negligible benefit |

### 6.4 Feasibility Scoring (25%)

| Score | Criteria |
|-------|----------|
| 5 | Data ready; proven approach; skills available; low complexity |
| 4 | Data mostly ready; established approach; minor skill gaps |
| 3 | Data requires preparation; moderate complexity; some uncertainty |
| 2 | Significant data gaps; high complexity; skill gaps; dependencies |
| 1 | Major feasibility concerns; experimental; high uncertainty |

### 6.5 Risk-Adjusted Score (20%)

| Risk Tier | Score Multiplier | Rationale |
|-----------|------------------|-----------|
| Tier 3 (Low Risk) | 1.0 | No adjustment |
| Tier 2 (Medium Risk) | 0.85 | Moderate governance overhead |
| Tier 1 (High Risk) | 0.70 | Significant governance and validation requirements |

### 6.6 Final Score Calculation

```
Final Score = (Strategic Value × 0.30) + (Business Impact × 0.25) + (Feasibility × 0.25) + (Risk-Adjusted Factor × 0.20 × Average of above three)
```

### 6.7 Prioritization Bands

| Band | Score Range | Recommendation |
|------|-------------|----------------|
| **Priority 1** | 4.0 - 5.0 | Immediate approval; allocate resources |
| **Priority 2** | 3.0 - 3.9 | Approve; schedule based on capacity |
| **Priority 3** | 2.0 - 2.9 | Conditional approval; may defer |
| **Priority 4** | < 2.0 | Defer or reject; revisit if circumstances change |

---

## 7. Fast-Track Process

### 7.1 Fast-Track Eligibility

Use cases may qualify for fast-track processing if ALL of the following criteria are met:

| Criterion | Requirement |
|-----------|-------------|
| Risk Tier | Tier 3 (Low Risk) |
| AI Type | Enhancement to existing model OR standard pattern |
| Investment | Below $[threshold] |
| Data | Uses existing, approved data sources |
| Timeline | Not urgent/regulatory driven |
| Complexity | Low technical complexity |

### 7.2 Fast-Track Process

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   SUBMISSION    │───▶│ FAST-TRACK      │───▶│   DECISION      │
│                 │    │ REVIEW          │    │                 │
│ Simplified form │    │ AI Eng Lead     │    │ Approve/Standard│
│                 │    │ review          │    │ track           │
│                 │    │                 │    │                 │
│ SLA: Immediate  │    │ SLA: 3 days     │    │ SLA: 1 day      │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

**Total SLA for Fast-Track: 5 business days**

### 7.3 Fast-Track Decision Authority
- AI Engineering Lead has sole approval authority for fast-track requests
- Any concerns trigger escalation to standard process

---

## 8. Decision Outcomes

### 8.1 Outcome Types

| Outcome | Definition | Next Steps |
|---------|------------|------------|
| **Approved** | Use case approved for progression to Gate 1 | Assign resources; schedule Discovery phase |
| **Approved with Conditions** | Approved subject to specific conditions | Document conditions; proceed when conditions met |
| **Deferred** | Valid use case but not prioritized currently | Add to backlog; revisit in [X] months |
| **Request More Information** | Cannot decide without additional information | Specific questions provided; resubmit within 10 days |
| **Rejected** | Use case not approved | Document rationale; archive; requestor may appeal |

### 8.2 Decision Communication

All decisions communicated within 3 business days including:
- Decision outcome
- Rationale for decision
- Priority band (if approved)
- Conditions (if applicable)
- Next steps and timeline
- Assigned AI Engineering point of contact (if approved)

### 8.3 Appeal Process

| Step | Action | Timeline |
|------|--------|----------|
| 1 | Requestor submits written appeal to AI Engineering Lead | Within 10 days of decision |
| 2 | AI Engineering Lead reviews with AI Solutions Architect | 5 business days |
| 3 | If not resolved, escalate to AI Steering Committee | Next scheduled meeting |
| 4 | AI Steering Committee decision is final | Communicated within 3 days |

---

## 9. Intake Review Cadence

### 9.1 Regular Review Meetings

| Meeting | Frequency | Purpose | Participants |
|---------|-----------|---------|--------------|
| Intake Triage | Twice weekly | Screen new submissions | AI Eng Lead, Solutions Architect |
| Assessment Sessions | Weekly | Full assessments (2-3 per session) | Assessment team + requestors |
| Priority Review | Monthly | Review backlog and reprioritize | AI Eng Lead, Business Sponsors |
| Portfolio Review | Monthly | Report to AI Steering Committee | AI Steering Committee |

### 9.2 Capacity Management

- AI Engineering maintains a capacity model updated monthly
- New approvals scheduled based on available capacity
- Priority 1 items may trigger reprioritization of existing work
- Quarterly capacity planning aligned with business planning cycles

---

## 10. GenAI-Specific Intake Considerations

### 10.1 Additional Evaluation Criteria for GenAI

| Criterion | Evaluation Questions |
|-----------|---------------------|
| Foundation Model Selection | Is a specific model required? Are approved models sufficient? |
| Prompt Sensitivity | How sensitive is the prompt content? System prompt exposure risk? |
| Output Risk | What is the risk of hallucination or incorrect output? |
| Content Type | Is content customer-facing? Regulatory implications? |
| Grounding Requirements | Is RAG or knowledge grounding required? Data source implications? |
| Human Review | What level of human review is appropriate? |

### 10.2 GenAI Risk Escalators

The following factors automatically increase risk tier for GenAI use cases:

| Factor | Tier Adjustment |
|--------|-----------------|
| Customer-facing content generation | Minimum Tier 2 |
| Financial or legal content | Minimum Tier 2 |
| Regulatory communications | Automatic Tier 1 |
| No human review before output | +1 Tier |
| External foundation model API (not Azure/Bedrock) | +1 Tier |

---

## 11. Agentic AI-Specific Intake Considerations

### 11.1 Additional Evaluation Criteria for Agentic AI

| Criterion | Evaluation Questions |
|-----------|---------------------|
| Autonomy Level | What level of autonomous action is requested? |
| Action Scope | What actions can the agent perform? |
| Boundary Definition | Are boundaries clearly defined and enforceable? |
| Reversibility | Can agent actions be reversed? |
| Tool Access | What tools/APIs will the agent access? |
| Multi-Agent | Does this involve multiple interacting agents? |
| Human Override | How quickly can humans intervene? |

### 11.2 Agentic AI Risk Escalators

| Factor | Tier Adjustment |
|--------|-----------------|
| Autonomy Level L3 (Monitored) | Minimum Tier 2 |
| Autonomy Level L4 (Autonomous) | Automatic Tier 1 |
| Financial transaction capability | Automatic Tier 1 |
| Customer data modification | Automatic Tier 1 |
| Multi-agent orchestration | +1 Tier |
| External system integration | +1 Tier (if not pre-approved) |

### 11.3 Microsoft Platform Intake Path

| Platform | Intake Path | Owning Team |
|----------|-------------|-------------|
| M365 Copilot (standard features) | Streamlined: IT enablement, not I&D intake | IT Department |
| M365 Copilot (custom plugins) | Standard intake | Innovation & Digitization |
| Power Automate (simple flows) | Fast-track eligible | Innovation & Digitization |
| Power Automate (AI-powered) | Standard intake | Innovation & Digitization |
| Copilot Studio (low-code agents) | Standard intake | Innovation & Digitization |
| MS Foundry (high-code agents) | Full intake, minimum Tier 2 | Innovation & Digitization |

---

## 12. Automation-Specific Intake Considerations

### 12.1 Additional Evaluation Criteria for Automation

| Criterion | Evaluation Questions |
|-----------|---------------------|
| Process Stability | Is the underlying process stable or undergoing changes? |
| Rule-Based Suitability | Is the process rule-based with clear logic? |
| Volume and Frequency | Is the volume sufficient to justify automation investment? |
| Exception Rate | What is the expected exception rate? Can exceptions be handled? |
| System Access | What systems need to be accessed? Are APIs available? |
| Current Manual Effort | How many FTEs/hours are currently spent on this process? |
| Data Sensitivity | Does the process handle sensitive data? |

### 12.2 Automation Risk Escalators

| Factor | Tier Adjustment |
|--------|-----------------|
| Unattended bot with financial transactions | Minimum Tier 2 |
| High-volume transaction processing (>1000/day) | Minimum Tier 2 |
| Modifies core banking records | Automatic Tier 1 |
| Customer-facing process | Minimum Tier 2 |
| Cross-system integration (>3 systems) | +1 Tier |
| No human review of exceptions | +1 Tier |

### 12.3 Hybrid (AI + Automation) Intake

For Hybrid initiatives:
- Complete BOTH AI and Automation sections of the intake form
- Risk tier = Higher of AI tier and Automation tier
- Feasibility assessment must cover both AI and Automation components
- May require coordination between Data Scientist (AI) and Business Analyst (Automation)

---

## 13. Metrics and Reporting

### 13.1 Intake Process Metrics

| Metric | Target | Measurement |
|--------|--------|-------------|
| Submission to Decision Time | <10 business days | Average days |
| Fast-Track Decision Time | <5 business days | Average days |
| Screening Pass Rate | >70% | % proceeding to assessment |
| Assessment Completion Rate | >90% | % completed within SLA |
| Approval Rate | Track only | % approved of assessed |
| Backlog Age | <90 days average | Average days deferred |

### 13.2 Monthly Reporting

Report to AI & Automation Steering Committee includes:
- Submissions received (by type: AI/Automation/Hybrid, by business unit)
- Decisions made (approved, deferred, rejected)
- Pipeline status (in assessment, awaiting resources)
- SLA performance
- Backlog status
- Capacity utilization (Innovation & Digitization team)
- IT Department coordination status (data requests pending/completed)

---

## 14. Templates and Artifacts

### 14.1 Document List

| Template | Purpose | Location |
|----------|---------|----------|
| AI/Automation Use Case Intake Form | Submission form | Appendix A |
| Prioritization Scoring Sheet | Assessment scoring | Appendix B |
| Decision Log Template | Record decisions | Appendix C |
| Fast-Track Request Form | Simplified intake | Appendix D |
| Automation Process Assessment Form | RPA/Workflow assessment | Appendix E |

---

## Appendix A: AI Use Case Intake Form Template

*[Full form template with all fields from Section 3]*

---

## Appendix B: Prioritization Scoring Sheet

| Use Case: | [Name] |
|-----------|--------|
| Submission Date: | [Date] |
| Assessed By: | [Names] |
| Assessment Date: | [Date] |

**Scoring:**

| Dimension | Score (1-5) | Weight | Weighted Score | Notes |
|-----------|-------------|--------|----------------|-------|
| Strategic Value | | 0.30 | | |
| Business Impact | | 0.25 | | |
| Feasibility | | 0.25 | | |
| **Subtotal** | | | | |
| Risk Tier | | | | |
| Risk Multiplier | | 0.20 | | |
| **Final Score** | | | | |

**Priority Band:** [ ]

**Recommendation:** [ ]

---

## Appendix C: Decision Log Template

| Field | Value |
|-------|-------|
| Use Case ID | |
| Use Case Name | |
| Requestor | |
| Business Unit | |
| Submission Date | |
| Decision Date | |
| Decision | Approved / Approved with Conditions / Deferred / Rejected |
| Priority Band | |
| Conditions (if applicable) | |
| Rationale | |
| Assigned Owner | |
| Target Gate 1 Date | |
| Decision Maker | |

---

## Appendix D: Fast-Track Request Form

*[Simplified version of intake form for eligible use cases]*

---

## Document Control

### Related Documents
- AI, Automation & Intelligent Solutions Governance Operating Model (AI-GOV-001)
- AI & Automation Initiative Approval & Stage-Gate Process (AI-GOV-003)
- AI, Automation & Intelligent Solutions Inventory Register (AI-GOV-004)
- Compliance Traceability Matrix (AI-GOV-CTM)

### Approval History

| Version | Date | Author | Approver | Changes |
|---------|------|--------|----------|---------|
| 1.0 | [Date] | [Author] | [Approver] | Initial release |
| 1.1 | [Date] | [Author] | [Approver] | Added Automation scope; Updated org structure; IT coordination |
