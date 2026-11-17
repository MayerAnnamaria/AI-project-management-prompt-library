# Basis of Estimate

## Purpose

Use this prompt to convert project cost data, vendor estimates, resource assumptions, and contingency into a professional Basis of Estimate.

The objective is to explain:

- how the estimate was created,
- what information it is based on,
- which assumptions affect the estimate,
- what is included,
- what is excluded,
- why contingency has been applied,
- and where financial uncertainty remains.

A strong Basis of Estimate should make the project budget easier to review, challenge, update, and govern.

---

## Best Used For

**Project phase:**  
Planning / Business Case / Budget Approval

**Project type:**  
Software implementation / Digital transformation / Data project / Cloud migration / Infrastructure / ERP / Product initiative

**Primary user:**  
Project Manager / Delivery Manager / PMO / Cost Owner / Finance Business Partner

**Delivery approach:**  
Predictive / Agile / Scrum / Kanban / Hybrid

**Recommended frequency:**  
At initial budgeting, major re-estimation points, scope changes, and governance reviews

---

# Prompt

```text id="boe-01"
ROLE

You are a senior IT Project Manager with experience in project
budgeting, vendor management, resource planning, commercial
governance, and international software delivery.

TASK

Create a professional Basis of Estimate from the project cost
information below.

PROJECT CONTEXT

Project:
[PROJECT NAME]

Business objective:
[OBJECTIVE]

Current phase:
[PHASE]

Delivery approach:
[PREDICTIVE / AGILE / SCRUM / KANBAN / HYBRID]

Estimate maturity:
[EARLY / PRELIMINARY / DEVELOPED / BASELINED]

Scope maturity:
[DETAILS]

Target completion:
[DATE]

Currency:
[CURRENCY]

COST DATA

Internal labour:
[VALUE / ASSUMPTIONS]

External development:
[VALUE]

Software licences:
[VALUE]

Cloud / infrastructure:
[VALUE]

Integration costs:
[VALUE]

Data migration:
[VALUE]

Testing / QA:
[VALUE]

Security / compliance:
[VALUE]

Training / change management:
[VALUE]

Vendor / consultancy costs:
[VALUE]

Project management / PMO:
[VALUE]

Operational transition:
[VALUE]

Contingency:
[VALUE / PERCENTAGE]

Other:
[VALUE]

Total estimated budget:
[VALUE]

ESTIMATING BASIS

[HISTORICAL DATA / VENDOR QUOTATIONS / RATE CARDS /
EXPERT ESTIMATE / BENCHMARK / BOTTOM-UP ESTIMATE / OTHER]

KNOWN ASSUMPTIONS

[LIST]

KNOWN EXCLUSIONS

[LIST]

KNOWN FINANCIAL RISKS

[LIST]

OUTPUT FORMAT

Create a professional Basis of Estimate with:

1. Estimate Overview
2. Estimating Methodology
3. Cost Composition
4. Key Assumptions
5. Contingency Rationale
6. Exclusions
7. Financial Risks and Uncertainty
8. Estimate Maturity
9. Recommended Management Actions
```

---

# Estimating Methodology

The prompt should identify which estimating methods support each major cost category.

Possible methods include:

```text id="boe-methods"
Vendor quotation
Internal rate card
Historical project data
Benchmark estimate
Expert judgement
Bottom-up estimate
Parametric estimate
Analogous estimate
Contracted rate
Capacity-based forecast
```

Do not imply that all cost values have the same level of confidence.

---

# Cost Confidence Review

For each major cost area, provide:

| Cost Area | Estimate | Estimating Basis | Confidence | Main Uncertainty |
|---|---:|---|---|---|

Recommended confidence scale:

```text id="boe-confidence"
High
Medium
Low
```

Example:

| Cost Area | Estimate | Basis | Confidence | Main Uncertainty |
|---|---:|---|---|---|
| CRM licences | €180,000 | Vendor quotation | High | User-volume change |
| Development | €420,000 | Vendor rate card + effort estimate | Medium | Requirements maturity |
| Data migration | €120,000 | Expert estimate | Low | Unknown data quality |

