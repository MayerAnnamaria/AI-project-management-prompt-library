# Chain Prompting Workflow

**Prompt ID:** AIWF-001 | **Category:** Advanced AI Workflows | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Generate consistent, connected project-management deliverables by reusing verified project context across a controlled sequence of AI prompts.

**Use case:** Create a project brief, risk register, risk response plan, and weekly status report without repeatedly entering the same information or allowing unverified AI-generated assumptions to become project facts.

Copy the master prompt, replace the placeholders, and execute the four stages sequentially.

### Master Prompt — Shared Project Context

```text
ROLE

You are a Senior IT Project Manager and PMO Quality Reviewer
experienced in international software delivery, project governance,
risk management, planning, and executive reporting.

PROJECT CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Delivery approach: [PREDICTIVE / AGILE / HYBRID]
Current phase: [PHASE]
Approved scope: [DETAILS]
Out-of-scope items: [DETAILS]
Budget: [AMOUNT / NOT PROVIDED]
Key milestones: [DATES]
Stakeholders: [ROLES]
Suppliers: [DETAILS]
Integrations / dependencies: [LIST]
Major constraints: [LIST]
Known risks and issues: [LIST]
Reporting date / period: [DATE]

WORKFLOW

We will complete four connected project-management tasks:

1. Project Brief
2. Risk Register
3. Risk Response Plan
4. Weekly Project Status Report

Use the same verified project context throughout.

Complete only the requested stage, then stop for review.
Use approved corrections in subsequent stages.

INFORMATION CONTROL

Classify information as:

- CONFIRMED FACT: Explicitly supported by the project input.
- AI ANALYSIS: Your interpretation of the available evidence.
- ASSUMPTION: A condition requiring confirmation.
- RECOMMENDATION: A proposed management action.
- INFORMATION GAP: Missing evidence required for a decision.

Never present AI analysis, assumptions, or recommendations
as confirmed project facts.

Do not invent:
- Budgets or actual expenditure
- Dates or milestone commitments
- Decisions or approvals
- Named owners
- Supplier commitments
- Risk scores based on nonexistent evidence
- Delivery progress or KPI results

Use project IDs consistently across outputs.

Examples:
Risk R-001
Issue I-001
Change CR-001
Decision D-001

For each stage:
1. Use the verified context and relevant approved outputs.
2. Produce the requested deliverable.
3. Flag missing information and unsupported conclusions.
4. Identify items requiring Project Manager validation.
5. Stop before generating the next deliverable.

Do not automatically treat earlier AI-generated outputs
as approved project information.
```

### Stage 1 — Project Brief

```text
TASK 1 — PROJECT BRIEF

Using the project context above, create a concise Project Brief.

Include:

1. Project Overview
2. Business Objectives
3. In-Scope / Out-of-Scope
4. Key Deliverables
5. Major Milestones
6. Dependencies and Constraints
7. Initial Risks
8. Assumptions and Information Gaps

Distinguish approved scope from proposed scope.

Do not invent milestones, costs, or requirements.

OUTPUT

Project Brief
Confirmed Facts
Assumptions
Validation Required

Stop for Project Manager review.
```

### Stage 2 — Risk Register

```text
TASK 2 — RISK REGISTER

Use the verified project context and approved Project Brief.

Identify up to eight material project risks.

For each risk provide:

Risk ID
Category
Cause–Event–Impact Description
Likelihood (1–5)
Impact (1–5)
Risk Score
Early Warning Indicator
Proposed Mitigation
Proposed Owner
Evidence / Assumption

Calculate Risk Score = Likelihood × Impact only when
the scoring method and supporting assessment are available.

Otherwise, mark the score as "To be assessed".

Do not confuse existing issues with future risks.

Check consistency with the approved Project Brief.

Stop for Project Manager review.
```

### Stage 3 — Risk Response Plan

