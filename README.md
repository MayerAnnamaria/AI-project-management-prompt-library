# AI Project Management Prompt Library

A practical library of **reusable AI prompts, decision frameworks, and quality assurance workflows** for IT project management.

Designed to help Project Managers and delivery teams analyze complex delivery challenges, evaluate trade-offs, manage risks, communicate with stakeholders, and develop evidence-based management recommendations.

The library combines structured AI prompting with professional project governance to support:

- **Decision-making:** Evaluate competing priorities, delivery risks, and management options.
- **Delivery control:** Structure project planning, reporting, change management, and issue resolution.
- **Stakeholder management:** Develop clear, assertive, business-oriented communication.
- **Quality assurance:** Challenge assumptions, verify information, and improve deliverables.
- **Responsible AI use:** Protect confidential information and maintain human accountability.

**Core principle:** AI supports analysis and recommendations. Formal decisions remain with authorized project stakeholders.

---

## Quick Start — Solve a Real Project Management Challenge

**Scenario:** A stakeholder requests additional functionality four weeks before release. The team has limited capacity, existing delivery commitments, and unresolved technical dependencies.

**Management challenge:** Should the Project Manager accept, defer, or reprioritize the request?

Use the [RACE Prompt Framework](race-framework.md) to evaluate the decision.

1. **Select the framework:** Open `race-framework.md`.
2. **Copy the prompt:** Use the Ready-to-Use Prompt section.
3. **Add project context:** Enter verified requirements, constraints, deadlines, and decision criteria.
4. **Evaluate options:** Generate an impact assessment, management recommendation, and stakeholder communication.
5. **Validate the result:** Run the independent Quality Check before using the recommendation.

**Expected output:** A structured comparison of delivery options, business and schedule trade-offs, a recommended management action, and professional stakeholder communication.

The objective is not simply to generate an answer, but to support an **informed, accountable management decision**.

---

## Explore the Library

| Area | Management Value |
|---|---|
| [Framework & Prompt Design](00_framework/) | Create consistent, reusable, evidence-based AI prompts |
| [Project Initiation](01_project-initiation/) | Define project objectives, scope, assumptions, and delivery boundaries |
| [Project Planning](02_project-planning/) | Structure estimates, responsibilities, dependencies, and execution plans |
| [Risk & Issue Management](03_risk-issue-management/) | Identify threats, assess exposure, and develop response strategies |
| [Reporting & Communication](04_reporting-communication/) | Communicate delivery performance, risks, and management decisions |
| [Commercial & Governance](05_commercial-governance/) | Analyze contractual matters, scope changes, and supplier obligations |
| [Stakeholder Management](06_stakeholder-management/) | Align expectations, communicate change, and manage competing priorities |
| [Advanced AI Workflows](07_advanced-ai-workflows/) | Connect prompts, challenge assumptions, and refine project deliverables |
| [AI Governance](08_ai-governance/) | Support confidentiality, factual verification, and responsible AI use |

### Recommended Starting Points

| Management Need | Recommended Template |
|---|---|
| Structure an AI request | [RACE Prompt Framework](race-framework.md) |
| Create a reusable PM prompt | [Prompt Template](prompt-template.md) |
| Identify project risks | [Risk Register](03_risk-issue-management/risk-register.md) |
| Evaluate delivery performance | [Weekly Status Report](04_reporting-communication/weekly-status-report.md) |
| Prepare a management decision | [Steering Committee Decision Paper](04_reporting-communication/steering-committee-decision-paper.md) |
| Improve a draft document | [Iterative Refinement Workflow](07_advanced-ai-workflows/iterative-refinement-workflow.md) |
| Challenge document quality | [Document Audit Workflow](07_advanced-ai-workflows/document-audit-workflow.md) |
| Verify AI-generated information | [Hallucination Verification Workflow](08_ai-governance/hallucination-verification-workflow.md) |

---

## Repository Structure

