# Lessons Learned Report

## Purpose

Use this prompt to convert retrospective notes, project observations, and delivery outcomes into a structured lessons learned report.

The report should capture:

- what worked well,
- what did not work well,
- why outcomes occurred,
- what should be repeated,
- what should change,
- and how future projects can benefit.

The objective is not to document blame.

The objective is to convert project experience into **reusable organisational knowledge**.

---

## Best Used For

**Project phase:**  
End of Phase / Major Milestone / Release / Project Close / Hypercare Exit

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Programme Manager

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At major milestones and project close

---

# Prompt

```text id="lessons-01"
ROLE

You are a senior IT Project Manager experienced in international
software delivery, project governance, continuous improvement,
delivery performance, stakeholder management, and organisational
learning.

TASK

Create a structured lessons learned report from the retrospective
notes below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Project phase / milestone:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Project objectives:
[OBJECTIVES]

Planned completion:
[DATE]

Actual / forecast completion:
[DATE]

Budget:
[PLANNED / ACTUAL IF AVAILABLE]

Key stakeholders:
[LIST]

Major vendors:
[LIST]

RETROSPECTIVE NOTES

[PASTE NOTES]

OUTPUT FORMAT

Create:

1. Executive Summary
2. What Went Well
3. What Could Be Improved
4. Root Cause Themes
5. Key Recommendations
6. Project Metrics
7. Actions for Future Projects
8. Knowledge Transfer / Ownership
```

---

# 1. Executive Summary

Write 3–5 sentences covering:

```text id="lessons-summary"
Overall delivery outcome
Most important success
Most important challenge
Most valuable lesson
Primary recommendation for future projects
```

Keep this concise and evidence-based.

---

# 2. What Went Well

Provide:

| Item | Evidence / Detail | Why It Worked | Recommendation to Replicate |
|---|---|---|---|

Examples may include:

```text id="lessons-well"
Early stakeholder engagement
Strong vendor governance
Effective UAT preparation
Clear escalation process
High-quality documentation
Early technical proof of concept
Strong cross-functional collaboration
Effective status reporting
Successful release planning
```

Do not write:

> Communication was good.

Instead write:

> Weekly cross-team dependency reviews reduced unresolved integration blockers and enabled earlier escalation to vendor owners.

---

# 3. What Could Be Improved

Provide:

| Item | Impact | Root Cause | Recommendation for Future |
|---|---|---|---|

Examples may include:

```text id="lessons-improve"
Requirements ambiguity
Late security involvement
Insufficient UAT capacity
Poor vendor mobilisation
Unclear ownership
Late architecture decisions
Data-quality assumptions
Environment instability
Weak dependency management
Insufficient operational readiness
```

Focus on system and process improvements rather than individual blame.

---

# Root Cause Rule

Avoid stopping at the symptom.

### Symptom

```text id="lesson-symptom"
UAT started late.
```

### Immediate Cause

```text id="lesson-immediate"
Business testers were not available.
```

### Deeper Cause

```text id="lesson-root"
Business resource commitments were not formally confirmed during
planning and no backup capacity had been identified.
```

The deeper cause produces the more useful lesson.

---

# 4. Root Cause Themes

Group related lessons where patterns exist.

Possible themes:

```text id="lesson-themes"
Planning
Requirements
Governance
Dependencies
Vendor Management
Architecture
Data
Testing
Security
Business Readiness
Communication
Decision-Making
Resources
```

Provide:

| Theme | Related Lessons | Common Root Cause | Future Control |
|---|---|---|---|

---

# Example

```text id="lesson-theme-example"
Theme:
Dependencies

Lessons:
API certification delay
Late security review
Delayed UAT-resource confirmation

Common Root Cause:
Critical external dependencies were tracked, but escalation
thresholds were not defined.

Future Control:
Define owner, due date, trigger, and escalation threshold for every
critical dependency during planning.
```

---

# 5. Key Recommendations

Prioritise the top five recommendations.

Use:

```text id="lesson-recommendation"
1. Recommendation
   Why it matters
   Where it should be applied

2. Recommendation
   Why it matters
   Where it should be applied
```

