# Iterative Refinement Workflow

## Purpose

Use iterative refinement when an AI-generated project-management output is directionally correct but not yet good enough for professional use.

Instead of discarding the first draft and starting again, improve the output through controlled review cycles.

A simple workflow is:

```text id="refine-flow-01"
Draft
↓
Critique
↓
Rewrite
↓
Refine
↓
Final Quality Check
```

The objective is not to generate more text.

The objective is to progressively improve:

- clarity,
- evidence,
- precision,
- tone,
- decision usefulness,
- and conciseness.

---

## Best Used For

Iterative refinement works especially well for:

- status reports,
- executive summaries,
- decision papers,
- risk narratives,
- change requests,
- stakeholder communications,
- vendor escalations,
- project briefs,
- lessons learned,
- meeting outputs.

---

# Core Principle

Do not use:

```text id="refine-vague"
Make this better.
```

Use:

```text id="refine-specific"
Identify exactly what is weak.

Explain why it is weak.

Correct those weaknesses.

Then review again against a defined quality standard.
```

---

# Three-Round Model

```text id="refine-rounds"
Round 1
Critique

Round 2
Rewrite

Round 3
Refine and Quality Check
```

---

# Round 1 — Critique the Draft

Start by asking the AI to identify specific weaknesses.

```text id="refine-round1"
ROLE

You are a senior IT Project Manager and PMO quality reviewer.

TASK

Review the project status summary below and identify its five
biggest weaknesses.

Be specific.

Check for:

- vague statements,
- unsupported RAG status,
- missing metrics,
- unclear risks,
- unclear actions,
- missing owners,
- missing decision requirements,
- weak executive relevance.

DRAFT

[PASTE DRAFT]

OUTPUT FORMAT

Weakness
Why It Matters
What Information Is Missing
Recommended Improvement
```

---

# Example Weak Draft

```text id="refine-weak-example"
Project update:

Things are generally progressing well, although there have been
some challenges.

Development is mostly on track.

There are some testing issues, but the team is working on them.

Budget appears fine.

We will continue working on the remaining items next week.

Overall status is Amber.
```

---

# Likely Critique

A quality review should identify issues such as:

```text id="refine-likely-issues"
"Mostly on track"
→ No evidence.

"Some testing issues"
→ Issue not defined.

"Budget appears fine"
→ No actual / forecast data.

Amber
→ No stated reason.

"We will continue working"
→ No specific next actions.
```

---

# Critique Before Rewrite

This sequence is important.

Avoid jumping directly to:

```text id="refine-direct"
Rewrite this professionally.
```

because the AI may improve wording without fixing the underlying project-management gaps.

Use:

```text id="refine-analysis-first"
Diagnose
↓
Correct
```

---

# Round 2 — Rewrite With Better Evidence

After reviewing the critique, supply missing information.

Example:

```text id="refine-round2"
Good.

Now rewrite the status report addressing all five weaknesses.

Use the confirmed information below.

PROJECT

Enterprise CRM Replacement

Overall Status:
Amber

Development:
82% complete against 85% planned.

Testing:
SIT pass rate is 91%.
Two Severity 1 defects remain open.

Schedule:
UAT is forecast five working days late.

Cause:
Identity-provider certification is delayed.

Budget:
Actual spend is €1.64M against €1.68M planned.

Recovery:
Mock authentication service implemented.
Testing has been resequenced.
Vendor escalation is active.

Next milestone:
UAT readiness review on 24 November.

Decision required:
Sponsor support is required if vendor certification is not confirmed
by 20 November.

OUTPUT FORMAT

Overall Status
Progress
Schedule
Quality
Cost
Risks / Issues
Recovery
Next Steps
Decision Required

Do not introduce information not provided above.
```

---

# Round 2 Objective

The output should move from:

```text id="refine-round2-before"
General language
```

to:

```text id="refine-round2-after"
Evidence-based management commentary
```

---

# Example

### Weak

> Testing has had some challenges.

### Stronger

> SIT pass rate is 91%, with two Severity 1 defects remaining open. UAT readiness remains dependent on closure of both defects and completion of identity-provider certification.

---

# Round 3 — Refine the Improved Version

Once the content is strong, refine the presentation.

```text id="refine-round3"
Good.

Now review the rewritten status report once more.

TASK

1. Remove repetition.
2. Reduce the length by approximately 20%.
3. Preserve every material project fact.
4. Make the tone suitable for senior management.
5. Make required decisions immediately visible.

Then provide:

Final Version

Quality Rating:
1–10

Rating Justification:
Maximum 3 sentences

Remaining Weaknesses:
If any.
```

---

# Why the Final Round Matters

A document can be accurate but still ineffective because it is:

- too long,
- repetitive,
- defensive,
- overly technical,
- poorly prioritised.

The final round optimises communication quality.

---

# Refinement Dimensions

