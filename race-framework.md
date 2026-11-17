# RACE Prompt Framework for Project Management

The RACE framework provides a simple and repeatable structure for creating high-quality AI prompts for project-management work.

RACE stands for:

**R — Role**  
**A — Ask**  
**C — Context**  
**E — Expected Output**

The framework is intentionally simple.

Its purpose is not to make prompts longer.

Its purpose is to make project-management requests more precise, reusable, and easier to review.

---

# 1. R — Role

Define the professional perspective required for the task.

A generic role often produces generic output.

## Weak

```text id="race-role-weak"
You are a project manager.
```

## Stronger

```text id="race-role-strong"
You are a senior IT Project Manager experienced in international
software delivery, stakeholder management, risk management,
quality assurance, vendor coordination, and project governance.
```

The role should match the actual task.

Examples:

- Senior IT Project Manager
- Delivery Manager
- PMO Lead
- Business Analyst
- Risk Manager
- Product Owner
- Scrum Master
- Kanban Delivery Lead
- QA Manager
- Vendor Manager

## Principle

Use the **most relevant professional perspective**, not the most impressive title.

---

# 2. A — Ask

Define one clear task.

## Weak

```text id="race-ask-weak"
Review my project and tell me what is wrong.
```

## Stronger

```text id="race-ask-strong"
Review the current project status and identify the five delivery
risks that require immediate management attention.
```

A strong Ask should make clear:

- what should be analysed,
- what decision should be supported,
- what time horizon matters,
- and what result is required.

Avoid combining unrelated tasks.

## Weak

```text id="race-multi-task"
Review the risks, write a status report, create a stakeholder matrix,
and prepare an escalation email.
```

## Better

Use separate prompts for:

1. Risk review
2. Status reporting
3. Stakeholder analysis
4. Escalation communication

This makes each output easier to review, reuse, and version.

---

# 3. C — Context

Context determines how relevant the output will be.

Useful project context may include:

```text id="race-context-list"
Project objective
Project phase
Delivery methodology
Project size
Timeline
Budget
Team structure
Stakeholders
Dependencies
Known risks
Known issues
Vendors
Technical constraints
Security constraints
Regulatory requirements
Relevant metrics
```

Not every prompt needs every field.

Only include information that can materially affect the analysis.

---

## Example Without Context

```text id="race-no-context"
Identify risks in a software project.
```

Likely output:

- schedule delay,
- budget overrun,
- scope creep,
- resource shortage.

These may be valid but are too generic for meaningful project-management use.

---

## Example With Context

```text id="race-with-context"
Project:
Customer onboarding platform replacement

Current phase:
System Integration Testing

Go-live:
6 weeks

Teams:
3 development squads
2 QA teams
External identity-verification vendor

Known issue:
Vendor API certification is 12 working days behind plan.

Dependency:
UAT cannot begin until certification is complete.

Current status:
Amber
```

Now the analysis can focus on the actual delivery environment.

---

# 4. E — Expected Output

Define exactly how the result should be presented.

Without an output instruction, the AI decides the structure.

That may produce useful information but an unusable project artifact.

---

## Example — Risk Analysis

```text id="race-output-risk"
OUTPUT FORMAT

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

## Example — Executive Reporting

```text id="race-output-exec"
OUTPUT FORMAT

1. Executive Summary
2. Overall RAG Status
3. Key Achievements
4. Top Risks and Issues
5. Decisions Required
6. Priorities for the Next Reporting Period
```

The required format should match the intended audience.

---

# RACE in Practice

A structured prompt may look like this:

```text id="race-example"
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

EXPECTED OUTPUT

Provide:

1. Overall UAT readiness:
   Ready / Ready with Conditions / Not Ready
2. Key blockers
3. Risks
4. Required actions
5. Owner for each action
6. Recommended decision
```

The output can now support an actual management decision.

---

# RACE Across Delivery Frameworks

The RACE structure remains the same regardless of the delivery approach.

What changes is the context and the decision criteria.

## Predictive Example

Relevant context may include:

- baseline schedule,
- milestone variance,
- critical path,
- cost variance,
- change requests.

## Scrum Example

Relevant context may include:

- Sprint Goal,
- backlog status,
- blocked work,
- velocity,
- acceptance criteria,
- Definition of Done.

## Kanban Example

Relevant context may include:

- WIP,
- WIP limits,
- cycle time,
- lead time,
- throughput,
- blocked work,
- work item age,
- Service Level Expectation.

## Hybrid Example

Relevant context may include:

- fixed governance milestones,
- iterative development,
- release cadence,
- cross-team dependencies,
- contractual commitments.

The framework should be adapted to the delivery environment rather than forcing every project into the same model.

---

# RACE vs Ad-Hoc Prompting

| Ad-Hoc Prompting | RACE-Based Prompting |
|---|---|
| Generic role | Relevant professional role |
| Vague request | Defined management task |
| Limited context | Project-specific context |
| AI chooses format | PM defines the output |
| Hard to reuse | Repeatable structure |
| Hard to review | Structured review possible |

---

# Senior-Level Extension

For complex projects, RACE should be supplemented with explicit management criteria.

Add:

```text id="race-senior-extension"
Assumptions
Constraints
Dependencies
Risk tolerance
Decision criteria
Escalation thresholds
Decision deadline
Required evidence
```

This improves transparency and reduces unsupported recommendations.

---

# Example — Decision Criteria

Instead of asking:

```text id="race-opinion"
Should we go live?
```

Use:

```text id="race-decision"
Assess go-live readiness against these criteria:

- no open Severity 1 defects,
- critical business processes tested,
- data migration reconciliation above the agreed threshold,
- rollback testing complete,
- operational support ready,
- security approval received,
- business owner approval received.

Identify any failed criteria.

Separate blockers from manageable risks.

Provide a recommendation with rationale.
```

This changes the AI task from:

> Give me an opinion.

to:

> Evaluate the project against defined management criteria.

---

# Small vs Enterprise Use

## Small IT Project

Keep the RACE prompt lightweight.

Example:

```text id="race-small"
ROLE:
You are an IT Project Manager supporting a six-person development team.

ASK:
Identify the three most important delivery risks this week.

CONTEXT:
- 3 developers
- 1 QA
- 1 Product Owner
- payment integration unfinished
- one developer unavailable for three days

OUTPUT:
Risk | Impact | Action | Owner
```

---

## International Enterprise Project

Provide more structured context.

Example:

```text id="race-enterprise"
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
- go-live in 12 weeks
- data migration and API integration on the critical path

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

---

# Standards and Framework Alignment

The RACE framework itself is framework-neutral.

Individual prompts may reference relevant concepts from:

- PMI / PMP
- PMBOK
- Agile
- Scrum
- Kanban
- hybrid delivery
- software quality
- DevOps
- risk management
- governance practices

Use these only where they are relevant to the specific project-management problem.

---

# Quality Check

Before using a RACE prompt, verify:

### Role
Is the professional perspective relevant?

### Ask
Is there one clear primary task?

### Context
Has enough project information been provided?

### Expected Output
Is the result structured for the intended audience?

### Decision Logic
Are assumptions, dependencies, risks, and decision criteria visible where relevant?

If the answer to any of these is **No**, improve the prompt before use.

---

# Key Principle

RACE improves AI output because it improves the quality of the project-management request.

The real value is not better wording.

The real value is:

**clearer thinking, structured analysis, consistent outputs, and better decision support.**