```text
TASK 3 — RISK RESPONSE PLAN

Use the validated Risk Register and project context.

Select up to three risks requiring the most active
management attention.

Do not prioritize solely by numerical score.

Consider:
- Risk severity
- Proximity
- Critical dependencies
- Milestone exposure
- Recovery difficulty
- Business impact

For each risk provide:

Risk ID
Reason for Priority
Response Strategy
Preventive Actions
Trigger / Early Warning
Contingency Actions
Residual Risk
Proposed Owner
Review Date / To Be Confirmed

Preserve the original risk IDs and descriptions.

Distinguish proposed actions from approved commitments.

Stop for Project Manager review.
```

### Stage 4 — Weekly Project Status Report

```text
TASK 4 — WEEKLY PROJECT STATUS REPORT

Use:
- Verified project context
- Approved Project Brief
- Validated Risk Register
- Reviewed Risk Response Plan
- New factual updates for the reporting period

WEEKLY UPDATES

[PASTE CURRENT PROGRESS, ISSUES, DECISIONS, AND METRICS]

Create:

1. Overall RAG Status and Rationale
2. Executive Summary
3. This Week's Progress
4. Key Risks and Issues
5. Risk Response Actions
6. Next Week's Priorities
7. Decisions / Actions Required

Use:
GREEN / AMBER / RED / INSUFFICIENT EVIDENCE

Do not infer current progress from project plans.

Do not claim actions were completed merely because
they appeared in the Risk Response Plan.

Reference risk IDs consistently.

Identify any risk that changed status or became an issue.

After generating the report, reconcile it against
all previously validated project outputs.

OUTPUT

Weekly Status Report
Cross-Document Consistency Check
Unresolved Information Gaps
Required Management Actions
```

### Reusable Checkpoint — Context Integrity

Run this between major stages or whenever project information changes.

```text
CONTEXT CHECKPOINT

Act as an independent PMO Quality Reviewer.

Review the verified project context and all approved
outputs generated in this workflow.

Identify:

1. Confirmed facts
2. AI-generated conclusions
3. Unverified assumptions
4. Missing information
5. Contradictions or outdated information
6. Inconsistent IDs, dates, owners, and milestones

OUTPUT

Item | Source | Current Position |
Issue / Contradiction | Required Correction

Then produce a concise Confirmed Project Context
containing only validated information.

Do not silently overwrite previous project facts.

Flag unresolved contradictions before the next stage.
```

---

## 2. Quality Check

Use this independent review after completing the workflow, especially before publishing formal project documentation.

```text
ROLE

You are an independent Senior PMO Quality Assurance Manager.

TASK

Review the completed chained project-management workflow.

INPUT

[PASTE THE PROJECT BRIEF, RISK REGISTER,
RISK RESPONSE PLAN, AND STATUS REPORT]

CHECK

1. Context Integrity:
   All deliverables use consistent project facts.

2. Traceability:
   Risks, actions, dependencies, and decisions
   retain consistent IDs and references.

3. Accuracy:
   No unsupported facts or invented metrics appear.

4. Assumptions:
   AI-generated assumptions have not become
   accepted facts without validation.

5. Risk Consistency:
   Significant risks remain visible until
   formally closed, accepted, or superseded.

6. Action Consistency:
   Mitigation actions have consistent descriptions,
   ownership, and implementation status.

7. Reporting Accuracy:
   RAG status, progress, and decisions are
   supported by current reporting-period evidence.

8. Governance:
   Proposed actions and recommendations are
   distinguished from authorized decisions.

9. Completeness:
   Critical dependencies, information gaps,
   and unresolved issues are visible.

10. Confidentiality:
    Sensitive project information is handled
    according to organizational requirements.

OUTPUT

Quality verdict: PASS / REVISE

RECONCILIATION TABLE

Item / ID | Earlier Output | Later Output |
Conflict / Gap | Required Correction

ADDITIONAL RESULTS

Findings: [ISSUES]
Required corrections: [ACTIONS]
Approval blockers: [CRITICAL ITEMS]
Validated context: [CONFIRMED FACTS ONLY]

Do not create missing evidence or retrospectively
approve decisions.
```

