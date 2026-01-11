# Technology Selection & Decision Framework

**Document ID:** AI-ENG-003
**Version:** 1.0
**Classification:** Internal
**Owner:** Head of AI Engineering, Innovation & Digitization Department
**Last Review Date:** [Date]
**Next Review Date:** [Date + 12 months]

---

## 1. Executive Summary

### 1.1 Purpose
This document establishes the framework for selecting appropriate technologies for AI, Automation, and Intelligent Solutions initiatives at Bank ABC. It provides decision criteria, selection matrices, and guidance to ensure consistent, justified technology choices that align with the bank's strategic direction, approved technology stack, and governance requirements.

### 1.2 Objectives
- Provide clear guidance for selecting AI vs. Automation vs. Hybrid approaches
- Enable consistent platform and technology selection across initiatives
- Establish pre-approved technology patterns for common use cases
- Define criteria for foundation model selection
- Streamline technology decisions while maintaining appropriate governance
- Reduce decision latency through clear guidelines and pre-approved options

### 1.3 Scope
This framework covers:
- Initiative type decisions (AI, Automation, Hybrid)
- AI platform selection (Analytical AI, GenAI, Agentic AI)
- Foundation model selection
- Automation platform selection
- Vector database and supporting technology selection
- Pre-approved architecture patterns
- Exception process for non-standard technologies

### 1.4 Organizational Context
- **Owning Department:** Innovation & Digitization Department
- **Decision Authority:** Head of AI Engineering
- **Escalation:** AI & Automation Steering Committee (for non-standard requests)
- **IT Coordination:** IT Department (Infrastructure, Security, Data)

---

## 2. Initiative Type Decision Framework

### 2.1 AI vs. Automation vs. Hybrid Decision Tree

```
                                    ┌─────────────────────────────┐
                                    │   New Use Case Request      │
                                    └─────────────┬───────────────┘
                                                  │
                                                  ▼
                              ┌───────────────────────────────────────┐
                              │ Does the process require judgment,    │
                              │ pattern recognition, or learning      │
                              │ from data?                            │
                              └───────────────┬───────────────────────┘
                                              │
                        ┌─────────────────────┼─────────────────────┐
                        │ YES                 │                     │ NO
                        ▼                     │                     ▼
        ┌───────────────────────────┐         │     ┌───────────────────────────┐
        │ Is there sufficient       │         │     │ Is the process rule-based │
        │ quality data available?   │         │     │ and repetitive?           │
        └───────────┬───────────────┘         │     └───────────┬───────────────┘
                    │                         │                 │
              ┌─────┴─────┐                   │           ┌─────┴─────┐
              │ YES       │ NO               │           │ YES       │ NO
              ▼           ▼                   │           ▼           ▼
    ┌─────────────┐  ┌─────────────┐         │  ┌─────────────┐  ┌─────────────┐
    │ AI or       │  │ Consider    │         │  │ AUTOMATION  │  │ Manual      │
    │ HYBRID      │  │ GenAI/RAG   │         │  │             │  │ Process     │
    └──────┬──────┘  │ approach    │         │  └─────────────┘  │ Review      │
           │         └─────────────┘         │                   └─────────────┘
           ▼                                 │
    ┌───────────────────────────┐            │
    │ Does it also require      │            │
    │ rule-based processing or  │            │
    │ system integration?       │            │
    └───────────┬───────────────┘            │
                │                            │
          ┌─────┴─────┐                      │
          │ YES       │ NO                   │
          ▼           ▼                      │
    ┌─────────────┐  ┌─────────────┐         │
    │ HYBRID      │  │ AI          │         │
    │ (AI + Auto) │  │ Only        │         │
    └─────────────┘  └─────────────┘         │
```

### 2.2 When to Use AI

AI is appropriate when the use case exhibits these characteristics:

| Characteristic | Description | Examples |
|---------------|-------------|----------|
| **Pattern Recognition** | Identifying patterns in data that humans find difficult | Fraud detection, anomaly identification |
| **Prediction** | Forecasting future outcomes based on historical data | Churn prediction, credit scoring, demand forecasting |
| **Natural Language** | Understanding or generating human language | Document classification, chatbots, summarization |
| **Judgment at Scale** | Decisions requiring nuanced judgment across many cases | Loan approval recommendations, customer segmentation |
| **Learning from Data** | Improving performance based on outcomes | Personalization, recommendation systems |
| **Unstructured Data** | Processing images, text, audio, or video | Document extraction, image classification |

**Data Requirements for AI:**
- Sufficient volume of quality training data (varies by technique)
- Access to relevant features/attributes
- Labeled data for supervised learning
- Representative historical data

### 2.3 When to Use Automation

Automation is appropriate when the use case exhibits these characteristics:

| Characteristic | Description | Examples |
|---------------|-------------|----------|
| **Rule-Based Logic** | Clear, definable business rules | Data validation, compliance checks |
| **Repetitive Tasks** | Same steps executed many times | Report generation, data entry |
| **High Volume** | Large number of transactions | Bulk processing, reconciliation |
| **Multi-System** | Moving data between systems | System integration, data migration |
| **Structured Process** | Well-defined inputs, outputs, and steps | Form processing, account updates |
| **Time-Sensitive** | Needs to run on schedule or trigger | Overnight batch processing, alerts |

**Process Requirements for Automation:**
- Stable, well-documented process
- Clear exception handling rules
- Defined business rules
- Accessible system interfaces

### 2.4 When to Use Hybrid (AI + Automation)

Hybrid approaches combine AI capabilities with automation workflows:

| Pattern | Description | Example Use Cases |
|---------|-------------|-------------------|
| **AI-Augmented Automation** | AI provides decisions/extractions that feed into automated workflow | Document processing with intelligent extraction |
| **Automation-Orchestrated AI** | Automation orchestrates multiple AI model calls | Multi-step document analysis pipeline |
| **AI with Automated Actions** | AI recommendations trigger automated actions | Fraud detection with automated case creation |
| **Intelligent Process Automation** | End-to-end automation with embedded AI | Customer onboarding with ID verification |

