# Iterative Refinement Workflow

**Prompt ID:** AIWF-003 | **Category:** Advanced AI Workflows | **Version:** 1.0 | **Status:** Draft

## 1. Ready-to-Use Prompt

**Purpose:** Improve AI-generated project-management documents through controlled critique, factual correction, and audience-focused refinement.

**Use case:** Refine status reports, executive summaries, risk statements, Steering Committee papers, change requests, requirements, vendor escalations, and stakeholder communications.

Copy the master prompt and replace the placeholders. Execute each stage sequentially, reviewing the output before continuing.

### Master Prompt — Iterative Refinement

```text
ROLE

You are a Senior IT Project Manager and PMO Quality Reviewer
experienced in project governance, executive reporting,
risk management, and stakeholder communication.

CONTEXT

Project: [PROJECT NAME]
Document type: [STATUS REPORT / DECISION PAPER / RISK REGISTER / OTHER]
Project phase: [PHASE]
Target audience: [EXECUTIVE / PMO / DELIVERY TEAM / USER]
Document purpose: [PURPOSE]
Decision required: [IF APPLICABLE]
Approved facts and metrics: [LIST]
Relevant quality criteria: [IF AVAILABLE]

DRAFT

[PASTE CURRENT DOCUMENT]

OBJECTIVE

Improve the document's clarity, evidence, precision,
actionability, executive relevance, and conciseness
without changing verified project facts.

Complete the following stages sequentially.
Stop after each stage for Project Manager review.

STAGE 1 — CRITIQUE

1. Identify the five most material weaknesses.
2. Review:
   - Vague or ambiguous statements
   - Unsupported claims or RAG assessments
   - Missing metrics and evidence
   - Unclear risks, dependencies, and impacts
   - Weak actions, owners, or deadlines
   - Missing decisions and escalation requirements
   - Excessive detail or repetition
3. Explain why each weakness matters.
4. Identify additional information needed.
5. Do not rewrite the document yet.

OUTPUT

Weakness | Evidence / Document Reference |
Why It Matters | Missing Information |
Recommended Correction | Priority

STAGE 2 — EVIDENCE-BASED REWRITE

After the critique has been reviewed, use:

Approved corrections: [PASTE]
Additional verified information: [PASTE]

1. Correct the material weaknesses.
2. Incorporate only confirmed new information.
3. Separate facts, forecasts, assumptions, and recommendations.
4. Make risks, actions, owners, and decisions explicit.
5. Preserve original project commitments unless
   verified corrections have been supplied.
6. Identify remaining evidence gaps.

OUTPUT

Revised Document — Version 2
Corrections Made
Information Still Missing

STAGE 3 — EXECUTIVE REFINEMENT

Refine Version 2 for the intended audience.

1. Remove repetition and unnecessary background.
2. Reduce length by approximately 20% where feasible.
3. Preserve all material:
   - Facts and metrics
   - Risks and dependencies
   - Actions and accountability
   - Decisions and deadlines
   - Important assumptions and qualifications
4. Use concise, factual, professional language.
5. Make business impact and decisions immediately visible.
6. Avoid defensive, vague, or overly technical wording.
7. Do not introduce new project information.

OUTPUT

Final Refined Document — Version 3
Material Information Preserved
Remaining Weaknesses

STAGE 4 — FINAL QUALITY VALIDATION

Compare Versions 1, 2, and 3.

Check:
- Factual accuracy
- Evidence and traceability
- Internal consistency
- Actionability
- Decision readiness
- Audience suitability
- Unintended changes or omissions

OUTPUT

Quality Verdict: PASS / REVISE
Version Comparison
Remaining Corrections
Approval Blockers

RULES

- Do not invent project facts, metrics, owners, or dates.
- Do not turn assumptions into confirmed statements.
- Do not replace missing evidence with confident wording.
- Do not remove material information solely to shorten text.
- Do not claim decisions or approvals were granted.
- Stop refining when further edits add no material value.
- Keep final approval with the authorized project owner.
```

### Optional Targeted Refinement

Use this short prompt when a document needs only one focused improvement rather than the full workflow.

