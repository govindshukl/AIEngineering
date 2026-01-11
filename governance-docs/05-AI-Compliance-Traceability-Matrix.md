# AI, Automation & Intelligent Solutions Compliance Traceability Matrix

**Document ID:** AI-GOV-CTM
**Version:** 1.1
**Classification:** Internal
**Owner:** Head of AI Engineering, Innovation & Digitization Department
**Last Review Date:** [Date]
**Next Review Date:** [Date + 12 months]

---

## 1. Executive Summary

### 1.1 Purpose
This Compliance Traceability Matrix maps Bank ABC's AI, Automation, and Intelligent Solutions governance documentation suite to applicable regulatory requirements and industry standards. It provides a comprehensive view of how each governance control addresses specific regulatory expectations, enabling efficient compliance demonstration and gap identification.

### 1.2 Scope
This matrix covers:
- SR 11-7 (Federal Reserve Model Risk Management Guidance)
- PRA SS1/23 (Bank of England Model Risk Management Principles)
- EU AI Act (High-Risk AI System Requirements)
- CBB (Central Bank of Bahrain) Technology Risk and Operational Resilience Requirements
- Basel Committee Principles for Operational Resilience
- GDPR/Data Protection Considerations for AI and Automation

### 1.3 Organizational Context
- **Owning Department:** Innovation & Digitization Department
- **Document Owner:** Head of AI Engineering
- **Scope:** AI, Automation (RPA/Workflow), and Hybrid initiatives

### 1.4 How to Use This Matrix
- **Regulatory Examinations:** Use to demonstrate compliance coverage
- **Gap Analysis:** Identify areas requiring additional documentation or controls
- **Document Reviews:** Ensure updates maintain regulatory alignment
- **Audit Preparation:** Map audit requests to relevant documentation

---

## 2. Regulatory Framework Overview

### 2.1 SR 11-7: Supervisory Guidance on Model Risk Management

| Aspect | Description | Applicability |
|--------|-------------|---------------|
| Issuing Authority | US Federal Reserve Board | Reference standard globally |
| Effective Date | April 2011 | Current |
| Scope | All models used for decision-making | All AI/ML models |
| Key Themes | Model development, validation, governance, documentation | Core framework |

**Key Requirements:**
1. Model development and implementation controls
2. Independent model validation
3. Model governance and oversight
4. Model inventory and documentation
5. Ongoing monitoring and outcomes analysis

### 2.2 PRA SS1/23: Model Risk Management Principles

| Aspect | Description | Applicability |
|--------|-------------|---------------|
| Issuing Authority | UK Prudential Regulation Authority | Reference standard |
| Effective Date | May 2024 (implementation) | Current |
| Scope | All models including AI/ML | All AI/ML models |
| Key Themes | Proportionality, board accountability, model risk framework | Enhanced framework |

**Key Principles:**
1. Model identification and model risk classification
2. Governance
3. Model development, implementation, and use
4. Independent model validation
5. Model risk mitigants
6. Data management

### 2.3 EU AI Act

| Aspect | Description | Applicability |
|--------|-------------|---------------|
| Issuing Authority | European Union | Reference for best practice |
| Effective Date | 2024-2026 (phased) | Emerging standard |
| Scope | AI systems by risk category | GenAI and high-risk AI |
| Key Themes | Risk-based classification, transparency, human oversight | GenAI and Agentic AI governance |

**Key Requirements for High-Risk AI:**
1. Risk management system
2. Data governance
3. Technical documentation
4. Record-keeping and traceability
5. Transparency and user information
6. Human oversight
7. Accuracy, robustness, and cybersecurity

### 2.4 CBB Requirements

| Aspect | Description | Applicability |
|--------|-------------|---------------|
| Issuing Authority | Central Bank of Bahrain | Primary regulator |
| Key Modules | HC Module, OM Module | Directly applicable |
| Key Themes | Technology risk, operational resilience, outsourcing | All AI/ML |

**Key Requirements:**
1. Technology risk management
2. Information security
3. Business continuity
4. Outsourcing and third-party management
5. Data governance