### 2.5 Decision Matrix: AI vs. Automation vs. Hybrid

| Factor | AI | Automation | Hybrid |
|--------|-----|------------|--------|
| **Decision Complexity** | High (judgment required) | Low (rule-based) | Mixed |
| **Data Dependency** | High | Low | Medium-High |
| **Process Stability** | Can adapt | Requires stability | Partial adaptation |
| **Volume Requirements** | Varies | High volume beneficial | Varies |
| **Rule Clarity** | Fuzzy/learned rules | Clear rules | Combined |
| **Integration Needs** | API/batch | Multi-system UI/API | Combined |
| **Human Review** | Often recommended | Exception-based | Selective |
| **Time to Value** | Longer (training) | Faster | Medium |

---

## 3. AI Technology Selection

### 3.1 AI Type Selection

#### 3.1.1 Analytical AI Selection Criteria

Use Analytical AI (traditional ML) when:
- Problem is well-defined with clear target variable
- Sufficient structured training data is available
- Interpretability is important
- Prediction/classification/regression is the goal
- Real-time or batch scoring is needed

Common techniques:
- Classification (XGBoost, Random Forest, Logistic Regression)
- Regression (Linear/Ridge/Lasso, Gradient Boosting)
- Clustering (K-Means, DBSCAN)
- Time Series (ARIMA, Prophet, LSTM)

#### 3.1.2 GenAI Selection Criteria

Use GenAI when:
- Natural language understanding or generation is required
- Working with unstructured text, code, or documents
- Conversational interface is needed
- Summarization, extraction, or transformation of text
- Knowledge retrieval and synthesis (RAG)
- Creative content generation

**AI Fatema Consideration:** For internal GenAI use cases, evaluate AI Fatema platform first before custom development.

#### 3.1.3 Agentic AI Selection Criteria

Use Agentic AI when:
- Multi-step reasoning is required
- Task requires tool/function calling
- Autonomous or semi-autonomous operation needed
- Complex orchestration of multiple capabilities
- Goal-oriented behavior with planning required

**Governance Note:** Agentic AI requires minimum Tier 2 classification and appropriate autonomy level controls.

### 3.2 Analytical AI Platform Selection

#### 3.2.1 AWS SageMaker

**When to Use:**
- Primary platform for analytical AI model development
- Batch and real-time inference requirements
- Need for managed ML infrastructure
- Integration with AWS data ecosystem
- MLOps capabilities (experiment tracking, model registry)

**Capabilities:**
- SageMaker Studio for development
- Built-in algorithms and frameworks
- Managed training and hosting
- Auto-scaling endpoints
- Integration with MLflow

**Standard Use Cases:**
- Credit risk models
- Churn prediction
- Fraud detection
- Customer segmentation
- Demand forecasting

#### 3.2.2 Custom Development

**When to Use:**
- Specialized algorithms not available in SageMaker
- Edge deployment requirements
- Specific framework requirements
- Integration with non-AWS systems (with justification)

**Requirements:**
- Justification documented in ADR
- Head of AI Engineering approval
- IT coordination for infrastructure
- Alignment with development standards (AI-ENG-001)

### 3.3 GenAI Platform Selection

#### 3.3.1 AI Fatema Platform (Preferred for Internal GenAI)

**Platform Overview:**
- In-house GenAI platform built on Open WebUI framework
- Supports Azure OpenAI and AWS Bedrock models
- Managed by Head of AI Engineering with vendor support
- Roadmap includes ila Bank and Corporate Portal integration

**When to Use AI Fatema:**
- Internal employee-facing GenAI applications
- Document Q&A and knowledge retrieval
- Internal chat assistants
- Employee self-service GenAI features
- Rapid prototyping of GenAI use cases

**When to Build Custom (Instead of AI Fatema):**
- Customer-facing applications requiring deep integration
- Specialized requirements AI Fatema cannot meet
- Performance requirements beyond AI Fatema capabilities
- Requires approval and justification

**AI Fatema Capabilities:**
- Multi-model support (Azure OpenAI, Bedrock)
- Conversation management
- Document upload and processing
- RAG integration
- User management and access control
- Audit logging

#### 3.3.2 Azure OpenAI

**When to Use:**
- Enterprise-grade GenAI requirements
- Microsoft ecosystem integration
- Content filtering requirements
- Azure data residency alignment
- Integration with M365 Copilot ecosystem

**Available Models:**
| Model | Use Case | Context Window |
|-------|----------|----------------|
| GPT-4o | General purpose, multimodal | 128K |
| GPT-4-turbo | Complex reasoning | 128K |
| GPT-4 | Complex reasoning | 8K-32K |
| GPT-3.5-turbo | Cost-effective, simpler tasks | 16K |
| text-embedding-ada-002 | Embeddings for RAG | N/A |

**Best For:**
- AI Fatema backend
- Microsoft ecosystem integrations
- Content with strict filtering needs
- Azure-based infrastructure

#### 3.3.3 AWS Bedrock

**When to Use:**
- AWS ecosystem integration
- Multiple model provider access
- Bedrock Guardrails requirements
- Existing AWS infrastructure

**Available Models:**
| Model Family | Provider | Use Case |
|--------------|----------|----------|
| Claude (3.5, 3) | Anthropic | Complex reasoning, long context |
| Titan | Amazon | General purpose, embeddings |
| Llama 2/3 | Meta | Cost-effective, open weights |
| Mistral | Mistral AI | European data residency |

**Best For:**
- AWS-native applications
- Multi-model strategies
- Guardrail requirements
- SageMaker integration

#### 3.3.4 GenAI Platform Comparison Matrix