```text
AI-project-management-prompt-library/
│
├── README.md
├── LICENSE
├── prompt-template.md
├── race-framework.md
│
├── 00_framework/
│   └── prompt-design-principles.md
│
├── 01_project-initiation/
│   ├── assumptions-constraints.md
│   ├── project-brief.md
│   ├── project-charter.md
│   ├── scope-definition.md
│   └── smart-objectives.md
│
├── 02_project-planning/
│   ├── basis-of-estimate.md
│   ├── communication-management-plan.md
│   ├── procurement-plan.md
│   ├── raci-matrix.md
│   ├── schedule-narrative.md
│   └── work-breakdown-structure.md
│
├── 03_risk-issue-management/
│   ├── issues-log.md
│   ├── qualitative-risk-analysis.md
│   ├── risk-identification-workshop.md
│   ├── risk-management-plan.md
│   ├── risk-register.md
│   └── risk-response-plan.md
│
├── 04_reporting-communication/
│   ├── difficult-stakeholder-communication.md
│   ├── lessons-learned-report.md
│   ├── meeting-minutes.md
│   ├── monthly-progress-report.md
│   ├── performance-dashboard-commentary.md
│   ├── steering-committee-decision-paper.md
│   └── weekly-status-report.md
│
├── 05_commercial-governance/
│   ├── contract-clause-analysis.md
│   ├── contract-closeout.md
│   ├── contractual-claim-notification.md
│   ├── scope-gap-analysis.md
│   ├── supplier-rfq-response-review.md
│   └── variation-change-instruction.md
│
├── 06_stakeholder-management/
│   ├── stakeholder-analysis-matrix.md
│   ├── stakeholder-complaint-response.md
│   ├── stakeholder-engagement-plan.md
│   ├── team-performance-feedback.md
│   └── user-change-notification.md
│
├── 07_advanced-ai-workflows/
│   ├── chain-prompting-workflow.md
│   ├── document-audit-workflow.md
│   ├── iterative-refinement-workflow.md
│   └── role-stacking-review-workflow.md
│
└── 08_ai-governance/
    ├── ai-confidentiality-and-professional-responsibility.md
    ├── hallucination-verification-workflow.md
    └── project-ai-use-policy.md
```

---

## How the Frameworks Work

The templates are designed to support the full progression from project information to management decisions.

```text
Verified Project Context
         ↓
Structured AI Prompt
         ↓
Analysis and Management Options
         ↓
Quality Check and Evidence Validation
         ↓
Project Manager Review
         ↓
Authorized Decision / Approval
```

### Standard Template Structure

Each operational prompt generally follows three sections:

| Section | Content |
|---|---|
| **1. Ready-to-Use Prompt** | Professional role, project inputs, management task, and expected output |
| **2. Quality Check** | Independent review of accuracy, evidence, governance, and practical usefulness |
| **3. Practical IT Use Case** | Realistic project scenario, sample input, management analysis, and recommended actions |

Governance reference documents may use a shorter format where a full worked example adds little value.

This structure makes prompts easier to copy, adapt, review, and reuse across different projects.

---

## Advanced AI Workflows

Beyond individual prompts, the library includes connected workflows for more complex project-management tasks.

| Workflow | Approach | Purpose |
|---|---|---|
| [Chain Prompting](07_advanced-ai-workflows/chain-prompting-workflow.md) | Context → Analysis → Response Plan → Report | Maintain consistency between related deliverables |
| [Role-Based Review](07_advanced-ai-workflows/role-stacking-review-workflow.md) | Author → Stakeholder Challenge → Revision | Anticipate questions and strengthen recommendations |
| [Iterative Refinement](07_advanced-ai-workflows/iterative-refinement-workflow.md) | Draft → Critique → Correct → Validate | Improve clarity, evidence, and executive communication |
| [Document Audit](07_advanced-ai-workflows/document-audit-workflow.md) | Document → Gap Analysis → Correction → Re-Audit | Identify weaknesses before formal review |

These workflows emphasize **progressive analysis and quality control**, rather than treating the first AI-generated answer as final.

---

## Delivery Approaches

The library is framework-neutral and can be adapted to different delivery environments.

| Approach | Typical Considerations |
|---|---|
| Predictive | Baselines, milestones, change control, critical path |
| Scrum | Sprint Goals, backlog priorities, acceptance criteria, dependencies |
| Kanban | WIP, cycle time, throughput, blocked work |
| Hybrid | Iterative delivery, fixed governance milestones, cross-team dependencies |

Relevant PMI, Agile, Scrum, Kanban, and project governance concepts can be incorporated according to the needs of each project.

---

## AI Governance & Responsible Use

AI-assisted project work must remain consistent with organizational confidentiality requirements and established decision authority.

**Before using AI:**

- Use approved AI environments and authorized information.
- Minimize confidential, personal, commercial, and security-sensitive data.
- Never include passwords, API keys, tokens, or production credentials.

**Before using AI-generated outputs:**

- Verify material facts, dates, figures, and calculations.
- Distinguish verified information from assumptions and recommendations.
- Validate contractual and technical claims against authoritative evidence.
- Obtain specialist review and formal approval when required.

For detailed controls, see the [AI Governance](08_ai-governance/) section.

**AI-generated content is a decision-support input, not an independently verified project record or formal authorization.**

---

## License & Disclaimer

The materials are reusable professional-development templates and illustrative project-management examples. They should be adapted to the relevant project, organization, delivery approach, and governance requirements.

They do not replace professional judgment, organizational policies, contractual obligations, or specialist legal, financial, technical, and security review.

**The goal is to make project-management work more structured, evidence-based, and decision-oriented—without outsourcing professional accountability.**