### 2.5 Basel Committee Principles

| Aspect | Description | Applicability |
|--------|-------------|---------------|
| Issuing Authority | Basel Committee on Banking Supervision | International standard |
| Key Documents | Principles for Operational Resilience, Sound Practices | Reference standard |
| Key Themes | Operational resilience, third-party risk | All AI/ML |

---

## 3. Master Traceability Matrix

### 3.1 SR 11-7 Mapping

| SR 11-7 Requirement | Bank ABC Document | Relevant Sections | Coverage |
|---------------------|-------------------|-------------------|----------|
| **Model Development** |
| Sound design and development practices | AI-GOV-003: Stage-Gate Process | Section 7 (Build Phase) | Full |
| | AI-ENG-001: Development Standards (Wave 3) | All | Full |
| Developmental evidence documented | AI-GOV-004: Model Inventory | Section 3.12 (Documentation Links) | Full |
| | AI-ENG-002: Model Card Template (Wave 3) | All | Full |
| Testing for intended use | AI-GOV-003: Stage-Gate Process | Section 8 (Gate 3: Validation) | Full |
| Clear statement of purpose | AI-GOV-002: Intake Framework | Section 3.2 (Use Case Definition) | Full |
| | AI-GOV-004: Model Inventory | Section 3.5 (Business Context) | Full |
| **Model Validation** |
| Independent review | AI-GOV-001: Operating Model | Section 4 (Three Lines Model) | Full |
| | AI-GOV-003: Stage-Gate Process | Section 8.3 (Validation Approach by Tier) | Full |
| Conceptual soundness | AI-GOV-003: Stage-Gate Process | Section 8.4 (Validation Scope) | Full |
| | AI-VAL-001: Validation Standards (Wave 4) | All | Full |
| Outcomes analysis | AI-GOV-003: Stage-Gate Process | Section 11 (Ongoing Operations) | Full |
| Process verification | AI-GOV-003: Stage-Gate Process | Section 8.4 (Implementation Verification) | Full |
| Ongoing monitoring | AI-GOV-003: Stage-Gate Process | Section 11.1 (Monitoring Requirements) | Full |
| | AI-MON-001: Monitoring Guide (Wave 3) | All | Full |
| **Model Governance** |
| Board/senior management oversight | AI-GOV-001: Operating Model | Section 2.1 (AI Steering Committee) | Full |
| Model risk management framework | AI-GOV-001: Operating Model | Section 3 (AI Risk Taxonomy and Tiering) | Full |
| Policies and procedures | AI-GOV-001, 002, 003, 004 | All Wave 1 documents | Full |
| Internal controls | AI-GOV-001: Operating Model | Section 4 (Three Lines Model) | Full |
| | AI-GOV-003: Stage-Gate Process | All | Full |
| Model inventory | AI-GOV-004: Model Inventory | All | Full |
| **Documentation** |
| Model documentation | AI-GOV-004: Model Inventory | Section 3.12 (Documentation Links) | Full |
| | AI-ENG-002: Model Card Template (Wave 3) | All | Full |
| Validation documentation | AI-GOV-003: Stage-Gate Process | Section 8.7 (Required Artifacts) | Full |
| | AI-VAL-001: Validation Standards (Wave 4) | All | Full |

### 3.2 PRA SS1/23 Mapping