| Criteria | AI Fatema | Azure OpenAI | AWS Bedrock |
|----------|-----------|--------------|-------------|
| **Primary Use** | Internal GenAI apps | Enterprise GenAI | AWS-integrated GenAI |
| **Model Variety** | Via Azure/Bedrock | OpenAI models | Multiple providers |
| **Setup Effort** | Low (existing platform) | Medium | Medium |
| **Customization** | Platform features | High | High |
| **Cost Model** | Platform + API costs | Token-based | Token-based |
| **Best For** | Internal assistants | M365 integration | AWS workloads |
| **Governance** | Pre-approved (internal) | Standard intake | Standard intake |

### 3.4 Foundation Model Selection

#### 3.4.1 Model Selection Criteria

| Criterion | Considerations |
|-----------|---------------|
| **Task Requirements** | Reasoning depth, creativity, instruction following |
| **Context Window** | Document length, conversation history needs |
| **Latency** | Real-time vs. batch tolerance |
| **Cost** | Token pricing, expected volume |
| **Quality** | Output accuracy for specific task |
| **Safety** | Content filtering, guardrail needs |
| **Data Residency** | Geographic data processing requirements |

#### 3.4.2 Approved Foundation Models

**Tier 1: Production Approved**
| Model | Provider | Platform | Approved Use |
|-------|----------|----------|--------------|
| GPT-4o | OpenAI | Azure OpenAI | General production use |
| GPT-4-turbo | OpenAI | Azure OpenAI | Complex reasoning |
| GPT-3.5-turbo | OpenAI | Azure OpenAI | Cost-sensitive, simpler tasks |
| Claude 3.5 Sonnet | Anthropic | AWS Bedrock | Complex reasoning, long context |
| Claude 3 Haiku | Anthropic | AWS Bedrock | Fast, cost-effective |
| Titan Text | Amazon | AWS Bedrock | AWS-native applications |

**Tier 2: Approved with Conditions**
| Model | Provider | Platform | Conditions |
|-------|----------|----------|------------|
| Llama 3 | Meta | Bedrock | Non-customer-facing initially |
| Mistral | Mistral AI | Bedrock | EU data residency use cases |

**Tier 3: Future Consideration (Not Yet Approved)**
| Model | Status | Notes |
|-------|--------|-------|
| Self-hosted Llama | Under evaluation | Pending security review |
| Self-hosted Mistral | Under evaluation | Pending infrastructure setup |

#### 3.4.3 Model Selection Matrix by Use Case

| Use Case Type | Recommended Primary | Alternative | Rationale |
|--------------|---------------------|-------------|-----------|
| **Internal Chat Assistant** | GPT-4o (via AI Fatema) | Claude 3.5 Sonnet | Balance of capability and cost |
| **Document Q&A / RAG** | GPT-4o | Claude 3.5 Sonnet | Strong retrieval + reasoning |
| **Code Generation** | GPT-4o | Claude 3.5 Sonnet | Code understanding |
| **Summarization** | GPT-3.5-turbo | Claude 3 Haiku | Cost-effective for simpler task |
| **Customer-Facing Chat** | GPT-4o | GPT-4-turbo | Quality and safety critical |
| **Long Document Processing** | Claude 3.5 Sonnet | GPT-4-turbo | Extended context window |
| **High Volume / Cost Sensitive** | GPT-3.5-turbo | Claude 3 Haiku | Lower per-token cost |
| **Complex Reasoning** | GPT-4-turbo | Claude 3.5 Sonnet | Maximum capability |

### 3.5 Vector Database Selection

#### 3.5.1 Qdrant (Primary)

**When to Use:**
- Primary vector database for RAG implementations
- High-performance similarity search required
- Production GenAI applications
- Integration with AI Fatema

**Capabilities:**
- High-performance vector search
- Filtering capabilities
- Horizontal scaling
- Python and REST APIs
- Cloud and self-hosted options

**Configuration Standards:**
- Use cosine similarity for text embeddings
- Configure appropriate HNSW parameters
- Implement collection naming conventions
- Set up backup and recovery procedures

#### 3.5.2 pgvector (Alternative)

**When to Use:**
- Simple RAG implementations
- PostgreSQL already in architecture
- Lower vector volume (<1M vectors)
- Cost optimization priority

**Considerations:**
- Performance limitations at scale
- Requires PostgreSQL expertise
- Less specialized features than Qdrant

#### 3.5.3 Vector Database Selection Matrix

| Criteria | Qdrant | pgvector |
|----------|--------|----------|
| **Performance** | High | Medium |
| **Scale** | Millions+ vectors | <1M vectors |
| **Setup Complexity** | Medium | Low (if PG exists) |
| **Cost** | Moderate | Low |
| **Best For** | Production RAG | Simple RAG, prototypes |
| **AI Fatema Integration** | Primary | Not integrated |

### 3.6 Agentic AI Platform Selection

#### 3.6.1 Microsoft Copilot Studio

**When to Use:**
- Low-code agent development
- Microsoft ecosystem integration
- Simple to medium complexity agents
- Citizen developer scenarios (with governance)
- Customer service chatbots

**Capabilities:**
- Visual conversation designer
- Power Automate integration
- Built-in NLU
- Multi-channel deployment
- Analytics and insights

**Governance:**
- Standard intake process
- Minimum Tier 3
- I&D oversight required

#### 3.6.2 Microsoft Azure AI Foundry (MS Foundry)

**When to Use:**
- High-code, complex agent development
- Custom tool/function integration
- Advanced reasoning requirements
- Production enterprise agents
- Multi-agent orchestration

**Capabilities:**
- Full code control
- Custom tool development
- Advanced orchestration
- Enterprise security integration
- Comprehensive monitoring

**Governance:**
- Full intake process
- Minimum Tier 2
- Head of AI Engineering approval

#### 3.6.3 Custom Agent Development

**When to Use:**
- Unique requirements not met by platforms
- Specific framework requirements (LangChain, etc.)
- Maximum flexibility needed
- Integration with proprietary systems

**Requirements:**
- Strong justification in ADR
- Head of AI Engineering approval
- Comprehensive security review
- Full compliance with AI-ENG-001

#### 3.6.4 Agentic Platform Selection Matrix

