# Chain Prompting Workflow

## Purpose

Use this workflow when several project-management outputs depend on the same project context.

Instead of starting a new AI conversation for every task, run related prompts sequentially in the same conversation so that each output builds on the previous one.

Example:

```text
Project Context
↓
Project Brief
↓
Risk Register
↓
Risk Response Plan
↓
Status Report
```

The objective is to reduce repeated context entry while improving consistency between project artefacts.

---

## Best Used For

**Project phase:**  
Initiation / Planning / Delivery / Reporting

**Project type:**  
Software implementation / Digital transformation / ERP / Data / Cloud / Infrastructure / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Project Coordinator

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended use:**  
When multiple outputs depend on the same underlying project information

---

# Core Principle

Chain prompting means:

```text
Prompt 1 produces Output A
↓
Prompt 2 uses Output A + existing project context
↓
Prompt 3 uses Outputs A and B
↓
Prompt 4 uses the combined context
```

The prompts are connected.

They are not isolated requests.

---

# Important Rule

Run connected steps in the **same AI conversation** when the workflow depends on context from previous outputs.

Do not unnecessarily restart the conversation between steps.

However, do not assume earlier AI-generated information is automatically correct.

Review important outputs before using them as inputs to later steps.

---

# Example Workflow

This example creates four connected project-management outputs:

```text
1. Project Brief
2. Risk Register
3. Risk Response Plan
4. Weekly Status Report
```

---

# Step 1 — Establish the Project Context

```text
ROLE

You are a senior IT Project Manager.

I will give you four connected project-management tasks.

Use the same project context throughout the conversation.

After completing each task, wait for the next instruction.

TASK 1

Create a concise project brief from the information below.

PROJECT

Project:
Enterprise CRM Replacement

Objective:
Replace the legacy CRM with a cloud-based platform supporting
Customer Service and Sales.

Target go-live:
30 September

Budget:
€2.5M

Delivery model:
Hybrid

Key vendor:
External CRM implementation partner

Key integrations:
SAP
Customer Portal
Identity Provider
Data Warehouse

Major business requirement:
Maintain customer-service operations during migration.

OUTPUT

Provide:

- Project Overview
- Objectives
- Scope
- Key Deliverables
- Major Dependencies
- Key Constraints
- Initial Risks
```

---

# Review Step 1

Before continuing, verify:

- project facts,
- dates,
- scope,
- dependencies,
- assumptions.

Correct errors before the next prompt.

Example:

```text
Correction:

SAP integration is in scope, but changes to SAP itself are not.

The target go-live date is 30 September, not 30 August.

Please update the project brief and use this corrected information
for all following steps.
```

This prevents errors from propagating through the chain.

---

# Step 2 — Create the Risk Register

After reviewing the brief:

```text
Good.

Using the confirmed project context and project brief above,
create an initial risk register.

Identify 8 material project risks.

Include:

Risk ID
Category
Risk Description
Likelihood 1–5
Impact 1–5
Score
Early Warning Indicator
Mitigation
Owner

Use cause-event-impact wording for the risk description.

Do not invent project facts.

Where information is missing, state the assumption explicitly.
```

---

# Example Risk Chain

```text
Project dependency
↓
Risk identified
↓
Risk scored
↓
Mitigation assigned
```

Example:

```text
Cause:
Identity-provider certification depends on an external vendor.

Event:
Certification is not completed before SIT.

Impact:
Authentication testing and UAT may be delayed.
```

---

# Step 3 — Convert Risks Into Response Plans

After reviewing the risk register:

```text
Good.

Using the risk register above, select the three risks requiring
the most management attention.

Do not rank only by numerical score.

Also consider:

- proximity,
- dependency impact,
- ability to affect major milestones,
- recovery difficulty.

For each risk provide:

Risk ID
Response Strategy
Preventive Actions
Trigger Point
Contingency Action
Residual Risk
Owner
Review Date
```

---

# Why This Step Matters

The workflow now moves from:

```text
Risk identification
```

to:

```text
Risk management action
```

A risk register alone does not show how the project will respond.

---

# Step 4 — Generate the Status Report

After reviewing the risk response plan:

```text
Good.

Now create a weekly project status report using the confirmed
project context, risk register, and risk response actions above.

OUTPUT FORMAT

1. Overall Status — RAG
2. Executive Summary
3. Progress This Week
4. Key Risks / Issues
5. Risk Response Actions in Progress
6. Next-Week Priorities
7. Decisions / Actions Required

Do not introduce project facts that have not appeared in the
conversation.

Where evidence is insufficient to determine a RAG status,
say so rather than inventing one.
```

---

# Full Chain

The completed workflow is:

```text
Project Description
↓
Project Brief
↓
Risk Register
↓
Risk Response Plan
↓
Weekly Status Report
```

Each output becomes part of the context for the next one.

---

# Why Chain Prompting Is Powerful