| SS1/23 Principle | Bank ABC Document | Relevant Sections | Coverage |
|------------------|-------------------|-------------------|----------|
| **Principle 1: Model Identification and Risk Classification** |
| Model definition | AI-GOV-001: Operating Model | Section 1.3 (Scope) | Full |
| Model inventory | AI-GOV-004: Model Inventory | All | Full |
| Risk tiering | AI-GOV-001: Operating Model | Section 3.2 (Risk Tiering Framework) | Full |
| Materiality assessment | AI-GOV-004: Model Inventory | Section 3.2 (Materiality field) | Full |
| **Principle 2: Governance** |
| Board accountability | AI-GOV-001: Operating Model | Section 2.1 (AI Steering Committee) | Full |
| Clear ownership | AI-GOV-001: Operating Model | Section 2.2 (Roles and Responsibilities) | Full |
| | AI-GOV-004: Model Inventory | Section 3.6 (Ownership) | Full |
| Three lines of defense | AI-GOV-001: Operating Model | Section 4 (Three Lines Model) | Full |
| Model risk appetite | AI-GOV-001: Operating Model | Section 3 (Risk Taxonomy) | Partial |
| **Principle 3: Model Development, Implementation, and Use** |
| Development standards | AI-GOV-003: Stage-Gate Process | Sections 5-7 | Full |
| | AI-ENG-001: Development Standards (Wave 3) | All | Full |
| Implementation controls | AI-GOV-003: Stage-Gate Process | Section 9 (Gate 4) | Full |
| | AI-OPS-001: MLOps Runbook (Wave 3) | All | Full |
| Appropriate model use | AI-GOV-002: Intake Framework | Section 3.2 (Use Case Definition) | Full |
| | AI-GOV-004: Model Inventory | Section 3.5 (Business Context) | Full |
| **Principle 4: Independent Model Validation** |
| Independence | AI-GOV-001: Operating Model | Section 4.2 (Second Line) | Full |
| | AI-GOV-003: Stage-Gate Process | Section 8.3 (Validation by Tier) | Full |
| Validation scope | AI-GOV-003: Stage-Gate Process | Section 8.4 (Validation Scope) | Full |
| Findings management | AI-GOV-003: Stage-Gate Process | Section 8.8 (Findings Classification) | Full |
| **Principle 5: Model Risk Mitigants** |
| Monitoring | AI-GOV-003: Stage-Gate Process | Section 11 (Ongoing Operations) | Full |
| Performance tracking | AI-GOV-004: Model Inventory | Section 3.10 (Performance Fields) | Full |
| Trigger events | AI-GOV-003: Stage-Gate Process | Section 11.4 (Trigger Events) | Full |
| **Principle 6: Data Management** |
| Data quality | AI-GOV-002: Intake Framework | Section 3.6 (Data Requirements) | Full |
| | AI-GOV-004: Model Inventory | Section 3.8 (Data Fields) | Full |
| Data lineage | AI-GOV-004: Model Inventory | Section 3.8 (Data Lineage Link) | Full |

### 3.3 EU AI Act Mapping (High-Risk AI Requirements)

| EU AI Act Requirement | Bank ABC Document | Relevant Sections | Coverage |
|-----------------------|-------------------|-------------------|----------|
| **Article 9: Risk Management System** |
| Risk identification | AI-GOV-001: Operating Model | Section 3 (AI Risk Taxonomy) | Full |
| Risk assessment | AI-GOV-001: Operating Model | Section 3.2 (Risk Tiering) | Full |
| | AI-GOV-002: Intake Framework | Section 3.8 (Preliminary Risk Assessment) | Full |
| Risk mitigation | AI-GOV-001: Operating Model | Section 4 (Three Lines Model) | Full |
| Testing | AI-GOV-003: Stage-Gate Process | Section 8 (Gate 3: Validation) | Full |
| **Article 10: Data Governance** |
| Training data governance | AI-GOV-004: Model Inventory | Section 3.8 (Data Fields) | Full |
| | AI-DATA-001: Data Governance Addendum (Wave 3) | All | Full |
| Bias examination | AI-GOV-003: Stage-Gate Process | Section 8.4 (Fairness and Bias) | Full |
| Data quality | AI-GOV-002: Intake Framework | Section 3.6 (Data Requirements) | Full |
| **Article 11: Technical Documentation** |
| System description | AI-GOV-004: Model Inventory | Section 3 (Schema) | Full |
| Development documentation | AI-ENG-002: Model Card Template (Wave 3) | All | Full |
| Performance metrics | AI-GOV-004: Model Inventory | Section 3.10 (Performance Fields) | Full |
| **Article 12: Record-Keeping** |
| Logging | AI-GOV-004: Model Inventory | Section 3.14 (Audit Trail) | Full |
| Traceability | AI-GOV-004: Model Inventory | All | Full |
| **Article 13: Transparency** |
| User information | AI-GOV-001: Operating Model | Section 7 (GenAI Governance) | Partial |
| Instructions for use | AI-ENG-002: Model Card Template (Wave 3) | All | Full |
| **Article 14: Human Oversight** |
| Human oversight measures | AI-GOV-001: Operating Model | Section 8 (Agentic AI Governance) | Full |
| | AI-GOV-002: Intake Framework | Section 11 (Agentic AI Considerations) | Full |
| Intervention capability | AI-GOV-001: Operating Model | Section 7.3 (Human Oversight by Autonomy) | Full |
| **Article 15: Accuracy, Robustness, Cybersecurity** |
| Accuracy | AI-GOV-003: Stage-Gate Process | Section 8.4 (Performance Testing) | Full |
| Robustness | AI-GOV-003: Stage-Gate Process | Section 8.4 (Stress Testing) | Full |
| Cybersecurity | AI-GOV-003: Stage-Gate Process | Section 6.2 (Security Design) | Full |

