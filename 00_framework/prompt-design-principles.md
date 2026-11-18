# Prompt Design Principles

A practical guide for creating **clear, reusable, and decision-oriented AI prompts** for IT project management.

**Core principle:** Start with the business problem, provide relevant context, define the expected output, and validate the result.

## 1. Start With the Business Problem

Every prompt should address a specific management need, risk, issue, or decision.

**Avoid:**
```text
Create a risk table.
```

**Use:**
```text
Identify project risks requiring immediate escalation
and assess whether existing mitigation actions are sufficient.
```

**Rule:** Define the decision before defining the AI task.

## 2. Select the Right Professional Role

Assign expertise that matches the task—not automatically the most senior title.

| Role | Best Used For |
|---|---|
| IT Project Manager | Planning, delivery, risks, stakeholders |
| Delivery Manager | Delivery performance, resources, profitability |
| PMO Lead | Governance, KPIs, portfolio reporting |
| Business Analyst | Requirements, processes, gap analysis |
| Risk Manager | Risk assessment, mitigation, escalation |
| QA Manager | Testing, defects, UAT, release readiness |
| Product Owner | Backlog, priorities, business value |
| Scrum Master | Sprint delivery, blockers, team improvement |
| Solution Architect | Architecture, integrations, technical risks |
| Vendor Manager | Supplier performance, contractual dependencies |

**Example:**
```text
You are a Senior IT Project Manager specializing in
software delivery, risk management, stakeholder coordination,
and project governance.
```

## 3. Define One Clear, Specific Task

Each prompt should focus on one primary management objective.

Specify:
- **What:** The analysis or action required.
- **Why:** The decision or outcome it supports.
- **When:** Relevant timeframe or deadline.
- **Scope:** Relevant boundaries and constraints.

**Avoid:**
```text
Analyze this project.
```

**Use:**
```text
Identify the five most significant delivery risks
that could affect production release within eight weeks.
Recommend mitigation actions and escalation priorities.
```

Separate unrelated tasks into reusable prompts.

## 4. Provide Relevant Project Context

Include only information that materially affects the analysis.

**Core inputs:**
```text
PROJECT CONTEXT

Project: [NAME]
Business objective: [OBJECTIVE]
Phase: [INITIATION / PLANNING / DELIVERY / TESTING / RELEASE]
Delivery approach: [AGILE / PREDICTIVE / HYBRID]
Current status: [GREEN / AMBER / RED]
Timeline: [KEY MILESTONES]
Budget: [IF RELEVANT]
Stakeholders: [KEY ROLES]
Risks and issues: [KNOWN ITEMS]
Dependencies: [CRITICAL DEPENDENCIES]
Constraints: [RESOURCES / TECHNICAL / REGULATORY]
```

### Adapt to the Delivery Framework

| Framework | Relevant Context |
|---|---|
| Agile / Scrum | Sprint Goal, backlog, velocity, blockers, Definition of Done |
| Kanban | WIP limits, cycle time, lead time, throughput, blocked work, SLE |
| Predictive | Baseline schedule, critical path, milestone and cost variance |
| Hybrid | Governance milestones, iterations, releases, cross-team dependencies |

**Rule:** Include framework-specific details only when relevant.

## 5. Define the Output and Audience

Specify the expected structure, level of detail, and target audience.

**Common output formats:**

| Output | Recommended Content |
|---|---|
| Risk Register | Risk, probability, impact, mitigation, owner |
| Action Plan | Action, priority, owner, deadline |
| Executive Status Report | RAG status, progress, risks, decisions |
| Decision Matrix | Options, benefits, risks, recommendation |
| Issue Log | Issue, root cause, impact, resolution |
| UAT Readiness Report | Test results, defects, blockers, go/no-go criteria |
| Stakeholder Analysis | Influence, interest, engagement strategy |

**Example:**
```text
OUTPUT FORMAT

Provide a table with:
Risk | Root Cause | Probability | Impact |
Mitigation | Owner | Due Date | Escalation Trigger

Conclude with:
1. Top three management priorities
2. Recommended actions
3. Decisions requiring approval
```

**Audience guidance:**
- **Delivery Team:** Blockers, actions, owners, deadlines.
- **Steering Committee:** Milestones, budget, risks, escalations.
- **Executive Sponsor:** Business impact, strategic risks, decisions.

## 6. Require Evidence-Based Analysis

Prevent unsupported conclusions and false precision.