---

# Key Assumptions

Every material financial assumption should be explicit.

Examples:

```text id="boe-assumptions"
Team size remains stable.
Vendor day rates remain unchanged.
Existing cloud infrastructure can be reused.
No major source-system redesign is required.
Data cleansing remains within planned effort.
Required licences are available under current enterprise agreements.
Business users are available for UAT.
No additional regulatory requirements emerge.
```

For each assumption provide:

| Assumption | Cost Impact if Incorrect | Validation Owner | Review Date |
|---|---|---|---|

---

# Contingency Rationale

Contingency should not appear as an unexplained percentage.

Explain what uncertainty it is intended to cover.

Possible drivers include:

- immature requirements,
- uncertain integration effort,
- incomplete architecture,
- unknown data quality,
- vendor uncertainty,
- resource availability,
- security requirements,
- changing scope,
- regulatory uncertainty,
- schedule compression.

Use:

```text id="boe-contingency"
CONTINGENCY REVIEW

Current contingency:
[VALUE / %]

Primary uncertainty drivers:
[LIST]

Estimate maturity:
[LEVEL]

Scope maturity:
[LEVEL]

Recommendation:
[RETAIN / REVIEW / REDUCE / INCREASE / REASSESS]

Rationale:
[EXPLANATION]
```

Do not recommend a contingency percentage without supporting project evidence.

---

# Exclusions

Explicit exclusions help prevent future budget misunderstandings.

Examples may include:

```text id="boe-exclusions"
Post-go-live operating costs
Future feature development
Additional hardware not yet identified
Third-party change requests
New regulatory requirements
Business-as-usual staffing
Extended hypercare
Unplanned data remediation
Additional licences caused by user growth
```

For every exclusion, consider whether it represents:

- accepted out-of-scope cost,
- future project cost,
- operational cost,
- or unresolved financial risk.

---

# Example Input

```text id="boe-example-input"
Project:
CRM Replacement

Current Phase:
Solution Design

Delivery Approach:
Hybrid

Estimate Maturity:
Preliminary

Currency:
EUR

Costs:
Internal project team — €300,000
Implementation vendor — €620,000
CRM licences — €180,000
Data migration vendor — €140,000
Integration development — €160,000
Testing — €90,000
Training and change management — €70,000
Cloud infrastructure — €40,000
Contingency — €160,000

Total:
€1,760,000

Estimating Basis:
Implementation vendor quotation
Internal rate cards
CRM licence quotation
Expert estimate for integrations and migration

Assumptions:
Customer data quality is acceptable.
Existing identity platform can be reused.
No major custom CRM development is required.

Exclusions:
Post-go-live operating support after hypercare.
Future CRM enhancements.
Additional third-party licences.
```

---

# Example Output Excerpt

## Estimate Overview

The preliminary project estimate is €1.76 million and includes implementation, internal delivery resources, software licensing, data migration, integrations, testing, training, cloud infrastructure, and contingency.

The estimate is currently based on a combination of vendor quotations, internal resource rates, and expert estimates. Confidence therefore varies across cost categories.

## Key Uncertainty

The highest financial uncertainty currently relates to data migration and integration effort because both depend on technical discovery and data-quality findings that are not yet complete.

## Contingency

The current contingency should be reviewed against the unresolved integration and data-migration risks before budget approval. It should not be treated as available delivery budget for additional scope.

---

# Budget Gap Analysis

After generating the Basis of Estimate, review the budget for missing cost areas.

```text id="boe-gap"
ROLE

You are a senior IT Project Manager performing a budget
completeness review.

TASK

Review the Basis of Estimate below and identify likely missing
or insufficiently defined cost categories.

[PASTE BASIS OF ESTIMATE]

Check for:

- licences,
- cloud costs,
- environments,
- infrastructure,
- data migration,
- integrations,
- security,
- testing,
- test data,
- vendor management,
- training,
- business change,
- deployment,
- hypercare,
- support transition,
- contingency,
- project management,
- PMO,
- travel for international teams,
- currency exposure,
- taxes where relevant.

OUTPUT FORMAT

Missing / Unclear Cost
Why It May Be Required
Potential Financial Impact
Clarification Required
Owner
Priority
```

