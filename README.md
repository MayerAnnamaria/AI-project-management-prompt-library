# AI Project Management Prompt & Decision Framework Library

A professional library of **reusable AI prompts, management decision frameworks, and quality assurance workflows for IT project management**.

Designed to support evidence-based decision-making, business value delivery, risk management, stakeholder alignment, and effective project governance across the project lifecycle.

The library enables Project Managers and delivery teams to:

- **Evaluate management decisions** — assess business value, delivery feasibility, risks, and trade-offs.
- **Strengthen delivery control** — improve planning, performance reporting, and change management.
- **Manage stakeholder expectations** — communicate professionally, assertively, and with a clear business focus.
- **Improve project quality** — challenge assumptions, validate evidence, and audit deliverables.
- **Apply AI responsibly** — maintain confidentiality, human oversight, and formal decision authority.

> **AI supports management analysis and recommendations. Accountability and formal decision authority remain with authorized project stakeholders.**

---

## Quick Start

Start with the [RACE Prompt Framework](race-framework.md), a reusable approach to structuring AI-assisted project-management tasks.

**Practical IT scenario:** A business stakeholder requests additional functionality shortly before a scheduled software release. The Project Manager must evaluate business criticality, delivery constraints, schedule impact, and available management options.

The framework supports:

- Structured impact assessment.
- Comparison of management options and trade-offs.
- Evidence-based recommendations.
- Professional stakeholder communication.
- Defined actions and approval requirements.