Without chaining:

```text
Prompt 1:
Explain project again

Prompt 2:
Explain project again

Prompt 3:
Explain project again

Prompt 4:
Explain project again
```

This creates:

- duplicated effort,
- inconsistent context,
- different assumptions,
- contradictory outputs.

With chaining:

```text
Shared project context
+
Progressive outputs
=
Greater consistency
```

---

# Chain Prompting Is Not Blind Automation

A critical rule:

```text
AI Output
↓
Human Review
↓
Correction
↓
Next Prompt
```

Not:

```text
AI Output
↓
Automatically becomes truth
↓
Next Prompt
```

Errors in an early output can propagate through every later artefact.

---

# Error Propagation Example

Suppose Step 1 incorrectly states:

```text
UAT starts 1 August.
```

Actual date:

```text
UAT starts 15 August.
```

If the mistake is not corrected:

- risk proximity may be wrong,
- schedule commentary may be wrong,
- weekly reporting may be wrong,
- escalation urgency may be wrong.

Therefore:

> Validate important context between chain stages.

---

# Checkpoint Prompt

Use this between major steps:

```text
Before continuing, review the information currently being used.

Separate it into:

1. Confirmed project facts
2. AI-generated conclusions
3. Assumptions
4. Missing information

Do not proceed until contradictions are highlighted.
```

This introduces a useful governance checkpoint.

---

# Chain Workflow Pattern

A reusable pattern is:

```text
Context
↓
Analyse
↓
Prioritise
↓
Plan
↓
Communicate
```

Example:

```text
Project Context
↓
Risk Analysis
↓
Risk Prioritisation
↓
Response Plan
↓
Executive Report
```

---

# Workflow 2 — Scope to Change Decision

```text
Requirements
↓
Scope Gap Analysis
↓
Change Impact Assessment
↓
Options Analysis
↓
Steering Committee Paper
```

Example prompts:

```text
STEP 1
Review the requirements for ambiguity.

STEP 2
Using the gaps identified above, determine which items may represent
scope changes.

STEP 3
Assess cost, schedule, risk, and technical impact.

STEP 4
Create three management options.

STEP 5
Create a Steering Committee decision paper.
```

---

# Workflow 3 — Issue Management

```text
Issue
↓
Root Cause
↓
Recovery Plan
↓
Stakeholder Communication
↓
Status Update
```

This is useful for:

- outages,
- vendor delays,
- test failure,
- integration issues,
- migration problems.

---

# Workflow 4 — Vendor Evaluation

```text
RFQ Requirements
↓
Supplier Response Review
↓
Clarification Questions
↓
Risk Assessment
↓
Recommendation
```

---

# Workflow 5 — Project Initiation Pack

One initial project description can support:

```text
Project Brief
↓
Project Charter
↓
Stakeholder Matrix
↓
RACI
↓
Initial Risk Register
↓
Communication Plan
```

This can significantly accelerate early project administration.

All outputs still require human validation.

---

# Workflow 6 — Release Readiness

```text
Release Scope
↓
Readiness Assessment
↓
Open Risks / Defects
↓
Go / No-Go Criteria
↓
Executive Recommendation
↓
Stakeholder Communication
```

---

# Prompt Chaining With Structured IDs

For complex workflows, use identifiers.

Example:

```text
Risk R-001
Risk R-002

Decision D-001

Change CR-014

Issue I-006
```

Then later prompts can say:

```text
Using risks R-001 and R-002, create response plans.
```

This reduces ambiguity.

---

# Context Preservation

At the beginning of a long chain, define:

```text
Project name
Objective
Scope
Budget
Timeline
Key stakeholders
Delivery model
Major dependencies
Key constraints
```

These form the shared context.

---

# Context Refresh

Long conversations can accumulate outdated information.

Use:

```text
Before the next task, summarise the current confirmed project
context in no more than 15 bullet points.

Exclude outdated assumptions.

Highlight unresolved contradictions.
```

Then review before continuing.

---

# Chain Branching

Not every workflow must be purely linear.

Example:

```text
Project Brief
       ↓
 ┌─────┴─────┐
 ↓           ↓
Risk       Stakeholder
Register   Matrix
 ↓           ↓
Response   Engagement
Plan       Plan
 └─────┬─────┘
       ↓
Status Report
```

This is useful when multiple outputs share the same source context.

---

# Advanced Branching Prompt

```text
Using the confirmed project brief above:

TASK A
Create the initial risk register.

TASK B
Create the stakeholder matrix.

Treat these as separate analyses using the same project context.

Do not assume conclusions from Task A automatically apply to Task B.
```

---

# Avoid Over-Chaining

A very long chain can become unreliable if:

- context changes,
- assumptions accumulate,
- outdated information remains,
- outputs become increasingly dependent on earlier AI interpretation.

Use checkpoints.

For major workflows:

```text
3–5 steps
↓
Validate context
↓
Continue
```