---

## 3. Practical IT Use Case

### Enterprise CRM Replacement — From Project Context to Weekly Governance

**Scenario:** A company is replacing its legacy CRM system with a cloud-based platform for Sales and Customer Service.

The Project Manager needs several related project documents, all based on the same business scope, integration dependencies, timeline, and risk assumptions.

Instead of preparing four independent prompts, the team uses a controlled chain in which each reviewed output becomes input to the next stage.

### Project Context

| Attribute | Details |
|---|---|
| Project | Enterprise CRM Replacement |
| Business objective | Replace legacy CRM and support Sales / Customer Service |
| Delivery approach | Hybrid |
| Budget | €2.5 million |
| Target go-live | 30 September 2027 |
| Supplier | External CRM Implementation Partner |
| Integrations | SAP, Customer Portal, Identity Provider, Data Warehouse |
| Key constraint | Maintain customer-service operations during migration |
| Current delivery progress | Not provided |

### Example Input

```text
Project: Enterprise CRM Replacement

Objective:
Replace the legacy CRM with a cloud-based solution
supporting Customer Service and Sales.

Budget: €2.5 million
Target go-live: 30 September 2027
Delivery model: Hybrid

Supplier:
External CRM implementation partner.

Key integrations:
- SAP
- Customer Portal
- Identity Provider
- Data Warehouse

Business constraint:
Customer-service operations must continue
during the migration.

Known project risks:
Not yet assessed.

Current project performance:
Not provided.

Task:
Execute the four-stage chain prompting workflow.
```

### Example Output — Stage 1: Project Brief

| Area | Project Brief |
|---|---|
| Objective | Implement cloud-based CRM for Sales and Customer Service |
| Budget | €2.5 million |
| Target go-live | 30 September 2027 |
| Major deliverable | Replacement CRM solution |
| Integration scope | SAP, Customer Portal, Identity Provider, Data Warehouse |
| Delivery approach | Hybrid |
| Supplier | External implementation partner |
| Key constraint | Maintain customer-service continuity |

**Proposed initial risk areas:** Integration dependencies, migration quality, operational continuity, and supplier delivery.

These are assessment candidates, not yet validated project risks.

**Human checkpoint:** Confirm that SAP integration is in scope but changes to SAP itself are excluded, if that distinction reflects the approved scope. Review all milestone and budget assumptions before proceeding.

### Example Output — Stage 2: Risk Register

<text color="secondary" size="xs">Illustrative assessment; likelihood, impact, and ownership require project validation.</text>

| ID | Potential Risk | Likelihood | Impact | Proposed Response |
|---|---|---|---|---|
| R-001 | Identity-provider certification may not be ready for integration testing | TBD | TBD | Confirm certification dependencies and review schedule |
| R-002 | Legacy-data quality problems may delay migration | TBD | TBD | Profile source data and define cleansing ownership |
| R-003 | Cutover disruption may affect customer-service operations | TBD | TBD | Establish continuity and rollback planning |
| R-004 | SAP integration dependencies may delay testing | TBD | TBD | Confirm API responsibilities and test environment access |

**Human checkpoint:** Validate risk causes, likelihood, impact, proximity, and accountable owners before approving the register.

### Example Output — Stage 3: Risk Response Plan

| Risk ID | Preventive Action | Trigger | Contingency |
|---|---|---|---|
| R-001 | Agree identity-provider certification plan | Certification forecast threatens test start | Assess resequencing and alternative testing |
| R-002 | Conduct data profiling and reconciliation planning | Data quality fails agreed readiness criteria | Assess cleansing and migration-plan changes |
| R-003 | Define cutover and operational-continuity approach | Readiness criteria are not met | Assess postponement or approved rollback |

**Management interpretation:** The three risks are proposed for active attention based on potential milestone and business-continuity impact. Final prioritization requires verified scoring and proximity information.

