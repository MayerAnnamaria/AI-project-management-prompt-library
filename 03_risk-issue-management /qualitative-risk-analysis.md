# Qualitative Risk Analysis

## Purpose

Use this prompt to assess and prioritise identified project risks using a consistent qualitative scoring model.

The objective is to determine:

- which risks require immediate management attention,
- which risks can be monitored,
- where mitigation should be prioritised,
- and whether residual exposure remains acceptable after planned responses.

Qualitative risk analysis should support management judgement, not replace it.

---

## Best Used For

**Project phase:**  
Planning / Delivery / Testing / Deployment

**Project type:**  
Software implementation / Digital transformation / Data / ERP / Infrastructure / Cloud / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / Risk Manager / PMO

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
After risk identification and during regular risk reviews

---

# Prompt

```text
ROLE

You are a senior IT Project Manager and risk-management specialist
experienced in international software delivery, digital transformation,
project governance, and technology risk.

TASK

Perform a qualitative risk analysis on the project risk list below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Target milestone:
[DATE / MILESTONE]

Risk tolerance:
[IF KNOWN]

SCORING MODEL

Likelihood:
1 = Rare
2 = Unlikely
3 = Possible
4 = Likely
5 = Very Likely

Impact:
1 = Minimal
2 = Minor
3 = Moderate
4 = Major
5 = Severe

Risk Score:
Likelihood × Impact

Risk Rating:
1–4 = Low
5–9 = Medium
10–16 = High
17–25 = Critical

RISK LIST

[PASTE UNSCORED RISKS]

OUTPUT FORMAT

Provide:

Risk ID
Risk Description
Likelihood
Impact
Risk Score
Risk Rating
Risk Proximity
Primary Impact Area
Priority Rank
Scoring Rationale
Recommended Management Focus

Then provide:

1. Highest-priority risks
2. Overall risk profile
3. Immediate management actions
4. Risks requiring escalation
5. Information gaps affecting confidence in the scores
```

---

# Scoring Principles

Risk scoring should be evidence-based.

Do not assign scores only because a risk sounds serious.

Consider:

```text
Historical evidence
Current project data
Dependency status
Vendor performance
Schedule proximity
Technical complexity
Available mitigation
Recovery capability
Stakeholder impact
Security / compliance exposure
```

Where evidence is insufficient, state that confidence in the score is limited.

---

# Likelihood Assessment

Use:

```text
1 — Rare
Event is highly unusual in the current project context.

2 — Unlikely
Event could occur but current evidence suggests low probability.

3 — Possible
Event could reasonably occur.

4 — Likely
Current indicators suggest the event is more likely than not.

5 — Very Likely
Strong indicators suggest the event is expected unless action is taken.
```

---

# Impact Assessment

Do not assess impact only against schedule.

Consider:

```text
Schedule
Budget
Scope
Quality
Security
Compliance
Operations
Customer
Reputation
Business Value
```

The overall impact rating should reflect the most material credible consequence.

---

# Example

```text
Risk:
Business users may not be available for UAT.

Likelihood:
4 — Likely

Impact:
4 — Major

Score:
16

Rating:
High

Rationale:
Business availability has not yet been confirmed, and UAT sits
directly on the path to the committed release date.
```

---

# Risk Proximity

Add proximity to improve prioritisation.

Use:

```text
Immediate:
Less than 2 weeks

Near-term:
2–6 weeks

Medium-term:
6–12 weeks

Long-term:
More than 12 weeks
```

A High risk that may materialise next week may require more attention than a Critical risk that is several months away and already well controlled.

---

# Priority Ranking

Do not rank risks solely by score.

Consider:

```text
Risk Score
+
Proximity
+
Dependency Impact
+
Recovery Difficulty
+
Business Impact
+
Security / Compliance Exposure
+
Decision Urgency
```

Example:

| Risk | Score | Proximity | Priority |
|---|---:|---|---|
| UAT resource shortage | 12 | Immediate | 1 |
| Vendor API delay | 16 | Near-term | 2 |
| Cloud cost increase | 12 | Long-term | 4 |

---

# Heat Map Commentary

After scoring, provide a concise management interpretation.

Include:

```text
Which risks are concentrated in High / Critical zones?

Which risk categories dominate?

Are several risks linked to the same dependency?

Which risks require governance attention?

Where is management intervention most urgent?
```

Example:

> The current risk profile is dominated by integration, testing, and vendor dependencies. The highest management priority should be the identity-provider delay because it affects multiple downstream activities and has limited schedule recovery time.

---

# Heat Map Summary

Present the current distribution:

| Rating | Number of Risks | Management Approach |
|---|---:|---|
| Critical | X | Immediate escalation / response |
| High | X | Active mitigation and frequent review |
| Medium | X | Monitor and manage |
| Low | X | Periodic review |

This is a summary, not a substitute for the detailed register.

---

# Prompt 2 — Residual Risk Analysis

After mitigation actions are defined, re-score the risk.