---

# Fact vs AI-Derived Information

Maintain this distinction:

```text
PROJECT FACT
Provided by source or stakeholder.

AI ANALYSIS
Derived interpretation.

ASSUMPTION
Used because information is missing.

RECOMMENDATION
Suggested future action.
```

Do not allow these categories to become mixed during the chain.

---

# Prompt — Context Integrity Review

```text
ROLE

You are a PMO quality reviewer.

TASK

Review the conversation context used in this chained workflow.

Identify:

- contradictions,
- unsupported facts,
- assumptions that became treated as facts,
- outdated information,
- inconsistent dates,
- inconsistent owners,
- inconsistent risk ratings.

OUTPUT FORMAT

Item
Problem
Source / Origin
Correction Required
Impact on Later Outputs
```

---

# Chain Prompting for Decision Support

A strong decision-support chain can be:

```text
Problem
↓
Evidence
↓
Root Cause
↓
Options
↓
Trade-Off Analysis
↓
Recommendation
↓
Decision Paper
```

This is more valuable than asking:

> What should I do?

because the reasoning structure becomes visible and reviewable.

---

# Example

```text
STEP 1
Analyse why UAT is delayed.

STEP 2
Identify the root causes.

STEP 3
Generate three realistic recovery options.

STEP 4
Compare schedule, cost, quality, and risk trade-offs.

STEP 5
Recommend one option.

STEP 6
Convert the analysis into a Steering Committee paper.
```

---

# Chain Prompting for Data-Informed PM

A data workflow could be:

```text
Raw KPI Data
↓
Metric Validation
↓
Trend Analysis
↓
Root Cause Hypotheses
↓
Management Commentary
↓
Recommended Actions
```

This works particularly well with:

- Jira data,
- testing metrics,
- issue logs,
- budget data,
- schedule performance,
- vendor KPIs.

---

# Example

```text
STEP 1
Check this KPI dataset for missing values and inconsistencies.

STEP 2
Analyse delivery trends.

STEP 3
Identify the three most important management signals.

STEP 4
Write executive dashboard commentary.

STEP 5
Recommend follow-up questions for the delivery leads.
```

---

# Chain Quality Review

At the end of a chain:

```text
Review all outputs produced in this conversation.

Check for:

- contradictions,
- duplicated actions,
- inconsistent owners,
- inconsistent dates,
- unsupported assumptions,
- risks that disappeared without explanation,
- decisions that were never formally made.

Return a reconciliation table.
```

---

# Reconciliation Table

| Item | Earlier Output | Later Output | Conflict | Correction |
|---|---|---|---|---|

This is particularly useful before using chained outputs in formal project documentation.

---

# Agile / Scrum Considerations

Example chain:

```text
Sprint / Release Data
↓
Delivery Risks
↓
Dependency Analysis
↓
Release Forecast
↓
Stakeholder Update
```

Avoid using AI to replace:

- Product Owner decisions,
- team estimation,
- retrospective discussion.

---

# Kanban Considerations

Example:

```text
Flow Metrics
↓
Bottleneck Analysis
↓
Root Cause
↓
Policy Improvement
↓
Service Review Commentary
```

---

# Predictive Considerations

Example:

```text
Schedule Data
↓
Variance Analysis
↓
Critical Dependency Review
↓
Recovery Options
↓
Steering Committee Decision
```

---

# Hybrid Considerations

Combine:

```text
Delivery data
+
Formal project governance
```

Example:

```text
Sprint / Flow Evidence
↓
Project Milestone Impact
↓
Management Options
↓
Governance Decision
```

---

# Confidentiality

The more steps a chained conversation contains, the more project information may accumulate in the AI context.

Before starting a chain, consider whether it includes:

- confidential financial data,
- personal information,
- security vulnerabilities,
- contract information,
- customer data,
- commercially sensitive vendor information.

Use anonymised or approved environments where necessary.

---

# Quality Checklist

Before using chain prompting, confirm:

- [ ] Tasks are logically connected
- [ ] Shared context is clearly defined
- [ ] Each step has a clear output
- [ ] Important outputs are reviewed before reuse
- [ ] Assumptions are identified
- [ ] Facts are not silently changed
- [ ] Context corrections are made explicitly
- [ ] IDs are used where helpful
- [ ] Long chains include checkpoints
- [ ] Final outputs are reconciled
- [ ] Sensitive information is handled appropriately

---

# Key Principle

Chain prompting is not:

```text
Ask AI many questions.
```

It is:

```text
Design a controlled sequence where each validated output
becomes structured input to the next management task.
```

That is what turns individual prompts into an **AI-assisted project-management workflow**.

---

# Prompt Metadata

```text
Prompt ID: AIWF-001
Category: Advanced AI Workflows
Version: 1.0
Status: Draft
Owner: Project Manager / PMO
Reviewer: Project Manager
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial chain-prompting workflow |