```text
Act as a Senior IT Project Manager.

Review the document below for [CLARITY / EVIDENCE /
ACTIONABILITY / TONE / CONCISENESS / DECISION READINESS].

[PASTE DOCUMENT]

Identify the three most important weaknesses.
Rewrite only the affected content.

Preserve all confirmed facts, metrics, decisions,
and deadlines.

Return:
1. Main Weaknesses
2. Revised Text
3. Changes Made
4. Remaining Evidence Gaps
```

---

## 2. Quality Check

Use this independent check to validate the final refined document against the original.

```text
QUALITY CHECK

Act as an independent Senior PMO Quality Assurance Manager.

Review:
- Original Draft — Version 1
- Revised Draft — Version 2
- Final Refined Draft — Version 3
- Approved corrections and source evidence

Verify:

1. Accuracy:
   Confirmed facts, figures, and dates remain correct.

2. Evidence:
   Material statements and management conclusions
   have appropriate supporting information.

3. Traceability:
   Every substantive change can be explained
   by a verified correction or quality improvement.

4. Assumptions:
   Unconfirmed information remains clearly identified.

5. Actionability:
   Actions have clear expectations, owners,
   deadlines, or explicit information gaps.

6. Decision Readiness:
   Required decisions, business implications,
   and consequences of inaction are visible.

7. Clarity:
   The document avoids vague, ambiguous,
   defensive, or unnecessarily technical language.

8. Conciseness:
   Repetition is reduced without losing
   important nuance or project commitments.

9. Consistency:
   No contradictory metrics, owners,
   milestones, or risk assessments were introduced.

10. Governance:
    Final approval and unresolved issues
    remain visible.

OUTPUT

Quality Verdict: PASS / REVISE

Version Comparison:
Item | Original | Final |
Change | Evidence | Assessment

Findings: [REMAINING ISSUES]
Required Corrections: [ACTIONS]
Approval Blockers: [CRITICAL GAPS]

Optional Quality Score:
Rate Accuracy, Clarity, Evidence,
Actionability, and Executive Relevance
from 1–10 with brief justification.

Treat scores as subjective review indicators,
not objective quality measurements.

Do not invent missing evidence or approve
the document on behalf of stakeholders.
```

---

## 3. Practical IT Use Case

### CRM Replacement — Refining a Weekly Executive Status Report

**Scenario:** A Project Manager prepares a weekly CRM replacement status report. The initial draft is too vague for senior management: it claims progress is on track without evidence and does not clearly explain testing risks or required decisions.

The Project Manager uses three refinement rounds to improve the report before submission.

### Project Context

| Attribute | Details |
|---|---|
| Project | Enterprise CRM Replacement |
| Reporting type | Weekly Executive Status |
| Delivery approach | Hybrid |
| Overall status | Amber |
| Development progress | 82% actual vs. 85% planned |
| SIT pass rate | 91% |
| Open critical defects | Two Severity 1 |
| UAT forecast | Five working days late |
| Main dependency | Identity-provider certification |
| Budget actual vs. plan | €1.64M vs. €1.68M |
| Next milestone | UAT readiness review, 24 November 2026 |

### Example Input — Version 1

```text
Project update:

Things are generally progressing well,
although there have been some challenges.

Development is mostly on track.

There are some testing issues,
but the team is working on them.

Budget appears fine.

We will continue working on remaining items.

Overall status: Amber.
```

### Round 1 — Critique

| Weakness | Why It Matters | Recommended Correction |
|---|---|---|
| "Generally progressing well" | No measurable basis | Include planned vs. actual progress |
| "Some testing issues" | Hides quality exposure | State pass rate and critical defects |
| "Budget appears fine" | Not financially meaningful | Include actual and planned expenditure |
| Amber status unexplained | Weak governance reporting | Link status to schedule and quality risk |
| No clear management action | Executives cannot respond | Define recovery activities and decision trigger |

**Review finding:** The draft needs verified delivery facts before a professional rewrite can be completed.

### Round 2 — Add Verified Information and Rewrite

**Additional project data provided by the Project Manager:**