| Criteria | Copilot Studio | MS Foundry | Custom |
|----------|---------------|------------|--------|
| **Complexity** | Low-Medium | High | Any |
| **Development Skill** | Low-code | High-code | High-code |
| **Time to Deploy** | Fast | Medium | Slow |
| **Customization** | Limited | High | Full |
| **Governance Intensity** | Standard | High | Highest |
| **Minimum Tier** | Tier 3 | Tier 2 | Tier 2 |
| **Best For** | Simple bots | Enterprise agents | Unique needs |

---

## 4. Automation Platform Selection

### 4.1 Automation Type Selection

| Automation Type | Characteristics | Platform Options |
|----------------|-----------------|------------------|
| **RPA (Robotic Process Automation)** | UI-based automation, legacy system access | Automation Anywhere, Power Automate Desktop |
| **Workflow Automation** | Business process flows, approvals, integrations | Power Automate Cloud |
| **Business Process Automation** | End-to-end process orchestration | Power Automate + Dataverse |
| **Conversational Automation** | Chat-based process initiation | Copilot Studio |

### 4.2 RPA Platform Selection

#### 4.2.1 Automation Anywhere

**When to Use:**
- Complex, enterprise-scale RPA
- Legacy system automation (mainframe, terminal)
- High-volume, mission-critical processes
- Advanced bot orchestration
- Existing Automation Anywhere investment

**Capabilities:**
- Task Bots and MetaBots
- Control Room for orchestration
- Credential Vault
- IQ Bot (intelligent document processing)
- Bot Insight analytics

**Best For:**
- Complex multi-application processes
- Mainframe/terminal automation
- High-volume batch processing
- Enterprise-scale deployments

#### 4.2.2 Power Automate Desktop

**When to Use:**
- Microsoft ecosystem integration
- Desktop automation needs
- Attended automation scenarios
- Integration with Power Automate Cloud
- Simpler RPA requirements

**Capabilities:**
- Desktop flow recording
- UI automation
- Integration with cloud flows
- Excel, browser automation
- Attended and unattended modes

**Best For:**
- Office automation
- Browser-based processes
- Attended user assistance
- Microsoft application integration

#### 4.2.3 RPA Platform Selection Matrix

| Criteria | Automation Anywhere | Power Automate Desktop |
|----------|--------------------|-----------------------|
| **Complexity Handling** | High | Medium |
| **Legacy System Support** | Excellent | Good |
| **Learning Curve** | Steeper | Moderate |
| **Microsoft Integration** | Good | Excellent |
| **Scalability** | Enterprise | Department/Enterprise |
| **Cost Model** | Bot-based licensing | User-based (M365) |
| **Best For** | Complex enterprise RPA | Office/browser automation |
| **Existing Investment** | Yes (approved vendor) | Yes (M365 included) |

#### 4.2.4 RPA Platform Decision Guide

```
Is the process primarily Microsoft Office/browser based?
├── YES → Does it require complex orchestration or high volume?
│         ├── YES → Consider Automation Anywhere
│         └── NO → Power Automate Desktop
│
└── NO → Does it involve legacy systems (mainframe, terminal)?
          ├── YES → Automation Anywhere
          └── NO → Does it require enterprise-scale orchestration?
                    ├── YES → Automation Anywhere
                    └── NO → Either platform (consider existing skills)
```

### 4.3 Workflow Automation Selection

#### 4.3.1 Power Automate Cloud

**When to Use:**
- Business process workflows
- Approval processes
- System integration via connectors
- Event-driven automation
- Microsoft 365 integration

**Capabilities:**
- 500+ pre-built connectors
- Approval workflows
- Scheduled and triggered flows
- AI Builder integration
- Business process flows

**Connector Categories:**
| Category | Examples | Governance |
|----------|----------|------------|
| Standard | SharePoint, Outlook, Teams | Freely available |
| Premium | SQL Server, HTTP, Dataverse | Requires premium license |
| Custom | Bank systems, APIs | Requires security review |
| On-premises | On-prem SQL, file systems | Requires gateway setup |

### 4.4 Conversational/Agent Selection

#### 4.4.1 Copilot Studio

**When to Use:**
- Customer service chatbots
- Employee self-service bots
- FAQ and knowledge base bots
- Simple task automation via chat
- Teams-integrated assistants

**Integration Options:**
- Power Automate for backend processes
- Dataverse for data storage
- Custom connectors for bank systems
- Azure services for advanced AI

**Governance:**
- I&D oversight required
- Standard intake process
- Follow Copilot Studio standards (AI-ENG-002)

---

## 5. Use Case Profile Matching

### 5.1 Use Case Profiling

When a new use case is submitted, profile it across these dimensions:

| Dimension | Options | Impact on Selection |
|-----------|---------|---------------------|
| **Initiative Type** | AI / Automation / Hybrid | Primary technology category |
| **Complexity** | Low / Medium / High | Platform sophistication |
| **Volume** | Low / Medium / High | Scalability requirements |
| **Latency** | Real-time / Near-real-time / Batch | Architecture pattern |
| **Integration** | None / Simple / Complex | Platform capabilities |
| **User Type** | Internal / External | Security, quality requirements |
| **Data Type** | Structured / Unstructured / Mixed | Technology type |

### 5.2 Technology Matching Matrix

| Use Case Profile | Recommended Stack | Notes |
|-----------------|-------------------|-------|
| **Internal employee assistant (GenAI)** | AI Fatema | Preferred platform for internal GenAI |
| **Document Q&A for employees** | AI Fatema + Qdrant RAG | Use existing AI Fatema RAG capabilities |
| **Customer-facing chatbot (simple)** | Copilot Studio | Low-code, quick deployment |
| **Customer-facing chatbot (complex)** | MS Foundry or Custom GenAI | Full control, enterprise features |
| **Credit risk scoring** | SageMaker + XGBoost/LightGBM | Traditional ML, interpretability |
| **Fraud detection** | SageMaker + ensemble models | Real-time scoring capability |
| **Document extraction + processing** | GenAI (extraction) + Power Automate (workflow) | Hybrid pattern |
| **High-volume data entry** | Automation Anywhere | Enterprise RPA |
| **Office process automation** | Power Automate Desktop + Cloud | Microsoft ecosystem |
| **Invoice processing** | AI (extraction) + Automation (workflow) | Hybrid IDP |
| **Report generation (rule-based)** | Power Automate | Workflow automation |
| **Predictive maintenance** | SageMaker + time series models | Analytical AI |
| **Customer segmentation** | SageMaker + clustering | Analytical AI |
| **Sentiment analysis** | Azure OpenAI / Bedrock | GenAI NLP |
| **Multi-step autonomous task** | MS Foundry | Agentic AI, Tier 2+ |

