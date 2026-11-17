# Professional Project Management Prompt Template

Use this template for every reusable prompt in the AI Project Management Playbook.

The objective is to ensure that each prompt is:

- professionally relevant,
- reusable across projects,
- structured for review,
- appropriate for the delivery environment,
- and governed as a project-management asset.

---

# 1. Prompt Name

Use a clear name based on the management problem being addressed.

**Examples:**

- Risk Register Review
- Delivery Delay Analysis
- UAT Readiness Assessment
- Vendor Performance Review
- Executive Status Report
- Stakeholder Engagement Analysis

---

# 2. Business Problem

Explain why the prompt exists.

Focus on the project-management problem rather than the AI task.

### Example

> The Project Manager needs to identify which project risks require immediate management attention and whether current mitigation actions are sufficient.

A strong business problem explains:

- what decision is required,
- why the issue matters,
- who will use the result,
- and what project outcome could be affected.

---

# 3. Best Used For

Define the operating context.

```text
Project phase:
[Initiation / Planning / Delivery / Testing / Deployment / Close-out]

Project environment:
[Software Development / Digital Transformation / Data / Infrastructure / ERP / Product]

Delivery approach:
[Predictive / Agile / Scrum / Kanban / Hybrid / Other]

Project complexity:
[Small / Medium / Enterprise / Programme]

Primary user:
[Project Manager / Project Coordinator / Delivery Manager / PMO / Business Analyst / Product Owner]

Recommended frequency:
[Ad hoc / Daily / Weekly / Monthly / Milestone-based]
```

Only include delivery-framework terminology when it is relevant.

---

# 4. Professional Role

Define the professional perspective required.

### Template

```text
ROLE

You are a senior IT Project Manager experienced in international
software and digital delivery.

You have expertise in project planning, delivery management,
risk management, stakeholder coordination, quality assurance,
vendor management, and project governance.
```

For specialist tasks, use the most relevant role.

Examples:

- Senior Risk Manager
- Delivery Manager
- PMO Lead
- Business Analyst
- Product Owner
- Scrum Master
- Kanban Delivery Lead
- QA Manager
- Vendor Manager
- Solution Architect

### Rule

Use the **most relevant expertise**, not automatically the most senior title.

---

# 5. Task

Define one primary task.

### Template

```text
TASK

Review the project information below and identify the issues
requiring immediate management attention.
```

A strong task should make clear:

- what should be analysed,
- what decision should be supported,
- what time horizon matters,
- and what result is required.

Avoid combining unrelated activities into one prompt.

---

# 6. Project Context

Provide only the information that can materially affect the analysis.

### Template

```text
PROJECT CONTEXT

Project:
[PROJECT NAME OR ANONYMISED DESCRIPTION]

Business objective:
[OBJECTIVE]

Current phase:
[PHASE]

Delivery approach:
[METHODOLOGY / FRAMEWORK]

Current status:
[GREEN / AMBER / RED OR OTHER]

Timeline:
[KEY DATES]

Budget:
[IF RELEVANT]

Team:
[TEAM STRUCTURE]

Stakeholders:
[KEY STAKEHOLDERS]

Dependencies:
[DEPENDENCIES]

Known risks:
[RISKS]

Known issues:
[ISSUES]

Constraints:
[CONSTRAINTS]

Relevant metrics:
[METRICS]
```

Do not provide unnecessary confidential information.

---

# 7. Framework-Specific Context

Use this section only when relevant.

## Agile / Scrum Example

```text
Sprint Goal:
[GOAL]

Sprint:
[NUMBER / DATES]

Backlog status:
[DETAILS]

Velocity / throughput:
[METRIC]

Blocked items:
[DETAILS]
```

## Kanban Example

```text
WIP:
[CURRENT WIP]

WIP limits:
[LIMITS]

Cycle time:
[METRIC]

Lead time:
[METRIC]

Throughput:
[METRIC]

Blocked work:
[ITEMS]

Work item age:
[DETAILS]

Service Level Expectation:
[SLE]
```

## Predictive Example

```text
Baseline schedule:
[DETAILS]

Milestone variance:
[VARIANCE]

Budget variance:
[VARIANCE]

Critical path:
[DETAILS]
```

Do not force framework-specific information into a prompt where it does not belong.

---

# 8. Required Analysis

Define how the information should be analysed.

### Example

```text
REQUIRED ANALYSIS

For each issue:

1. Identify the underlying cause.
2. Distinguish symptoms from root causes.
3. Assess the project impact.
4. Identify affected dependencies.
5. Assess urgency.
6. Recommend an action.
7. Identify an accountable owner.
8. Define an escalation trigger where appropriate.
```

The analysis criteria should match the management decision.

---

# 9. Decision Criteria

For significant project decisions, define explicit criteria.

### Example

```text
DECISION CRITERIA

Do not recommend production release if:

- any Severity 1 defect remains unresolved,
- rollback testing is incomplete,
- critical security approval is missing,
- business readiness is not confirmed,
- or a critical operational dependency remains unresolved.
```