```text
ROLE

You are a senior project risk manager assessing residual project risk.

TASK

Re-score the risks below assuming the listed mitigation actions
have been fully implemented.

For each risk compare:

- inherent / pre-mitigation risk,
- mitigation actions,
- residual likelihood,
- residual impact,
- residual score,
- residual rating.

OUTPUT FORMAT

Risk
Initial Rating
Mitigation
Residual Likelihood
Residual Impact
Residual Score
Residual Rating
Residual Exposure Acceptable?
Further Action Required?
```

---

# Inherent vs Residual Risk

## Inherent Risk

Exposure before planned mitigation.

## Residual Risk

Exposure remaining after mitigation is implemented.

Example:

```text
Initial:
Likelihood 4 × Impact 5 = 20 Critical

After mitigation:
Likelihood 2 × Impact 5 = 10 High
```

The impact may remain severe even when mitigation significantly reduces likelihood.

---

# Mitigation Effectiveness Review

Do not automatically reduce scores because actions exist.

Ask:

```text
Has the mitigation actually been implemented?

Is there evidence that it is effective?

Has likelihood genuinely changed?

Has impact genuinely changed?

Is the action preventive or only reactive?
```

Only reduce the residual score when there is a defensible reason.

---

# Example Input

```text
R-01
External identity provider may miss API certification.

R-02
Business users may not be available for UAT.

R-03
Critical integration defects may remain unresolved before release.

R-04
Data migration quality may be below the agreed acceptance threshold.

R-05
Security approval may not complete before go-live.
```

---

# Example Output

| Risk | L | I | Score | Rating | Priority |
|---|---:|---:|---:|---|---:|
| Identity-provider delay | 4 | 4 | 16 | High | 1 |
| UAT availability | 4 | 4 | 16 | High | 2 |
| Integration defects | 3 | 5 | 15 | High | 3 |
| Data migration quality | 3 | 4 | 12 | High | 4 |
| Security approval delay | 3 | 5 | 15 | High | 5 |

Priority order should then be explained using proximity and dependency impact, not only numerical score.

---

# Scoring Confidence

For each risk, optionally assign:

```text
High confidence
Medium confidence
Low confidence
```

Low confidence may result from:

- missing data,
- unclear dependencies,
- unvalidated assumptions,
- unreliable vendor information,
- insufficient historical evidence.

Use:

| Risk | Score | Confidence | Missing Evidence |
|---|---:|---|---|

---

# Agile / Scrum Considerations

Useful evidence may include:

- backlog volatility,
- team capacity,
- blocked items,
- defect trends,
- release dependencies,
- technical debt,
- Sprint / iteration performance.

Do not treat iteration-level variation automatically as project risk.

---

# Kanban Considerations

Flow metrics may support qualitative assessment.

Examples:

```text
WIP increasing
Cycle time worsening
Work item age increasing
Throughput declining
Repeated blocked work
SLE breaches increasing
```

These signals may justify revisiting likelihood or proximity.

---

# Predictive Considerations

Relevant evidence may include:

- critical-path exposure,
- milestone variance,
- procurement delay,
- schedule float,
- budget tolerance,
- resource availability.

---

# Hybrid Considerations

Combine formal project risk scoring with delivery-level evidence.

Example:

```text
Delivery signal
↓
Risk reassessment
↓
Updated score
↓
Management action
↓
Governance escalation if required
```

---

# Escalation Review

Flag risks where:

```text
Rating is Critical
Risk exceeds agreed tolerance
Risk threatens a committed milestone
Security or compliance exposure is material
Mitigation exceeds PM authority
Risk affects several workstreams
Residual exposure remains High or Critical
```

---

# Quality Checklist

Before accepting the analysis, confirm:

- [ ] Risks have been clearly defined
- [ ] Likelihood is justified
- [ ] Impact is justified
- [ ] Score calculation is correct
- [ ] Priority is not based only on score
- [ ] Proximity is considered
- [ ] Dependencies are considered
- [ ] Confidence in scoring is visible
- [ ] Residual risk is assessed separately
- [ ] Mitigation effectiveness is evidenced
- [ ] Escalation thresholds are considered

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- qualitative risk analysis,
- uncertainty,
- prioritisation,
- risk responses,
- monitoring,
- governance,
- escalation.

## PMBOK Relevance

This prompt supports:

- risk,
- planning,
- measurement,
- governance,
- delivery.

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

Risk scoring should be reviewed with:

- Risk Owner
- Project Manager
- relevant technical or business experts
- PMO / Risk function where applicable
- Sponsor where risk exceeds tolerance

AI can structure and challenge scoring logic.

It should not independently determine organisational risk appetite or final risk acceptance.

---

# Confidentiality

Avoid exposing:

- security vulnerabilities,
- confidential commercial exposure,
- supplier financial concerns,
- personal performance information,
- sensitive customer or regulatory information.

Anonymise project data where required.

---

# Prompt Metadata

```text
Prompt ID: RISK-003
Category: Risk & Issue Management
Version: 1.0
Status: Draft
Owner: Project Manager / Risk Manager
Reviewer: Risk Owners / PMO
Project Type: IT / Digital Transformation
Delivery Approach: Framework-neutral
Risk Level: High
AI Model Tested:
Last Reviewed:
```

---

# Version History

| Version | Date | Change |
|---|---|---|
| 1.0 | YYYY-MM-DD | Initial qualitative risk-analysis framework |