```text
Overall RAG: Amber

Development:
82% complete against 85% planned.

Testing:
SIT pass rate 91%.
Two Severity 1 defects remain open.

Schedule:
UAT forecast five working days late.

Cause:
Identity-provider certification delayed.

Budget:
€1.64M actual against €1.68M planned.

Recovery:
Mock authentication service implemented.
Testing resequenced.
Vendor escalation active.

Next milestone:
UAT readiness review — 24 November 2026.

Management decision:
Sponsor support required if vendor certification
is not confirmed by 20 November 2026.
```

**Rewritten Status Report — Version 2**

The Enterprise CRM Replacement project is **Amber**, primarily due to delayed identity-provider certification affecting testing readiness and the planned start of UAT.

Development is 82% complete against 85% planned. SIT currently has a 91% pass rate, with two Severity 1 defects remaining open. UAT is forecast to begin five working days later than planned.

Actual expenditure is €1.64M against €1.68M planned.

The project team has implemented mock authentication services, re-sequenced testing activities, and escalated the certification dependency to the vendor.

A UAT readiness review is scheduled for 24 November 2026. Sponsor support will be required if certification is not confirmed by 20 November.

### Round 3 — Executive Refinement

**Final Refined Version — Version 3**

<box border radius="lg" padding={3} gap={2}>
  <row align="center" justify="between">
    **Enterprise CRM Replacement — Weekly Status**

    <badge color="warning">Amber</badge>
  </row>
  **Executive Summary**

  UAT is forecast **five working days late** due to delayed identity-provider certification. Development is 82% complete against 85% planned, while SIT has reached a 91% pass rate with two Severity 1 defects still open.

  <table>
    <table-row><table-cell>Development</table-cell><table-cell>82% actual / 85% planned</table-cell></table-row>
    <table-row><table-cell>Testing</table-cell><table-cell>91% SIT pass rate; 2 Severity 1 defects</table-cell></table-row>
    <table-row><table-cell>Budget</table-cell><table-cell>€1.64M actual / €1.68M planned</table-cell></table-row>
    <table-row><table-cell>UAT</table-cell><table-cell>5 working days late (forecast)</table-cell></table-row>
  </table>
  **Recovery:** Mock authentication implemented, testing re-sequenced, and vendor escalation active.

  **Decision trigger:** Sponsor support required if certification remains unconfirmed by **20 November 2026**. The next UAT readiness review is scheduled for **24 November 2026**.
</box>

This version makes the schedule exposure, quality position, financial data, recovery measures, and escalation trigger immediately visible.

### Version Comparison

| Dimension | Version 1 | Version 3 |
|---|---|---|
| Project health | "Generally progressing well" | Amber with specific rationale |
| Development | "Mostly on track" | 82% actual vs. 85% planned |
| Testing | "Some issues" | 91% SIT pass; two Severity 1 defects |
| Budget | "Appears fine" | €1.64M actual vs. €1.68M planned |
| Schedule | Not provided | Five-working-day UAT forecast delay |
| Recovery | Generic activity | Specific mitigation actions |
| Decision | Not stated | Sponsor escalation trigger |
| Executive usefulness | Limited | Actionable and evidence-based |

### Management Decisions

1. **Schedule recovery:** Validate whether certification and unresolved Severity 1 defects will affect the 24 November readiness assessment.
2. **Vendor escalation:** Obtain a confirmed certification date and evidence supporting the recovery forecast.
3. **Quality governance:** Confirm defect ownership and closure requirements before UAT readiness approval.
4. **Executive decision:** Escalate for sponsor support if certification remains unconfirmed by 20 November.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The refined report substantially improves clarity, evidence, and decision relevance. Project figures remain consistent with the supplied data, and management attention is focused on the certification dependency and UAT readiness.

**Required corrections:** Confirm that the status uses the latest reporting-period data, validate remaining defect impacts, and verify the named sponsor decision route.

**Approval blockers:** Official publication remains subject to source-data validation and authorized project approval.

**Governance:** Supports PMI-aligned project monitoring, quality assurance, risk management, stakeholder communication, and decision support.

AI-assisted refinement improves document clarity and structure but does not replace verified project reporting or human approval. Do not enter confidential project, supplier, financial, or security information into AI systems unless organizational policy permits it.