### 3.4 EU AI Act Mapping (GenAI/Foundation Model Requirements)

| EU AI Act GenAI Requirement | Bank ABC Document | Relevant Sections | Coverage |
|-----------------------------|-------------------|-------------------|----------|
| **GPAI Model Obligations** |
| Technical documentation | AI-GOV-004: Model Inventory | Section 3.3 (GenAI-Specific Fields) | Full |
| Training data summary | AI-GOV-004: Model Inventory | Section 3.8 (Data Fields) | Full |
| Systemic risk assessment | AI-GOV-001: Operating Model | Section 3.1.7 (GenAI-Specific Risks) | Full |
| **Transparency (Deployers)** |
| AI-generated content marking | AI-GOV-001: Operating Model | Section 6.4 (Output Controls) | Partial |
| Human notification | AI-GOV-001: Operating Model | Section 6.4 (Output Controls) | Partial |

### 3.5 CBB Mapping

| CBB Requirement | Bank ABC Document | Relevant Sections | Coverage |
|-----------------|-------------------|-------------------|----------|
| **HC Module - Technology Risk** |
| Technology governance | AI-GOV-001: Operating Model | Section 2 (Governance Structure) | Full |
| Risk management | AI-GOV-001: Operating Model | Section 3 (AI Risk Taxonomy) | Full |
| Change management | AI-GOV-003: Stage-Gate Process | All | Full |
| **OM Module - Operational Risk** |
| Operational risk framework | AI-GOV-001: Operating Model | Section 3.1.4 (Operational Risk) | Full |
| Incident management | AI-GOV-001: Operating Model | Section 8 (Escalation) | Full |
| Business continuity | AI-GOV-003: Stage-Gate Process | Section 9.3 (Rollback Plan) | Partial |
| **Information Security** |
| Security controls | AI-GOV-003: Stage-Gate Process | Section 6.2 (Security Design) | Full |
| Access management | AI-GOV-004: Model Inventory | Section 10 (Access Control) | Full |
| Security testing | AI-GOV-003: Stage-Gate Process | Section 8.2 (Security Testing) | Full |
| **Third-Party/Outsourcing** |
| Vendor management | AI-GOV-002: Intake Framework | Section 1.3 (Scope - Third-party) | Partial |
| Third-party risk | AI-GOV-001: Operating Model | Section 3.1.7 (Foundation model dependency) | Partial |
| **Data Governance** |
| Data quality | AI-GOV-004: Model Inventory | Section 3.8 (Data Fields) | Full |
| Data protection | AI-GOV-004: Model Inventory | Section 3.8 (PII Involved) | Full |

### 3.6 Basel Committee Mapping