### 5.3 Pre-Approved Architecture Patterns

#### Pattern 1: Internal GenAI Assistant
```
┌─────────────┐     ┌─────────────┐     ┌─────────────────┐
│   User      │────▶│  AI Fatema  │────▶│  Azure OpenAI   │
│ (Employee)  │◀────│  (Open WebUI)│◀────│  or Bedrock     │
└─────────────┘     └──────┬──────┘     └─────────────────┘
                           │
                    ┌──────▼──────┐
                    │   Qdrant    │
                    │ (if RAG)    │
                    └─────────────┘
```
**Governance:** Tier 3 (standard internal use)

#### Pattern 2: RAG-Enabled Document Q&A
```
┌─────────────┐     ┌─────────────┐     ┌─────────────────┐
│  Documents  │────▶│  Embedding  │────▶│     Qdrant      │
│             │     │   Model     │     │  Vector Store   │
└─────────────┘     └─────────────┘     └────────┬────────┘
                                                 │
┌─────────────┐     ┌─────────────┐     ┌────────▼────────┐
│   User      │────▶│  AI Fatema  │────▶│   LLM (GPT-4o)  │
│   Query     │◀────│             │◀────│   + Context     │
└─────────────┘     └─────────────┘     └─────────────────┘
```
**Governance:** Tier 2-3 depending on data sensitivity

#### Pattern 3: Analytical AI Model Serving
```
┌─────────────┐     ┌─────────────┐     ┌─────────────────┐
│   Data      │────▶│  SageMaker  │────▶│    SageMaker    │
│   Sources   │     │  Processing │     │    Training     │
└─────────────┘     └─────────────┘     └────────┬────────┘
                                                 │
┌─────────────┐     ┌─────────────┐     ┌────────▼────────┐
│ Application │────▶│  SageMaker  │◀────│    MLflow       │
│   (API)     │◀────│  Endpoint   │     │    Registry     │
└─────────────┘     └─────────────┘     └─────────────────┘
```
**Governance:** Tier 1-3 based on risk assessment

#### Pattern 4: Hybrid Document Processing
```
┌─────────────┐     ┌─────────────┐     ┌─────────────────┐
│  Document   │────▶│  GenAI      │────▶│   Extracted     │
│   Input     │     │  Extraction │     │   Data          │
└─────────────┘     └─────────────┘     └────────┬────────┘
                                                 │
┌─────────────┐     ┌─────────────┐     ┌────────▼────────┐
│  Output /   │◀────│  Power      │◀────│   Validation    │
│  System     │     │  Automate   │     │   Rules         │
└─────────────┘     └─────────────┘     └─────────────────┘
```
**Governance:** Tier 2-3 based on data sensitivity

#### Pattern 5: Enterprise RPA
```
┌─────────────┐     ┌─────────────────────┐     ┌─────────────┐
│  Schedule   │────▶│  Automation         │────▶│  Target     │
│  or Trigger │     │  Anywhere           │     │  Systems    │
└─────────────┘     │  Control Room       │     └─────────────┘
                    └──────────┬──────────┘
                               │
                    ┌──────────▼──────────┐
                    │    Task Bots        │
                    │  (Attended/         │
                    │   Unattended)       │
                    └─────────────────────┘
```
**Governance:** Tier 2-3 based on process criticality

### 5.4 Quick Selection Guide by Initiative Type

#### For AI Initiatives:
```
1. Is it Natural Language / Text / Conversational?
   → GenAI (consider AI Fatema first)

2. Is it Prediction / Classification / Scoring?
   → Analytical AI (SageMaker)

3. Does it require autonomous multi-step actions?
   → Agentic AI (MS Foundry or Copilot Studio)
```

#### For Automation Initiatives:
```
1. Is it Microsoft Office / Browser based?
   → Power Automate Desktop

2. Is it workflow / approvals / integrations?
   → Power Automate Cloud

3. Is it legacy systems / high-volume / complex?
   → Automation Anywhere

4. Is it conversational / chat-based?
   → Copilot Studio
```

---

## 6. In-House vs. SaaS Embedded AI

### 6.1 Decision Framework

Bank ABC uses several SaaS applications that may include embedded AI capabilities. This section provides guidance on when to use SaaS-embedded AI vs. building in-house.

#### 6.1.1 When to Use SaaS Embedded AI

Use vendor-provided AI when:
- Feature is core to the SaaS product
- Vendor AI meets quality and compliance needs
- Minimal customization required
- Data handling meets bank requirements
- Cost-effective compared to custom build
- Faster time to value

Examples:
- CRM-embedded recommendation engines
- Email security AI filtering
- SaaS analytics and insights features

#### 6.1.2 When to Build In-House

Build custom AI when:
- Bank-specific requirements not met by vendor
- Competitive differentiation needed
- Data cannot leave bank systems
- Deep integration with bank data required
- Vendor AI quality insufficient
- Long-term cost benefits

Examples:
- Customer-specific risk models
- Bank-branded customer assistants
- Proprietary analytics

### 6.2 SaaS AI Capability Assessment

When evaluating SaaS-embedded AI:

| Assessment Area | Questions to Ask |
|-----------------|------------------|
| **Data Handling** | Where is data processed? Stored? Who has access? |
| **Model Transparency** | Can vendor explain how AI works? |
| **Customization** | Can AI be tuned to bank needs? |
| **Compliance** | Does it meet regulatory requirements? |
| **Performance** | Quality metrics available? SLAs? |
| **Cost** | Pricing model? Included vs. additional? |
| **Governance** | How to audit? How to override? |