**Human checkpoint:** Confirm action ownership, feasible trigger thresholds, escalation arrangements, and whether contingency measures are authorized.

### Example Output — Stage 4: Weekly Project Status Report

The original project description does not contain current-week progress or delivery results. A valid report must make that limitation visible.

| Report Area | Current Position |
|---|---|
| Overall RAG | Insufficient evidence |
| Progress this week | Not provided |
| Confirmed completed milestones | Not provided |
| R-001 Identity-provider risk | Assessment required |
| R-002 Data-migration risk | Assessment required |
| R-003 Operational-continuity risk | Assessment required |
| Current corrective actions | Not provided |
| Decisions required | Confirm risk ownership and delivery readiness evidence |

**Executive Summary**

The Enterprise CRM Replacement project has a target go-live of 30 September 2027 and a budget of €2.5 million. The preliminary risk analysis highlights integration, data migration, and operational-continuity exposures. However, no current-week performance evidence has been supplied. The Project Manager must obtain milestone, testing, supplier, and risk updates before assigning an official RAG status or presenting delivery progress.

**Next-week information priorities:** Obtain the latest integration plan, data-quality assessment, cutover readiness position, and supplier delivery update. These are proposed information-gathering activities, not confirmed delivery commitments.

### Cross-Document Consistency Review

| Item | Earlier Output | Later Output | Assessment |
|---|---|---|---|
| Project budget | €2.5M | €2.5M | Consistent |
| Target go-live | 30 Sep 2027 | 30 Sep 2027 | Consistent |
| Identity-provider dependency | Project Brief | R-001 / Status Report | Traceable |
| Data migration | Risk R-002 | Response Plan / Status Report | Traceable |
| Continuity requirement | Project Brief | R-003 | Traceable |
| Risk scores | Not validated | Not asserted | Appropriate |
| Current project RAG | Not provided | Insufficient evidence | Appropriate |

### Management Decisions

1. **Validate the baseline:** Confirm approved scope, budget, milestones, and integration responsibilities before using the project brief as a reference.
2. **Prioritize material risks:** Assess likelihood, impact, proximity, and recovery difficulty rather than relying on generic AI scoring.
3. **Approve response ownership:** Assign accountable roles and validate contingency actions before implementation.
4. **Control reporting quality:** Require current project evidence before assigning RAG status, declaring progress, or communicating management decisions.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The workflow preserves project context and maintains consistent risk identifiers. Risks are linked to response planning and management reporting without converting hypothetical assessments into confirmed facts.

**Required corrections:** Validate the initial project scope, approve risk assessments and response owners, and supply current weekly progress information.

**Approval blockers:** Unconfirmed risk prioritization, incomplete ownership, and missing performance evidence for an official weekly report.

**Governance:** Supports PMI-aligned planning, risk management, performance monitoring, stakeholder communication, decision-making, and project assurance.

### Other Reusable Chains

The same controlled approach can support additional project-management workflows:

| Workflow | Connected Deliverables |
|---|---|
| Scope and Change | Requirements → Scope Gap Analysis → Impact Assessment → Steering Decision Paper |
| Issue Management | Issue → Root Cause Analysis → Recovery Plan → Stakeholder Update |
| Supplier Evaluation | RFQ Requirements → Supplier Response Review → Clarifications → Procurement Recommendation |
| Project Initiation | Project Brief → Stakeholder Matrix → RACI → Risk Register → Communication Plan |
| Release Readiness | Release Scope → Readiness Review → Go / No-Go Assessment → Communication |
| Data-Informed Reporting | KPI Validation → Trend Analysis → Management Commentary → Actions |

**Core governance principle:** Each major AI-generated deliverable should be reviewed before it informs the next one. Long workflows should include periodic context refreshes and final reconciliation.

AI can accelerate project documentation and analysis, but it cannot validate facts independently, authorize decisions, or replace accountable project governance. Use approved environments or anonymized information for confidential financial, contractual, security, supplier, or customer data.