Open the [RACE Framework — Practical IT Use Case](race-framework.md#3-practical-it-use-case) to explore the worked example.

---

## What's Included

| Area | Management Applications |
|---|---|
| **[Framework](00_framework/)** | Standardize prompt design, analytical structure, and quality requirements |
| **[Project Initiation](01_project-initiation/)** | Establish business objectives, project scope, assumptions, and delivery boundaries |
| **[Project Planning](02_project-planning/)** | Define work packages, responsibilities, estimates, schedules, and procurement requirements |
| **[Risk & Issue Management](03_risk-issue-management)** | Identify risk exposure, prioritize responses, and manage issues and escalations |
| **[Reporting & Communication](04_reporting-communication/)** | Communicate project performance, business impact, and required management decisions |
| **[Commercial & Governance](05_commercial-governance/)** | Assess contractual obligations, scope changes, supplier performance, and commercial exposure |
| **[Stakeholder Management](06_stakeholder-management/)** | Align expectations, manage competing priorities, and communicate organizational change |
| **[Advanced AI Workflows](07_advanced-ai-workflows/)** | Connect management activities, challenge recommendations, and improve deliverable quality |
| **[AI Governance](08_ai-governance/)** | Establish confidentiality controls, evidence verification, and responsible AI practices |

---

## Standard Template Structure

Operational templates generally follow a consistent three-section structure to support practical reuse and quality control.

| Section | Purpose |
|---|---|
| **1. Ready-to-Use Prompt** | Defines the professional role, project context, management task, expected output, and quality requirements |
| **2. Quality Check** | Provides a separate review prompt to assess accuracy, evidence, completeness, decision readiness, and governance |
| **3. Practical IT Use Case** | Demonstrates application through an illustrative project scenario, management analysis, and recommended actions |

Governance documents may use a shorter structure where a practical example is not required.

This approach supports consistent documentation, efficient reuse, and structured review across different projects.

---

## How to Use

1. **Define the management objective** — identify the problem, required deliverable, or decision.
2. **Select the relevant template** — choose the prompt or workflow appropriate to the task.
3. **Provide verified project context** — specify facts, constraints, dependencies, and business priorities.
4. **Generate the analysis** — run the prompt in an approved AI environment.
5. **Validate the output** — review evidence, calculations, assumptions, risks, and recommendations.
6. **Apply project governance** — obtain the appropriate review, decision, or approval.

```text
Verified Project Context
          ↓
Structured AI Prompt
          ↓
Analysis & Management Recommendation
          ↓
Quality Check & Evidence Validation
          ↓
Human Review
          ↓
Authorized Decision / Approval
```

**Management principle:** AI-generated recommendations should be assessed against business objectives, delivery constraints, and established decision authority before implementation.

---

## Advanced AI Workflows

The library extends beyond standalone prompts by connecting management activities into reusable workflows.

These workflows support consistency, structured analysis, quality assurance, and continuous improvement across project deliverables.

| Workflow | Process | Management Value |
|---|---|---|
| **[Chain Prompting](07_advanced-ai-workflows/chain-prompting-workflow.md)** | Project Brief → Risk Register → Response Plan → Status Report | Maintains consistency and traceability between related deliverables |
| **[Role-Based Review](07_advanced-ai-workflows/role-stacking-review-workflow.md)** | Draft → Reviewer Challenge → Revision | Challenges assumptions and anticipates stakeholder concerns |
| **[Iterative Refinement](07_advanced-ai-workflows/iterative-refinement-workflow.md)** | Draft → Critique → Rewrite → Validation | Improves analytical quality, clarity, and decision readiness |
| **[Document Audit](07_advanced-ai-workflows/document-audit-workflow.md)** | Document → Gap Analysis → Correction → Re-Audit | Identifies material quality and governance gaps before formal review |

Outputs from earlier workflow stages should be validated before being used as inputs for subsequent management activities.

---

## Delivery Approaches

The library is framework-neutral and adaptable to predictive, adaptive, and hybrid delivery environments.

| Delivery Approach | Management Considerations |
|---|---|
| **Predictive** | Scope baselines, milestone planning, schedule control, formal change management |
| **Adaptive / Agile** | Iterative delivery, evolving requirements, business value prioritization, continuous feedback |
| **Scrum** | Product and Sprint Goals, backlog priorities, dependencies, acceptance, and stakeholder feedback |
| **Kanban** | Workflow efficiency, work-in-progress limits, throughput, cycle time, and blocked work |
| **Hybrid** | Iterative development within defined governance milestones, financial constraints, and delivery commitments |

Select and adapt the relevant practices according to project complexity, delivery methodology, contractual obligations, and organizational governance requirements.

---

## AI Governance & Quality Assurance

AI-assisted project management requires appropriate information security, factual verification, professional judgment, and human oversight.

### Before Using AI

- Use approved AI environments and authorized project information.
- Protect confidential, personal, commercial, and security-sensitive data.
- Apply data minimization and appropriate anonymization.
- Never disclose credentials, API keys, passwords, or production secrets.

### Before Using AI Output

- Verify material facts, dates, calculations, and source references.
- Distinguish confirmed information from estimates, assumptions, and recommendations.
- Assess business value, delivery feasibility, and residual risk.
- Validate contractual, financial, and technical claims.
- Obtain specialist review and formal approval where required.

### Governance References

| Document | Purpose |
|---|---|
| [AI Confidentiality and Professional Responsibility](08_ai-governance/ai-confidentiality-and-professional-responsibility.md) | Protect project information and maintain professional accountability |
| [Hallucination Verification Workflow](08_ai-governance/hallucination-verification-workflow.md) | Identify unsupported claims and verify AI-generated information |
| [Project AI Use Policy](08_ai-governance/project-ai-use-policy.md) | Establish authorized, secure, and accountable AI usage |

**AI-generated content does not constitute independently verified project information, formal approval, or authorization to change project commitments.**

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

## License & Disclaimer

See [LICENSE](LICENSE) for repository usage and distribution terms.

The materials are reusable professional-development templates and illustrative IT project-management scenarios. They are intended to support structured analysis, management recommendations, and professional decision-making.

Adapt all outputs to the specific project context and applicable organizational, security, contractual, legal, and regulatory requirements.

The included examples are illustrative and should not be interpreted as independently validated project results or formally approved management practices.

These materials do not replace professional judgment, specialist expertise, or established project governance processes.

> **Use AI to improve management thinking, strengthen decision quality, and support business value delivery — not to outsource professional accountability.**