| Basel Principle | Bank ABC Document | Relevant Sections | Coverage |
|-----------------|-------------------|-------------------|----------|
| **Operational Resilience** |
| Critical operations | AI-GOV-001: Operating Model | Section 3.2 (Risk Tiering) | Full |
| Dependencies mapping | AI-GOV-004: Model Inventory | Section 3.13 (Dependencies) | Full |
| Testing | AI-GOV-003: Stage-Gate Process | Section 8 (Validation) | Full |
| **Third-Party Risk** |
| Concentration risk | AI-GOV-001: Operating Model | Section 3.1.7 (Foundation model dependency) | Partial |
| Service continuity | AI-GOV-003: Stage-Gate Process | Section 9.3 (Rollback) | Partial |

---

## 4. Document-to-Regulation Mapping

### 4.1 AI-GOV-001: AI/ML Governance Operating Model

| Section | SR 11-7 | SS1/23 | EU AI Act | CBB | Basel |
|---------|---------|--------|-----------|-----|-------|
| 1. Executive Summary | - | - | - | - | - |
| 2. Governance Structure | ✓ Governance | ✓ P2 | - | ✓ Tech Gov | - |
| 3. AI Risk Taxonomy and Tiering | ✓ Governance | ✓ P1, P2 | ✓ Art 9 | ✓ Risk Mgmt | ✓ Op Resilience |
| 4. Three Lines Model | ✓ Governance, Validation | ✓ P2, P4 | - | - | - |
| 5. Governance Touchpoints | ✓ Governance | ✓ P3 | - | ✓ Change Mgmt | - |
| 6. GenAI Governance | - | - | ✓ GPAI | - | - |
| 7. Agentic AI Governance | - | - | ✓ Art 14 | - | - |
| 8. Escalation Pathways | ✓ Governance | ✓ P2 | - | ✓ Incident Mgmt | - |
| 9. Reporting and Communication | ✓ Governance | ✓ P2 | - | - | - |
| 10. Integration with Existing Governance | ✓ Governance | ✓ P2 | - | - | - |

### 4.2 AI-GOV-002: AI Use Case Intake & Prioritization Framework

| Section | SR 11-7 | SS1/23 | EU AI Act | CBB | Basel |
|---------|---------|--------|-----------|-----|-------|
| 1. Executive Summary | - | - | - | - | - |
| 2. Intake Process Overview | ✓ Governance | ✓ P3 | - | ✓ Change Mgmt | - |
| 3. Use Case Request Form | ✓ Documentation | ✓ P1, P3 | ✓ Art 11 | - | - |
| 4. Initial Screening Criteria | ✓ Governance | ✓ P1 | ✓ Art 9 | - | - |
| 5. Full Assessment Process | ✓ Governance | ✓ P1, P3 | ✓ Art 9 | ✓ Risk Mgmt | - |
| 6. Prioritization Scoring Model | ✓ Governance | ✓ P1 | - | - | - |
| 7. Fast-Track Process | ✓ Governance | ✓ P1 | - | - | - |
| 8. Decision Outcomes | ✓ Governance | ✓ P2 | - | - | - |
| 10. GenAI-Specific Intake | - | - | ✓ GPAI | - | - |
| 11. Agentic AI-Specific Intake | - | - | ✓ Art 14 | - | - |

### 4.3 AI-GOV-003: AI Initiative Approval & Stage-Gate Process

| Section | SR 11-7 | SS1/23 | EU AI Act | CBB | Basel |
|---------|---------|--------|-----------|-----|-------|
| 1-2. Overview | ✓ Governance | ✓ P3 | - | ✓ Change Mgmt | - |
| 3. Governance by Risk Tier | ✓ Governance | ✓ P1 | - | - | - |
| 4. Gate 0: Intake | ✓ Governance | ✓ P1 | - | - | - |
| 5. Gate 1: Feasibility | ✓ Development | ✓ P3 | ✓ Art 9 | - | - |
| 6. Gate 2: Design | ✓ Development | ✓ P3 | ✓ Art 11 | ✓ Change Mgmt | - |
| 7. Build Phase | ✓ Development | ✓ P3 | ✓ Art 10 | - | - |
| 8. Gate 3: Validation | ✓ Validation | ✓ P4 | ✓ Art 9, 15 | - | ✓ Testing |
| 9. Gate 4: Production | ✓ Governance | ✓ P3 | - | ✓ Change Mgmt | - |
| 10. Gate 5: PIR | ✓ Monitoring | ✓ P5 | - | - | - |
| 11. Ongoing Operations | ✓ Monitoring | ✓ P5 | - | - | ✓ Op Resilience |
| 12. Model Retirement | ✓ Governance | ✓ P1 | - | - | - |
| 13. Exception Handling | ✓ Governance | ✓ P2 | - | - | - |