**Reusable instruction:**
```text
Use confirmed project information as the basis for analysis.

Clearly distinguish:
- Confirmed facts
- Assumptions
- Information gaps
- Recommendations

Identify likely root causes, dependencies, and project impacts.
Do not invent missing information or unsupported numerical estimates.
```

For significant issues, assess:

**Symptom → Root Cause → Impact → Corrective Action → Owner**

Use defined probability and impact scales rather than unsupported risk percentages.

## 7. Make Recommendations Actionable

Every recommendation should support a practical management decision.

**Avoid:**
```text
Monitor the integration delay closely.
```

**Use:**
```text
Agree a recovery plan with the API provider within
two working days and evaluate an approved testing workaround.
```

Where relevant, specify:

**Action + Accountable Owner + Priority + Due Date + Escalation Trigger**

### Define Decision and Escalation Criteria

Use project-specific thresholds.

**Examples:**
- Milestone delay exceeds the approved tolerance.
- Budget variance exceeds the agreed threshold.
- Critical dependency has no recovery plan.
- Severity 1 defect remains unresolved before release.
- Vendor misses a contractual commitment.

For major decisions, define acceptance criteria before requesting a recommendation.

## 8. Apply a Quality Review

Include this compact QA instruction in important prompts.

```text
QUALITY REVIEW

Act as a Senior QA Manager and review the output.

Verify:
1. Accuracy: Conclusions are supported by available evidence.
2. Completeness: Relevant risks, dependencies, and gaps are covered.
3. Actionability: Recommendations are feasible, prioritized,
   and assigned to accountable owners.
4. Governance: Escalations and required approvals are identified.
5. Confidentiality: Sensitive project information is protected.

Flag contradictions, unsupported claims, and missing information.

OUTPUT:
- Quality verdict: PASS / REVISE
- Findings requiring correction
- Recommended improvements

Do not invent missing information.
```

## 9. Protect Confidentiality and Human Accountability

AI supports project decisions; it does not replace accountable decision-makers.

**Before submitting project data:**
- Remove or anonymize personal and client information.
- Never include passwords, credentials, or API keys.
- Protect commercial pricing, contracts, and proprietary information.
- Follow organizational data protection and AI usage policies.

Use placeholders such as `[CLIENT]`, `[VENDOR]`, and `[PROJECT]`.

**Require human validation before:**
- Budget or scope changes
- Contractual commitments
- Risk acceptance
- Production release or go-live
- Security-sensitive decisions
- Executive reporting

Apply PMI, PMBOK, Scrum, Kanban, DevOps, or other professional practices only where relevant. Do not imply formal certification or compliance without verification.

## 10. Design for Reuse and Version Control

Keep reusable prompt instructions separate from project-specific information.

```text
REUSABLE PROMPT
+ PROFESSIONAL ROLE
+ PROJECT CONTEXT
+ OUTPUT FORMAT
+ QUALITY REVIEW
```

Use placeholders to support reuse across projects.

**Minimum prompt metadata:**

| Field | Purpose |
|---|---|
| Prompt ID / Name | Identification |
| Category / Use Case | Intended application |
| Owner | Accountability |
| Version | Change tracking |
| Status | Draft / Tested / Reviewed / Approved / Retired |
| Last Reviewed | Maintenance |
| Expected Output | Deliverable definition |

Test prompts against realistic project scenarios before publishing or approving them.

---

## Prompt Quality Checklist

Before publishing a reusable prompt, confirm:

- [ ] **Purpose:** Business problem and required decision are clear.
- [ ] **Role:** Professional expertise matches the task.
- [ ] **Task:** One primary objective with defined scope.
- [ ] **Context:** Relevant project information is provided.
- [ ] **Framework:** Delivery methodology is reflected where relevant.
- [ ] **Output:** Structure and target audience are specified.
- [ ] **Evidence:** Facts, assumptions, and gaps are distinguishable.
- [ ] **Actions:** Recommendations include ownership and priorities.
- [ ] **Governance:** Decision criteria, escalations, and approvals are defined where needed.
- [ ] **Quality:** Accuracy, completeness, and feasibility are reviewed.
- [ ] **Security:** Sensitive information is protected.
- [ ] **Reuse:** Placeholders, versioning, and testing support maintenance.

---

## Key Principle

**Measure prompt quality by the usefulness of the management decisions it supports—not by prompt length or complexity.**