Use targeted instructions.

---

# 1. Clarity

```text id="refine-clarity"
Identify any sentence that could be interpreted in more than one way.

Rewrite it to be unambiguous.
```

---

# 2. Evidence

```text id="refine-evidence"
Identify every material claim that lacks evidence.

For each, state what evidence or metric would strengthen it.
```

---

# 3. Conciseness

```text id="refine-concise"
Reduce this document by 25%.

Remove:

- repetition,
- background the audience already knows,
- unnecessary adjectives,
- low-value detail.

Do not remove:

- decisions,
- risks,
- actions,
- metrics,
- deadlines.
```

---

# 4. Tone

```text id="refine-tone"
Review the tone.

Identify language that is:

- defensive,
- emotional,
- apologetic,
- aggressive,
- vague.

Rewrite it to be factual, calm, and confident.
```

---

# Example

### Defensive

```text id="refine-defensive"
Unfortunately, the vendor has once again failed to provide the
necessary certification despite our repeated requests.
```

### Factual

```text id="refine-factual"
Vendor certification remains outstanding against the agreed
milestone and is now affecting the planned UAT start.
```

---

# 5. Executive Relevance

```text id="refine-executive"
You are the Executive Sponsor.

Remove information that does not support:

- understanding project health,
- understanding material risk,
- making decisions,
- confirming accountability.

Retain all information required for governance.
```

---

# 6. Actionability

```text id="refine-actionability"
Review every action in the document.

Check whether each has:

- a clear action,
- owner,
- deadline,
- intended outcome.

Flag any weak actions.
```

---

# 7. Decision Clarity

```text id="refine-decision"
Review the document from the perspective of the decision-maker.

Is it immediately clear:

- what decision is required,
- why it is required,
- by when,
- what happens if no decision is made?

Rewrite if necessary.
```

---

# Example — Refining a Risk Statement

### Round 0

```text id="refine-risk-0"
Vendor delay may affect project.
```

### Round 1

Critique:

```text id="refine-risk-1"
Which vendor?
Which deliverable?
What milestone?
What probability?
What impact?
```

### Round 2

```text id="refine-risk-2"
If the identity provider does not complete certification by
20 November, authentication testing may delay UAT by five working
days.
```

### Round 3

```text id="refine-risk-3"
Identity-provider certification remains the main UAT schedule risk.
Certification is required by 20 November to protect the current UAT
forecast.
```

The final version is shorter while preserving decision relevance.

---

# Example — Refining an Executive Update

### Draft

```text id="refine-exec-draft"
The team has been working very hard and has made good progress,
although unfortunately some challenges have arisen with the vendor
which are currently being investigated and managed.
```

### Critique

Problems:

```text id="refine-exec-critique"
"working very hard"
→ not project-health evidence

"good progress"
→ vague

"some challenges"
→ vague

"being investigated"
→ unclear accountability
```

### Refined

```text id="refine-exec-final"
Delivery remains Amber because identity-provider certification is
five working days late.

The vendor escalation is active, and the project team has
re-sequenced testing to protect the UAT milestone.
```

---

# Refinement for Steering Committee Papers

Use:

```text id="refine-steerco"
Review this Steering Committee paper.

ROUND 1
Identify:

- unclear decision,
- weak options,
- missing trade-offs,
- unsupported recommendation,
- excessive detail.

ROUND 2
Rewrite the paper addressing these gaps.

ROUND 3
Reduce the executive section to one page while preserving all
decision-critical information.
```

---

# Refinement for Vendor Escalations

```text id="refine-vendor"
ROUND 1
Identify emotional, blaming, or unsupported statements.

ROUND 2
Rewrite using only verified facts, project impact, required action,
and deadline.

ROUND 3
Review from the supplier's perspective and remove any wording that
creates avoidable ambiguity.
```

---

# Refinement for Requirements

```text id="refine-requirements"
ROUND 1
Identify ambiguity and missing acceptance criteria.

ROUND 2
Rewrite requirements to be clearer and testable.

ROUND 3
Review as QA Lead and identify anything that still cannot be
objectively verified.
```

---

# Refinement for Risk Registers

```text id="refine-risk-register"
ROUND 1
Identify vague risks and weak mitigation.

ROUND 2
Rewrite using cause-event-impact structure.

ROUND 3
Check whether mitigation actions reduce likelihood or impact and
whether owners are clear.
```

---

# Refinement for Meeting Minutes

```text id="refine-minutes"
ROUND 1
Identify decisions hidden in discussion and actions without owners.

ROUND 2
Restructure into decisions, actions, risks, and discussion.

ROUND 3
Remove unnecessary transcript-style detail.
```

---

# Refinement for User Communications

```text id="refine-user-comms"
ROUND 1
Identify jargon, unclear impact, and missing user action.

ROUND 2
Rewrite in plain language.

ROUND 3
Review from the end-user perspective and shorten while preserving
all actions and deadlines.
```