### 6.3 In-House Application Integration

#### 6.3.1 Corporate Banking Portal Integration

For AI/Automation integration with Corporate Banking Portal:
- Custom development in coordination with portal team
- API-based integration patterns
- Follow portal development standards
- GenAI features via AI Fatema or dedicated deployment
- Governance: Standard intake process

#### 6.3.2 ila Bank App Integration

For AI/Automation integration with ila Bank digital banking app:
- Mobile-optimized implementations
- Real-time performance requirements
- Customer-facing quality standards
- Strict security and testing requirements
- Governance: Minimum Tier 2 for customer-facing AI

---

## 7. Architecture Pattern Catalog

### 7.1 GenAI Patterns

#### 7.1.1 Basic Conversational AI
- Single-turn or multi-turn conversation
- Prompt engineering for behavior
- Content filtering and guardrails
- Use AI Fatema for internal applications

#### 7.1.2 RAG (Retrieval-Augmented Generation)
- Document chunking and embedding
- Vector similarity search
- Context injection into prompts
- Source attribution in responses
- Qdrant as primary vector store

#### 7.1.3 Document Processing
- Text extraction from documents
- Structured data extraction
- Summarization and analysis
- Hybrid with workflow automation

### 7.2 Analytical AI Patterns

#### 7.2.1 Batch Inference
- Scheduled scoring jobs
- Bulk predictions
- Results to database/data lake
- SageMaker Batch Transform

#### 7.2.2 Real-Time Inference
- API-based predictions
- Low-latency requirements
- Auto-scaling endpoints
- SageMaker Endpoints

#### 7.2.3 Embedded Scoring
- In-application scoring
- Edge deployment scenarios
- Model serialization (ONNX, etc.)

### 7.3 Automation Patterns

#### 7.3.1 Attended Bot
- User-triggered execution
- Desktop assistance
- Interactive processes
- Power Automate Desktop

#### 7.3.2 Unattended Batch
- Scheduled execution
- High-volume processing
- No user interaction
- Automation Anywhere

#### 7.3.3 Event-Triggered Workflow
- Trigger-based execution
- Integration scenarios
- Approval workflows
- Power Automate Cloud

### 7.4 Hybrid Patterns

#### 7.4.1 AI-Augmented Automation
```
Document → [AI Extraction] → [Validation Rules] → [Automated Actions]
```
- GenAI for intelligent extraction
- Automation for workflow execution
- Human-in-loop for exceptions

#### 7.4.2 Automation-Orchestrated AI
```
Trigger → [Data Prep Automation] → [AI Model] → [Result Processing]
```
- Automation prepares data
- AI provides predictions/decisions
- Automation handles outputs

---

## 8. Approved Technology Stack

### 8.1 Approved Platforms Summary

| Category | Approved Technologies | Primary | Notes |
|----------|----------------------|---------|-------|
| **GenAI Platform (Internal)** | AI Fatema | ✓ | Preferred for internal GenAI |
| **GenAI API - Azure** | Azure OpenAI | ✓ | GPT-4, GPT-4o, GPT-3.5 |
| **GenAI API - AWS** | AWS Bedrock | ✓ | Claude, Titan, Llama |
| **Analytical AI** | AWS SageMaker | ✓ | Primary ML platform |
| **MLOps** | MLflow | ✓ | Experiment tracking, registry |
| **MLOps** | SageMaker | ✓ | Training, endpoints |
| **Vector Database** | Qdrant | ✓ | Primary for RAG |
| **Vector Database** | pgvector | | Simple RAG scenarios |
| **RPA** | Automation Anywhere | ✓ | Enterprise RPA |
| **RPA** | Power Automate Desktop | | Microsoft ecosystem |
| **Workflow** | Power Automate Cloud | ✓ | Business workflows |
| **Conversational AI** | Copilot Studio | ✓ | Low-code agents |
| **Agentic AI** | MS Foundry | ✓ | High-code agents |
| **Data Platform** | Lakehouse Architecture | ✓ | Via IT Data Management |

### 8.2 Restricted/Prohibited Technologies

#### 8.2.1 Technologies Requiring Exception Approval

| Technology | Reason | Exception Authority |
|------------|--------|---------------------|
| Self-hosted LLMs | Security, infrastructure | AI & Automation Steering Committee |
| Non-approved cloud AI services | Security, vendor risk | AI & Automation Steering Committee |
| Open-source AI frameworks not on approved list | Security review needed | Head of AI Engineering |
| Custom model training on non-AWS platforms | Infrastructure standardization | Head of AI Engineering |

#### 8.2.2 Explicitly Prohibited

| Technology | Reason |
|------------|--------|
| Consumer AI tools (ChatGPT direct, etc.) | Data security, compliance |
| Unapproved third-party AI APIs | Vendor risk, data handling |
| Shadow AI/automation deployments | Governance, security |
| AI tools without data residency clarity | Regulatory compliance |

### 8.3 Emerging Technologies Watch List

Technologies under evaluation for potential future approval:

| Technology | Status | Evaluation Timeline |
|------------|--------|---------------------|
| Self-hosted Llama 3 | Security review | Q2 2024 |
| Self-hosted Mistral | Infrastructure planning | Q3 2024 |
| Additional Bedrock models | Ongoing evaluation | Continuous |
| Advanced RAG frameworks | Technical evaluation | Q2 2024 |
| Multi-agent orchestration tools | Research phase | Q4 2024 |

---

## 9. Selection Process

### 9.1 Technology Selection Workflow