---

# Cost Driver Analysis

Identify the factors most likely to move the estimate.

Provide:

| Cost Driver | Current Assumption | Change Scenario | Potential Impact | Owner |
|---|---|---|---|---|

Typical IT cost drivers include:

- delivery duration,
- vendor effort,
- number of integrations,
- data volume,
- data quality,
- number of environments,
- licence volumes,
- cloud consumption,
- testing effort,
- security requirements,
- amount of customisation.

---

# Agile / Scrum Considerations

Where relevant, estimate at the appropriate level.

Possible inputs include:

- stable team cost,
- expected delivery duration,
- vendor capacity,
- release horizon,
- product roadmap,
- cloud and licence costs.

Avoid pretending that every future backlog item can be estimated precisely at project initiation.

Instead, distinguish between:

```text id="boe-agile"
Committed / understood cost
Forecast cost
Uncertain future scope
Contingency
```

---

# Kanban Considerations

For flow-based delivery, cost forecasting may consider:

- stable team capacity,
- throughput,
- service demand,
- vendor capacity,
- operational cost,
- expected delivery horizon.

Do not convert every work item into a detailed upfront estimate where continuous flow is the actual delivery model.

---

# Predictive Considerations

The Basis of Estimate may link directly to:

- WBS,
- work packages,
- schedule,
- resource plan,
- procurement plan,
- cost baseline.

Ensure that cost categories can be traced back to approved project scope.

---

# Hybrid Considerations

For hybrid projects, separate:

```text id="boe-hybrid"
Fixed costs
+
Capacity-based delivery costs
+
Variable vendor costs
+
Contingency
```

This often provides a clearer financial model than treating every element as fixed.

---

# Quality Review

Before using the estimate for governance or budget approval, confirm:

- [ ] Estimate methodology is documented
- [ ] Scope assumptions are visible
- [ ] Cost categories are complete
- [ ] Exclusions are explicit
- [ ] Vendor estimates are identifiable
- [ ] Contingency has a rationale
- [ ] Estimate confidence is visible
- [ ] Financial risks are identified
- [ ] Unverified values are clearly labelled
- [ ] The total reconciles with the underlying cost data

---

# Governance Review

For significant budgets, identify:

```text id="boe-governance"
Decision required
Decision owner
Budget threshold
Approval level
Required evidence
Decision date
```

Examples:

- approve preliminary budget,
- approve contingency usage,
- approve vendor contract,
- approve additional scope,
- re-baseline project budget.

---

# Standards / Framework Alignment

## PMI / PMP Relevance

Relevant themes may include:

- estimating,
- financial management,
- planning,
- risk,
- procurement,
- governance,
- business value.

## PMBOK Relevance

This prompt supports:

- finance,
- planning,
- risk,
- scope,
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

Validate the Basis of Estimate with relevant stakeholders, including:

- Project Manager
- Finance
- Project Sponsor
- Procurement
- Delivery Lead
- Technical Lead
- Product Owner where relevant
- Vendor Manager
- PMO

AI can structure and challenge estimate logic.

It cannot validate whether a quoted amount, contractual rate, or financial assumption is correct unless verified source data is provided.

---

# Confidentiality

Cost information may be commercially sensitive.

Do not enter into public AI tools:

- confidential vendor rates,
- contract pricing,
- salary information,
- protected commercial terms,
- confidential budgets,
- procurement-sensitive information.

Use anonymised or scaled values where necessary.

---

# Prompt Metadata

```text id="boe-metadata"
Prompt ID: PLAN-004
Category: Project Planning
Version: 1.0
Status: Draft
Owner: Project Manager
Reviewer: Finance / Sponsor / PMO
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
| 1.0 | YYYY-MM-DD | Initial IT Basis of Estimate framework |
