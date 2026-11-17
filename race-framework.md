# RACE Prompt Framework for Project Management

The RACE framework provides a simple structure for creating clear, reusable, and professionally useful AI prompts.

It is built around four elements:

**R — Role**  
**A — Ask**  
**C — Context**  
**E — Expected Output**

The purpose is not to make prompts longer.

The purpose is to make project-management requests more precise.

---

# 1. R — Role

Define the professional perspective required for the task.

A generic role usually produces generic output.

### Weak

```text id="avtclt"
You are a project manager.
```

### Stronger

```text id="psf65n"
You are a senior IT Project Manager experienced in software
implementation, cross-functional delivery, risk management,
stakeholder coordination, and project governance.
```

The role should reflect the expertise required for the specific task.

Examples:

- Senior IT Project Manager
- Delivery Manager
- PMO Lead
- Business Analyst
- Risk Manager
- QA Manager
- Product Owner
- Vendor Manager

### Principle

Use the **most relevant professional perspective**, not the most impressive title.

---

# 2. A — Ask

Define one clear task.

### Weak

```text id="acbd56"
Review my project and tell me what is wrong.
```

### Stronger

```text id="0vl1v1"
Review the current project status and identify the five delivery
risks requiring immediate management attention.
```

A strong Ask should answer:

- What should be analysed?
- What decision should it support?
- What should the AI produce?

Avoid combining several unrelated activities into one prompt.

### Example

Instead of:

```text id="7ot2yc"
Analyse the risks, write a status report, create a stakeholder
matrix, and prepare an escalation email.
```

Use four separate prompts.

This makes the output easier to review and reuse.

---

# 3. C — Context

Context determines how relevant the output will be.

Useful project context may include:

```text id="c1veza"
Project objective
Project phase
Delivery methodology
Team structure
Timeline
Budget constraints
Current status
Milestones
Dependencies
Known risks
Issues
Stakeholders
Vendors
Technical constraints
Regulatory requirements
```

Not every prompt requires every field.

Include only the information that can materially affect the analysis.

---

## Example

### Without Context

```text id="3lcw05"
Identify risks in a software project.
```

Likely result:

- schedule delay,
- budget overrun,
- scope creep,
- resource shortage.

These may be valid, but they are too generic for meaningful project management.

### With Context

```text id="ijqq1d"
Project:
Customer onboarding platform replacement

Current phase:
System integration testing

Go-live:
6 weeks

Teams:
3 development squads
2 QA teams
External identity-verification vendor

Current issue:
Vendor API certification is 12 working days behind schedule.

Dependency:
UAT cannot begin until certification is complete.

Current project status:
Amber
```

The resulting analysis can now focus on the real delivery environment.

---

# 4. E — Expected Output

Define exactly how the information should be presented.

Without an output instruction, the AI decides the format.

That may produce useful content but an unusable deliverable.

---

## Example: Risk Analysis

```text id="8zzbp7"
OUTPUT FORMAT:

Provide a table with:

Risk
Root Cause
Probability
Impact
Early Warning Indicator
Mitigation
Owner
Escalation Trigger
```

---

## Example: Executive Reporting

```text id="j1zcgt"
OUTPUT FORMAT:

1. Executive Summary
2. Overall RAG Status
3. Key Achievements
4. Top Risks and Issues
5. Decisions Required
6. Priorities for Next Reporting Period
```

---

# RACE in Practice

A basic project-management prompt may look like this:

```text id="8sjmp8"
ROLE

You are a senior IT Project Manager experienced in international
software implementation projects.

ASK

Assess whether the project is ready to begin User Acceptance Testing.

CONTEXT

Project:
ERP implementation

Current phase:
System Integration Testing

Planned UAT:
Next Monday

Open defects:
3 Critical
11 High
27 Medium

Test completion:
91%

Business test scripts approved:
85%

Training environment:
Available

Test data:
Incomplete for two business units

OUTPUT

Provide:

1. Overall UAT readiness: Ready / Ready with Conditions / Not Ready
2. Key blockers
3. Risks
4. Required actions
5. Owner for each action
6. Recommended go/no-go decision
```

The output can now support a real project decision.

---

# RACE vs Ad-Hoc Prompting

| Ad-Hoc Prompting | RACE-Based Prompting |
|---|---|
| Generic role | Relevant professional role |
| Vague request | Defined task |
| Little context | Project-specific context |
| AI chooses format | PM defines output |
| Difficult to reuse | Repeatable framework |
| Difficult to review | Structured review possible |

---

# Senior-Level Extension

For complex projects, RACE should be supplemented with explicit decision criteria.

Add:

```text id="l7ppd4"
Assumptions
Constraints
Dependencies
Risk tolerance
Escalation thresholds
Decision deadline
Required evidence
```

For example:

```text id="kkxn5h"
Do not recommend go-live if:

- any Severity 1 defect remains open,
- data migration reconciliation is below 99.5%,
- rollback testing is incomplete,
- or the business owner has not approved operational readiness.
```

This changes the AI task from:

> Give me your opinion.

to:

> Evaluate the project against explicit management criteria.

That is far more useful in professional project environments.

---

# Example: Small IT Project

```text id="m7tcga"
ROLE:
You are an IT Project Manager supporting a six-person development team.

ASK:
Identify the three most important delivery risks for the next sprint.

CONTEXT:
- Two-week sprint
- 3 developers
- 1 QA
- 1 Product Owner
- Payment integration unfinished
- One developer unavailable for three days

OUTPUT:
Risk | Impact | Action | Owner
```

The framework remains lightweight.

---

# Example: Enterprise IT Project

```text id="gad9l2"
ROLE:
You are a senior Delivery Manager responsible for an international
digital transformation programme.

ASK:
Identify the delivery risks requiring executive attention.

CONTEXT:
- 4 countries
- 6 workstreams
- 45 project team members
- 3 external vendors
- €7M programme budget
- Go-live in 12 weeks
- Data migration and API integration on critical path

OUTPUT:

Risk
Root Cause
Schedule Impact
Commercial Impact
Dependency Impact
Mitigation
Executive Decision Required
Owner
Decision Deadline
```

The same framework scales with project complexity.

---

# Quality Standard

Before using a RACE prompt, check:

### Role

Is the professional perspective relevant to the task?

### Ask

Is there one clear primary objective?

### Context

Has enough information been provided to avoid generic output?

### Expected Output

Can the result be directly reviewed, discussed, or converted into a project action?

If the answer to any of these questions is **No**, improve the prompt before using it.

---

# Key Principle

RACE improves AI output because it improves the quality of the project-management request.

The real value is not:

> better wording from AI.

The real value is:

> clearer thinking, structured analysis, and more consistent decision support.