Recommendations should be reusable beyond the current project.

---

# Recommendation Quality

### Weak

```text id="lesson-rec-weak"
Communicate better.
```

### Better

```text id="lesson-rec-good"
For projects with external integration dependencies, establish a
weekly dependency review from the design phase and define escalation
thresholds before development begins.
```

---

# 6. Project Metrics

Compare planned and actual performance where reliable data exists.

| Metric | Planned | Actual | Variance | Lesson |
|---|---:|---:|---:|---|

Possible measures:

```text id="lesson-metrics"
Completion Date
Budget
Milestone Delivery
Defect Rate
Test Pass Rate
Critical Defects
Vendor Milestone Performance
Release Readiness
Change Requests
Risk Materialisation
```

Do not invent missing values.

---

# Example

| Metric | Planned | Actual | Lesson |
|---|---|---|---|
| UAT Start | 1 Aug | 8 Aug | Business-resource confirmation should occur earlier |
| Critical Defects at UAT | 0 | 1 | Entry criteria were not enforced early enough |
| Budget | €1.8M | €1.76M | Financial control remained effective |

---

# 7. Actions for Future Projects

Turn lessons into specific actions.

Provide:

| Action | Applies To | Owner | Timing | Evidence of Adoption |
|---|---|---|---|---|

Example:

```text id="lesson-action-example"
Action:
Add external dependency escalation thresholds to the standard
project initiation checklist.

Owner:
PMO.

Timing:
Before next project launch.

Evidence:
Updated template approved and published.
```

A lesson without an action may never change future delivery.

---

# Lesson → Improvement Flow

Use:

```text id="lesson-flow"
Observation
↓
Evidence
↓
Root Cause
↓
Lesson
↓
Recommendation
↓
Future Action
↓
Owner
```

---

# 8. Knowledge Transfer

Define how the lesson will be reused.

Possible destinations:

```text id="lesson-knowledge"
PMO knowledge base
Project template library
Delivery playbook
Architecture standards
Testing checklist
Vendor onboarding checklist
Risk library
Project initiation checklist
```

Do not simply archive the report.

---

# Example Input

```text id="lesson-example-input"
Project:
CRM Replacement

Notes:
- weekly status format worked well and sponsor feedback positive
- data migration rehearsal started 2 weeks late
- source data quality worse than expected
- UAT tester availability was confirmed too late
- identity vendor missed certification deadline
- mock service helped protect SIT
- security team engaged early and approval completed on time
- final go-live was 1 week late
- budget completed 3% under approved amount
- business training completed successfully
```

---

# Example Output Excerpt

## What Went Well

| Item | Detail | Recommendation |
|---|---|---|
| Security engagement | Security team joined during design and approval completed on schedule | Engage Security during initiation on future projects |
| Integration contingency | Mock identity service allowed testing to continue during vendor delay | Create mocks for high-risk external dependencies where feasible |
| Reporting | Weekly reporting format was positively received by Sponsor | Retain standard status format |

---

## What Could Be Improved

| Item | Root Cause | Recommendation |
|---|---|---|
| Data migration | Source-data quality was assumed rather than profiled early | Conduct data profiling during discovery |
| UAT resources | Named testers were not confirmed during planning | Require business-resource commitment before UAT planning is approved |
| Vendor dependency | Certification escalation thresholds were unclear | Add formal dependency triggers and escalation rules |

---

# Prompt 2 — Lessons Quality Review

```text id="lessons-review"
ROLE

You are a PMO Director reviewing a project lessons learned report.

TASK

Review the report below.

[PASTE REPORT]

Check for:

- vague lessons,
- blame-oriented language,
- missing evidence,
- symptoms presented as root causes,
- recommendations that are not actionable,
- lessons that are too project-specific to reuse,
- lessons without owners,
- repeated themes that should be consolidated.

OUTPUT FORMAT

Finding
Why It Matters
Recommended Improvement
Priority
```

---

# Prompt 3 — Cross-Project Pattern Analysis

Where lessons from multiple projects are available:

```text id="lessons-cross-project"
ROLE

You are a PMO knowledge-management lead.

TASK

Compare the lessons learned from the projects below.

[PASTE MULTIPLE REPORTS]

Identify:

1. Repeated failure patterns
2. Repeated success patterns
3. Systemic organisational causes
4. Standards or templates that should change
5. Recommended PMO actions

OUTPUT FORMAT

Pattern
Projects Affected
Evidence
Organisational Impact
Recommended PMO Action
```

This converts individual lessons into organisational improvement.

---

# Prompt 4 — Mid-Project Lessons Review

Do not wait until project close.

```text id="lessons-mid-project"
ROLE

You are a senior IT Project Manager facilitating a mid-project
lessons review.

TASK

Review the delivery experience so far.

[PASTE NOTES]

Identify:

- practices to continue,
- practices to stop,
- practices to improve,
- lessons that can still influence the current project.

Prioritise actions that can create benefit before project completion.
```

---

# Agile / Scrum Considerations

Relevant lessons may emerge from:

- retrospectives,
- release reviews,
- backlog management,
- team collaboration,
- product feedback,
- cross-team dependencies.

Avoid duplicating retrospective outputs without adding project-level insight.

---

# Kanban Considerations

Lessons may include:

- bottlenecks,
- WIP policies,
- ageing work,
- blocked dependencies,
- workflow design,
- SLE accuracy.

Example:

> The integration-review stage repeatedly accumulated excessive WIP. Future projects should define review-capacity limits and explicit escalation rules during workflow design.

---

# Predictive Considerations

Lessons may focus on:

- baseline assumptions,
- milestone planning,
- procurement,
- schedule recovery,
- change control,
- estimating.

---

# Hybrid Considerations

Review both:

```text id="lesson-hybrid"
Formal governance performance
+
Adaptive delivery performance
```

A project may have effective Agile team delivery but weak enterprise governance, or the reverse.

---

# Avoid Blame

Avoid:

```text id="lesson-blame"
The vendor was incompetent.

The business team failed.

The developers communicated badly.
```

Prefer:

```text id="lesson-neutral"
Vendor capacity assumptions were not validated before mobilisation.

Business resource commitments were not confirmed early enough.

Cross-team technical dependencies lacked a defined escalation path.
```

The goal is improvement, not assigning personal fault.

---

# Evidence Hierarchy

Where possible, support lessons using:

```text id="lesson-evidence"
Project metrics
Risk / issue history
Decision logs
Vendor performance
Test results
Schedule data
Budget data
Stakeholder feedback
Retrospective feedback
```

Distinguish evidence from opinion.

---

# Quality Checklist

Before finalising the report, confirm:

- [ ] Both successes and improvement areas are included
- [ ] Lessons are evidence-based where possible
- [ ] Root causes are explored
- [ ] Personal blame is avoided
- [ ] Recommendations are specific
- [ ] Recommendations are reusable
- [ ] Actions have owners
- [ ] Lessons are linked to future practice
- [ ] Metrics are used where reliable
- [ ] Knowledge-transfer destination is defined
- [ ] Lessons can be applied before project close where possible

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- continuous improvement,
- organisational learning,
- knowledge transfer,
- delivery performance,
- stakeholder feedback,
- governance,
- project closure.

## PMBOK Relevance

This prompt supports:

- measurement,
- delivery,
- governance,
- team learning,
- stakeholders,
- value.

## Delivery Framework

Framework-neutral.

Adaptable to:

- Predictive
- Agile
- Scrum
- Kanban
- Hybrid

---

# Human Review Required

Validate lessons with:

- Project Manager
- delivery team
- business stakeholders
- PMO
- vendors where appropriate
- Sponsor for strategic lessons

AI can identify patterns and structure observations.

It should not determine organisational conclusions without stakeholder validation.

---

# Confidentiality

Lessons learned may contain sensitive information about:

- vendors,
- internal teams,
- security,
- budgets,
- customer impact,
- performance.

Anonymise information where necessary before sharing outside the appropriate governance environment.

---

# Prompt Metadata

```text id="lessons-metadata"
Prompt ID: REPORT-007
Category: Reporting & Communication
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: PMO / Project Team
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Low
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial IT lessons-learned framework |