```
┌─────────────────────┐
│ 1. Use Case Intake  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ 2. Profile Use Case │  ◀── Section 5.1 dimensions
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ 3. Match to Pattern │  ◀── Section 5.2-5.4 matrices
└──────────┬──────────┘
           │
           ▼
┌─────────────────────────────────────────────┐
│ 4. Is it a pre-approved pattern/technology? │
└──────────┬───────────────────┬──────────────┘
           │ YES               │ NO
           ▼                   ▼
┌─────────────────────┐  ┌─────────────────────┐
│ 5a. Document in     │  │ 5b. Technology      │
│     Solution Design │  │     Exception       │
└──────────┬──────────┘  │     Process         │
           │             └──────────┬──────────┘
           │                        │
           ▼                        ▼
┌─────────────────────┐  ┌─────────────────────┐
│ 6. Proceed with     │  │ 6. Approval +       │
│    Development      │  │    ADR Required     │
└─────────────────────┘  └─────────────────────┘
```

### 9.2 Roles and Responsibilities

| Role | Responsibility in Technology Selection |
|------|---------------------------------------|
| **Head of AI Engineering** | Final authority on technology decisions; Exception approval |
| **Data Scientist** | AI technology recommendation; Feasibility assessment |
| **Business Analyst** | Automation technology recommendation; Process assessment |
| **Digital Product Owner** | Business requirements validation |
| **IT Department** | Infrastructure feasibility; Security review coordination |

### 9.3 Decision Documentation

#### 9.3.1 Architecture Decision Record (ADR) Requirements

For non-trivial technology decisions, document using ADR format:

```markdown
# ADR-{number}: {Title}

## Status
[Proposed | Accepted | Deprecated | Superseded]

## Context
What is the issue that we're seeing that motivates this decision?

## Decision
What is the change that we're proposing/making?

## Technology Selected
- Primary: {Technology}
- Alternatives Considered: {List}

## Selection Rationale
Why this technology over alternatives?

## Consequences
What becomes easier or more difficult because of this change?

## Compliance
- Risk Tier: {1|2|3}
- Governance Requirements: {List}
- IT Coordination: {Required|Not Required}
```

#### 9.3.2 When ADR is Required

| Scenario | ADR Required |
|----------|--------------|
| Pre-approved pattern, pre-approved tech | No |
| Pre-approved pattern, non-standard config | Yes (brief) |
| New pattern, approved tech | Yes |
| Any non-approved technology | Yes (detailed) |
| Exception request | Yes (detailed) |

---

## 10. Exception Process

### 10.1 Non-Standard Technology Request

#### 10.1.1 Request Process

1. **Identify Need:** Document why approved technologies don't meet requirements
2. **Research Alternatives:** Evaluate alternative approaches within approved stack
3. **Prepare Request:** Complete Non-Standard Technology Request Form
4. **Risk Assessment:** Assess security, compliance, operational risks
5. **Submit for Review:** Submit to Head of AI Engineering
6. **Approval/Rejection:** Decision documented with rationale

#### 10.1.2 Evaluation Criteria

| Criterion | Questions |
|-----------|-----------|
| **Business Justification** | Why can't approved technologies meet the need? |
| **Technical Fit** | Does this technology solve the problem effectively? |
| **Security** | What are the security implications? IT Security review? |
| **Compliance** | Does it meet regulatory requirements? |
| **Vendor Risk** | Is the vendor established? What's the support model? |
| **Integration** | How does it integrate with existing systems? |
| **Skills** | Do we have or can we acquire necessary skills? |
| **Total Cost** | What's the total cost of ownership? |
| **Exit Strategy** | Can we migrate away if needed? |

#### 10.1.3 Risk Assessment Requirements

For exception requests, assess:
- Data security risks
- Compliance/regulatory risks
- Operational risks
- Vendor/continuity risks
- Integration risks
- Skill/knowledge risks

### 10.2 Approval Authority

| Exception Type | Approver | Timeline |
|----------------|----------|----------|
| Minor deviation (config, version) | Head of AI Engineering | 2-3 days |
| New tool within approved category | Head of AI Engineering | 1 week |
| New category of technology | AI & Automation Steering Committee | 2-3 weeks |
| Technology with significant risk | AI & Automation Steering Committee + IT | 3-4 weeks |

### 10.3 Exception Documentation

All approved exceptions must document:
- Original request and justification
- Risk assessment findings
- Approval decision and conditions
- Mitigation measures required
- Review/expiration date
- Monitoring requirements

---

## 11. Governance & Review

### 11.1 Technology Stack Review

#### 11.1.1 Annual Review Process

Annual review of approved technology stack:
1. Assess current technology performance and adoption
2. Evaluate new technologies in market
3. Review exception requests and patterns
4. Update approved/restricted lists
5. Communicate changes to stakeholders

#### 11.1.2 Emerging Technology Assessment

Ongoing assessment of new technologies:
- Monitor AI/ML market developments
- Evaluate vendor roadmaps
- Conduct pilots where appropriate
- Document findings and recommendations
- Present to Steering Committee for approval decisions

### 11.2 Vendor Management

#### 11.2.1 Vendor Relationship Ownership

| Vendor/Technology | Relationship Owner |
|-------------------|-------------------|
| Azure OpenAI | Head of AI Engineering + IT |
| AWS Bedrock/SageMaker | Head of AI Engineering + IT |
| Automation Anywhere | Head of AI Engineering |
| Microsoft Power Platform | IT Department + I&D |
| Qdrant | Head of AI Engineering |

#### 11.2.2 Contract Coordination

- Licensing managed through IT Procurement
- Technical requirements from Innovation & Digitization
- Security requirements from IT Security
- Contract renewals reviewed annually

### 11.3 Deprecation Process

When technology is deprecated:

1. **Announce Deprecation:** Communicate to stakeholders
2. **Set Timeline:** Define migration timeline
3. **Identify Affected:** List all affected applications/processes
4. **Migration Plan:** Create migration plan for each
5. **Execute Migration:** Support teams in migration
6. **Retire:** Remove from approved list, decommission

---

## Appendices

### Appendix A: Technology Selection Checklist

#### Pre-Selection
- [ ] Use case profiled (Section 5.1)
- [ ] Initiative type determined (AI/Automation/Hybrid)
- [ ] Pre-approved patterns reviewed
- [ ] Business requirements documented