---

# Refinement Prompt Library

Useful targeted refinement instructions include:

```text id="refine-library"
Make the risk more specific.

Replace assumptions with questions.

Separate facts from interpretation.

Make the action measurable.

Make ownership explicit.

Remove blame.

Reduce technical detail.

Strengthen the executive summary.

Make the decision required explicit.

Cut repetition.

Add evidence.

Remove unsupported certainty.

Make deadlines visible.

Clarify the consequence of inaction.
```

---

# Avoid Generic Refinement Requests

Weak:

```text id="refine-generic-weak"
Improve this.
```

Better:

```text id="refine-generic-better"
The second paragraph is too defensive.

Rewrite it using:

- confirmed facts,
- current impact,
- action already taken,
- next decision required.

Do not apologise or blame the vendor.
```

---

# Quality Scoring

A quality score can be useful if the criteria are defined.

Example:

```text id="refine-score-prompt"
Rate this status report from 1–10 against:

1. Accuracy
2. Clarity
3. Evidence
4. Actionability
5. Executive relevance

Provide one score for each category.

Then identify the single biggest improvement still required.
```

---

# Example Scorecard

| Dimension | Score |
|---|---:|
| Accuracy | 9 |
| Clarity | 8 |
| Evidence | 8 |
| Actionability | 9 |
| Executive Relevance | 8 |

Do not treat AI-generated scores as objective performance metrics.

The value is in the critique behind the score.

---

# Stop Criteria

Do not refine endlessly.

Stop when:

```text id="refine-stop"
Facts are accurate

Message is clear

Evidence is sufficient

Required actions are explicit

Audience needs are met

Further editing adds little value
```

---

# Over-Refinement Risk

Too many rounds can:

- remove important nuance,
- introduce new assumptions,
- make language artificial,
- over-compress important information.

Use human judgement.

---

# Human-in-the-Loop Model

Use:

```text id="refine-hitl"
Draft
↓
AI Critique
↓
Human Adds Missing Facts
↓
AI Rewrite
↓
Human Review
↓
AI Final Polish
↓
Human Approval
```

The human supplies missing project truth.

The AI improves structure and communication.

---

# Fact Integrity Rule

Never allow refinement to change facts merely to make the document sound stronger.

Example:

Confirmed:

```text id="refine-fact-confirmed"
Release date is at risk.
```

Do not refine into:

```text id="refine-fact-bad"
Release date will be achieved.
```

unless evidence supports it.

---

# Version Comparison

For important outputs ask:

```text id="refine-version-compare"
Compare Draft V1 and Draft V2.

Identify:

- information removed,
- information added,
- factual changes,
- assumption changes,
- tone changes.

Flag anything material that changed unintentionally.
```

---

# Iterative Refinement Workflow

Recommended sequence:

```text id="refine-final-flow"
1. Generate Draft
2. Diagnose Weaknesses
3. Add Missing Facts
4. Rewrite
5. Refine for Audience
6. Reduce Unnecessary Detail
7. Quality Check
8. Human Approval
```

---

# Agile / Scrum Considerations

Use iterative refinement for:

- Sprint Review summaries,
- release updates,
- backlog descriptions,
- stakeholder messages.

The AI should not override team decisions or Product Owner priorities.

---

# Kanban Considerations

Refine:

- service-review commentary,
- bottleneck analysis,
- flow summaries,
- blocked-item escalations.

Keep metrics linked to management action.

---

# Predictive Considerations

Refine:

- milestone reports,
- variance narratives,
- formal change documents,
- executive reports.

---

# Hybrid Considerations

Refine both:

```text id="refine-hybrid"
Delivery evidence
+
Formal governance communication
```

---

# Quality Checklist

Before finalising an iteratively refined output, confirm:

- [ ] Weaknesses were identified before rewriting
- [ ] Missing facts were added by a reliable source
- [ ] Facts remain unchanged
- [ ] Assumptions remain visible
- [ ] Evidence supports major claims
- [ ] Tone fits the audience
- [ ] Actions are specific
- [ ] Decisions are clear
- [ ] Repetition has been removed
- [ ] Important nuance has not been lost
- [ ] Final version has human approval

---

# Key Principle

Iterative refinement is not:

```text id="refine-key-bad"
Generate
↓
Generate again
↓
Generate again
```

It is:

```text id="refine-key-good"
Draft
↓
Diagnose
↓
Correct
↓
Refine
↓
Validate
```

Each round should have a specific purpose.

---

# Prompt Metadata

```text id="refine-metadata"
Prompt ID: AIWF-003
Category: Advanced AI Workflows
Version: 1.0
Status: Draft
Owner: Project Manager / PMO
Reviewer: Project Manager
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: Low / Medium
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial iterative-refinement workflow |