Decision criteria make the output more transparent and repeatable.

---

# 10. Output Format

Always define how the answer should be presented.

### Example

```text
OUTPUT FORMAT

Provide a table:

Issue
Root Cause
Impact
Priority
Recommended Action
Owner
Due Date
Escalation Trigger
```

Then provide:

```text
1. Overall assessment
2. Top three management priorities
3. Decisions required
4. Information still missing
```

The output format should reflect the intended audience.

---

# 11. Assumptions and Information Gaps

Require missing information to be visible.

### Template

```text
Do not invent missing project information.

Clearly separate:

- Confirmed facts
- Assumptions
- Information gaps
- Recommendations

If an important conclusion cannot be reached because information
is missing, state what information is required.
```

---

# 12. Risk and Dependency Check

Where relevant, require the AI to consider:

```text
Schedule impact
Budget impact
Scope impact
Quality impact
Resource impact
Technical impact
Security impact
Vendor impact
Stakeholder impact
Dependency impact
Operational impact
```

Not every category needs to appear in every prompt.

---

# 13. Quality Review

Before finalising the result, require a quality check.

### Template

```text
QUALITY REVIEW

Before finalising:

- identify contradictions,
- identify unsupported assumptions,
- flag missing information,
- ensure recommendations are actionable,
- ensure ownership is clear,
- check whether proposed actions address root causes,
- highlight conclusions requiring independent validation.
```

---

# 14. Human Review

Define where professional judgement remains mandatory.

### Template

```text
HUMAN REVIEW REQUIRED

The AI-generated output is decision support only.

The Project Manager or accountable stakeholder must validate
the output before it influences:

- budget,
- scope,
- contracts,
- project commitments,
- risk acceptance,
- staffing,
- executive reporting,
- production release,
- security decisions,
- or go-live approval.
```

---

# 15. Confidentiality and Data Protection

Before using the prompt, remove or anonymise:

- personal data,
- customer-identifying information,
- passwords,
- credentials,
- API keys,
- confidential financial data,
- commercially sensitive pricing,
- protected contract information,
- security-sensitive architecture,
- proprietary source code where restricted.

Use placeholders where appropriate.

Examples:

```text
Client A
Vendor B
Project X
€XM programme
External API provider
Critical production system
```

---

# 16. Standards and Framework Alignment

Each prompt should identify relevant standards or practices only where they genuinely apply.

### Template

```text
## Standards / Framework Alignment

PMI / PMP relevance:
[RELEVANT DOMAIN OR COMPETENCY]

PMBOK relevance:
[RELEVANT PRINCIPLE / PERFORMANCE AREA]

Delivery framework:
[Agile / Scrum / Kanban / Predictive / Hybrid / Framework-neutral]

Additional practices:
[Testing / DevOps / Risk / Product / Governance / Other]
```

Avoid claiming:

- PMI approval,
- PMP certification of the prompt,
- or formal compliance unless independently verified.

Use wording such as:

> "Aligned with relevant PMI/PMP project-management concepts."

---

# 17. Example Input

Include one short fictional or anonymised project example.

```text
Project:
Customer Self-Service Portal

Current phase:
System Integration Testing

Current status:
Amber

Planned UAT:
Three weeks

Known issue:
External payment API certification is 10 working days behind plan.

Dependencies:
UAT requires successful API certification.

Open defects:
2 Critical
8 High
19 Medium
```

---

# 18. Example Output

Keep the example concise.

| Issue | Impact | Action | Owner |
|---|---|---|---|
| API certification delay | UAT start at risk | Agree recovery plan with vendor and evaluate controlled test workaround | Integration Lead |
| Critical defects | Readiness risk | Prioritise resolution and retest before UAT entry decision | QA Lead |

---

# 19. Prompt Metadata

Every prompt should include:

```text
Prompt ID:
Category:
Version:
Status:
Owner:
Reviewer:
Created:
Last Reviewed:
Project Type:
Delivery Approach:
Risk Level:
AI Model Tested:
```

### Recommended Status Values

```text
Draft
Tested
Reviewed
Approved
Retired
```

---

# 20. Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial version |
| 1.1 | YYYY-MM-DD | Improved analysis criteria |
| 1.2 | YYYY-MM-DD | Added governance controls |

---

# Standard Prompt Flow

Every reusable prompt should broadly follow:

```text
BUSINESS PROBLEM
        ↓
PROFESSIONAL ROLE
        ↓
TASK
        ↓
PROJECT CONTEXT
        ↓
FRAMEWORK-SPECIFIC CONTEXT
        ↓
REQUIRED ANALYSIS
        ↓
DECISION CRITERIA
        ↓
OUTPUT FORMAT
        ↓
ASSUMPTIONS / INFORMATION GAPS
        ↓
QUALITY REVIEW
        ↓
HUMAN GOVERNANCE
```

---

# Key Principle

A professional prompt is not valuable because it is long or complex.

It is valuable when it consistently helps the Project Manager produce an output that is:

**relevant → structured → evidence-based → actionable → reviewable → governable.**