### 4.4 AI-GOV-004: AI/ML Model Inventory Register

| Section | SR 11-7 | SS1/23 | EU AI Act | CBB | Basel |
|---------|---------|--------|-----------|-----|-------|
| 1-2. Overview and Governance | ✓ Inventory | ✓ P1 | ✓ Art 12 | - | - |
| 3.1-3.2 Core and Classification | ✓ Inventory | ✓ P1 | ✓ Art 11 | - | - |
| 3.3 GenAI-Specific Fields | - | - | ✓ GPAI | - | - |
| 3.4 Agentic AI-Specific Fields | - | - | ✓ Art 14 | - | - |
| 3.5-3.6 Business and Ownership | ✓ Inventory | ✓ P2 | - | - | - |
| 3.7 Lifecycle Status | ✓ Inventory | ✓ P1 | - | - | - |
| 3.8 Data Fields | ✓ Documentation | ✓ P6 | ✓ Art 10 | ✓ Data Gov | - |
| 3.9 Technical Infrastructure | ✓ Documentation | ✓ P3 | ✓ Art 11 | - | - |
| 3.10 Performance and Monitoring | ✓ Monitoring | ✓ P5 | ✓ Art 15 | - | - |
| 3.11 Validation and Compliance | ✓ Validation | ✓ P4 | - | - | - |
| 3.13 Dependencies | ✓ Documentation | ✓ P3 | - | - | ✓ Dependencies |
| 3.14 Audit Trail | ✓ Documentation | - | ✓ Art 12 | - | - |
| 10. Access Control | ✓ Governance | ✓ P2 | - | ✓ Info Sec | - |

---

## 5. Gap Analysis

### 5.1 Identified Gaps (Wave 1 Documents)

| Gap ID | Regulation | Requirement | Current Coverage | Recommended Action | Priority |
|--------|------------|-------------|------------------|-------------------|----------|
| GAP-001 | EU AI Act | AI-generated content marking | Partial | Enhance GenAI governance section with explicit output labeling requirements | Medium |
| GAP-002 | CBB | Business continuity for AI | Partial | Add AI-specific BCP requirements to Wave 3 documents | Medium |
| GAP-003 | CBB | Third-party AI vendor management | Partial | Develop AI vendor assessment framework | High |
| GAP-004 | SS1/23 | Model risk appetite statement | Partial | Formalize AI risk appetite in Operating Model | High |
| GAP-005 | Basel | Concentration risk (foundation models) | Partial | Add foundation model dependency management | Medium |

### 5.2 Gap Closure Roadmap

| Gap ID | Target Document | Target Wave | Owner | Status |
|--------|-----------------|-------------|-------|--------|
| GAP-001 | AI-GOV-001 Update | Wave 2 | AI Engineering | Planned |
| GAP-002 | AI-OPS-001 MLOps Runbook | Wave 3 | AI Engineering | Planned |
| GAP-003 | New: AI Vendor Standards | Wave 2 | AI Engineering + Procurement | Planned |
| GAP-004 | AI-GOV-001 Update | Wave 2 | AI Engineering + Risk | Planned |
| GAP-005 | AI-GOV-001 Update | Wave 2 | AI Engineering | Planned |

---

## 6. Regulatory Change Management

### 6.1 Regulatory Monitoring Process

| Activity | Frequency | Owner | Output |
|----------|-----------|-------|--------|
| Regulatory horizon scanning | Monthly | Compliance | Regulatory update report |
| Impact assessment | As needed | AI Engineering + Compliance | Impact assessment memo |
| Gap analysis update | Quarterly | AI Engineering | Updated CTM |
| Document updates | As needed | AI Engineering | Revised documents |