#### Selection
- [ ] Technology options identified
- [ ] Selection criteria applied
- [ ] Decision documented (ADR if required)
- [ ] Alignment with approved stack verified
- [ ] Exception request submitted (if needed)

#### Approval
- [ ] Appropriate approval obtained
- [ ] IT coordination completed (if required)
- [ ] Security review completed (if required)
- [ ] Documentation finalized

### Appendix B: Architecture Decision Record Template

```markdown
# ADR-{YYYY-NNN}: {Short Title}

**Date:** {YYYY-MM-DD}
**Status:** {Proposed | Accepted | Deprecated | Superseded by ADR-XXX}
**Deciders:** {List of people involved in decision}

## Context

{Describe the context and problem statement. What issue are we facing?}

## Decision Drivers

- {Driver 1}
- {Driver 2}
- {Driver 3}

## Considered Options

1. {Option 1}
2. {Option 2}
3. {Option 3}

## Decision Outcome

**Chosen option:** "{Option X}"

### Rationale

{Explain why this option was chosen}

### Consequences

**Positive:**
- {Positive consequence 1}
- {Positive consequence 2}

**Negative:**
- {Negative consequence 1}
- {Negative consequence 2}

## Technology Details

| Aspect | Details |
|--------|---------|
| Technology | {Name} |
| Version | {Version} |
| Vendor | {Vendor} |
| Platform | {Azure/AWS/On-prem} |
| License | {License type} |

## Compliance

- **Risk Tier:** {1 | 2 | 3}
- **Security Review:** {Required | Completed | N/A}
- **IT Coordination:** {Required | Completed | N/A}

## References

- {Link to related documents}
```

### Appendix C: Non-Standard Technology Request Form

```markdown
# Non-Standard Technology Request

**Request ID:** {Auto-generated}
**Date:** {YYYY-MM-DD}
**Requestor:** {Name, Role}
**Project/Use Case:** {Name}

## 1. Technology Requested

| Field | Value |
|-------|-------|
| Technology Name | |
| Vendor | |
| Version | |
| Category | {AI Platform | Automation | Database | Framework | Other} |

## 2. Business Justification

### Why is this technology needed?
{Description}

### Why can't approved technologies meet this need?
{Specific gaps in approved stack}

### What alternatives were considered?
{List of alternatives and why rejected}

## 3. Technical Assessment

### How will this technology be used?
{Description of intended use}

### Integration requirements
{How it integrates with existing systems}

### Infrastructure requirements
{Compute, storage, network needs}

## 4. Risk Assessment

| Risk Category | Assessment | Mitigation |
|--------------|------------|------------|
| Security | | |
| Compliance | | |
| Operational | | |
| Vendor | | |
| Skills | | |

## 5. Cost Estimate

| Item | One-time | Annual |
|------|----------|--------|
| License | | |
| Infrastructure | | |
| Implementation | | |
| Training | | |
| **Total** | | |

## 6. Approvals

| Role | Name | Decision | Date |
|------|------|----------|------|
| Head of AI Engineering | | | |
| IT Security (if required) | | | |
| Steering Committee (if required) | | | |
```

### Appendix D: Use Case Profile Assessment Template

```markdown
# Use Case Technology Profile

**Use Case Name:** {Name}
**Intake ID:** {ID}
**Assessment Date:** {Date}
**Assessor:** {Name}

## 1. Initiative Type Assessment

| Question | Answer | Notes |
|----------|--------|-------|
| Does it require judgment/learning from data? | Yes/No | |
| Is there sufficient quality data available? | Yes/No | |
| Is the process rule-based? | Yes/No | |
| Is it repetitive/high-volume? | Yes/No | |
| **Initiative Type:** | AI / Automation / Hybrid | |

## 2. Dimension Profile

| Dimension | Value | Notes |
|-----------|-------|-------|
| Complexity | Low / Medium / High | |
| Volume | Low / Medium / High | |
| Latency | Real-time / Near-real-time / Batch | |
| Integration | None / Simple / Complex | |
| User Type | Internal / External | |
| Data Type | Structured / Unstructured / Mixed | |

## 3. Technology Recommendation

| Component | Recommended Technology | Alternative |
|-----------|----------------------|-------------|
| Primary Platform | | |
| AI/ML Technology | | |
| Automation Tool | | |
| Data Store | | |
| Integration | | |

## 4. Pattern Match

**Pre-approved Pattern:** {Pattern name or "Custom"}

**Justification:**
{Why this technology selection}

## 5. Governance Classification

- **Risk Tier:** {1 | 2 | 3}
- **ADR Required:** {Yes | No}
- **Exception Required:** {Yes | No}
```

### Appendix E: Reference Architecture Diagrams

*Note: Detailed architecture diagrams for each pre-approved pattern are maintained in the Architecture Repository and referenced from this document.*

**Available Reference Architectures:**
1. RAD-001: Internal GenAI Assistant (AI Fatema)
2. RAD-002: RAG Document Q&A
3. RAD-003: SageMaker ML Pipeline
4. RAD-004: Hybrid Document Processing
5. RAD-005: Enterprise RPA (Automation Anywhere)
6. RAD-006: Power Platform Workflow
7. RAD-007: Copilot Studio Agent
8. RAD-008: MS Foundry Agentic AI

---

## Document Control

### Related Documents
- AI, Automation & Intelligent Solutions Governance Operating Model (AI-GOV-001)
- AI, Automation & Intelligent Solutions Intake & Prioritization Framework (AI-GOV-002)
- AI/ML Development Standards (AI-ENG-001)
- Automation Development Standards (AI-ENG-002)
- Model Validation Standards (AI-VAL-001)
- Monitoring & Performance Standards (AI-MON-001)
- AI & Automation Security Standards (AI-SEC-001)

### Approval History

| Version | Date | Author | Approver | Changes |
|---------|------|--------|----------|---------|
| 1.0 | [Date] | [Author] | [Approver] | Initial release |