### 6.2 Key Regulatory Developments to Monitor

| Regulation | Development | Expected Timeline | Potential Impact |
|------------|-------------|-------------------|------------------|
| EU AI Act | Implementation guidance | 2024-2026 | High - GenAI requirements |
| CBB | AI-specific guidance | TBD | High - Primary regulator |
| Basel | AI/ML principles | TBD | Medium - International standards |
| PRA SS1/23 | Full implementation | May 2024 | Medium - Reference standard |

---

## 7. Audit and Examination Support

### 7.1 Common Examination Requests Mapping

| Examination Request | Relevant Documents | Key Sections |
|--------------------|-------------------|--------------|
| Model inventory | AI-GOV-004 | All |
| Model governance framework | AI-GOV-001 | Sections 2, 3, 4 |
| Validation reports | AI-GOV-003 | Section 8 |
| Model documentation | AI-GOV-004 | Section 3.12 |
| Risk tiering methodology | AI-GOV-001 | Section 3.2 |
| Change management | AI-GOV-003 | All |
| Monitoring and performance | AI-GOV-003, AI-GOV-004 | Sections 11, 3.10 |
| Data governance | AI-GOV-004 | Section 3.8 |
| Third-party AI | AI-GOV-002 | Section 1.3 |

### 7.2 Examination Preparation Checklist

| Item | Document | Ready |
|------|----------|-------|
| Current model inventory | AI-GOV-004 | ☐ |
| Governance framework documentation | AI-GOV-001 | ☐ |
| Stage-gate evidence for recent deployments | AI-GOV-003 | ☐ |
| Validation reports for Tier 1 models | Per AI-GOV-003 | ☐ |
| Model cards for production models | Per AI-GOV-004 | ☐ |
| Monitoring dashboards and alerts | Per AI-GOV-003 | ☐ |
| Training records for AI governance | HR | ☐ |
| Risk committee minutes | Governance | ☐ |

---

## 8. Appendices

### Appendix A: Regulatory Reference Library

| Regulation | Full Title | Link/Reference |
|------------|-----------|----------------|
| SR 11-7 | Supervisory Guidance on Model Risk Management | Federal Reserve, April 2011 |
| SS1/23 | Model Risk Management Principles for Banks | PRA, May 2023 |
| EU AI Act | Regulation on Artificial Intelligence | EU 2024/... |
| CBB HC Module | High-Level Controls Module | CBB Rulebook |
| CBB OM Module | Operational Risk Management Module | CBB Rulebook |
| Basel PSMOR | Principles for Sound Management of Operational Risk | BCBS, 2011 |
| Basel POR | Principles for Operational Resilience | BCBS, 2021 |

### Appendix B: Glossary of Regulatory Terms

| Term | Definition | Source |
|------|------------|--------|
| Model | Quantitative method that processes input data to produce output | SR 11-7 |
| Model Risk | Potential for adverse consequences from decisions based on incorrect model outputs | SR 11-7 |
| High-Risk AI | AI systems with significant potential impact on health, safety, fundamental rights | EU AI Act |
| GPAI | General-Purpose Artificial Intelligence | EU AI Act |
| Three Lines Model | Governance model with first line (business), second line (risk), third line (audit) | IIA |

### Appendix C: Version History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | [Date] | Initial release | [Author] |

---

## Document Control

### Related Documents
- AI, Automation & Intelligent Solutions Governance Operating Model (AI-GOV-001)
- AI, Automation & Intelligent Solutions Intake & Prioritization Framework (AI-GOV-002)
- AI & Automation Initiative Approval & Stage-Gate Process (AI-GOV-003)
- AI, Automation & Intelligent Solutions Inventory Register (AI-GOV-004)

### Approval History

| Version | Date | Author | Approver | Changes |
|---------|------|--------|----------|---------|
| 1.0 | [Date] | [Author] | [Approver] | Initial release |
| 1.1 | [Date] | [Author] | [Approver] | Updated document names; Added Automation scope context |
