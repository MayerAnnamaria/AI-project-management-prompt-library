# Basis of Estimate

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** PLAN-004 | **Category:** Project Planning

---


## 1. Ready-to-Use Prompt

**Purpose:** Establish a transparent, evidence-based cost estimate to support project budgeting, financial risk management, and investment decisions.

**Use case:** Evaluate cost assumptions, vendor quotations, contingency, and budget completeness when preparing funding requests, revising estimates, or reviewing major scope changes.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager specializing in project
cost estimation, resource planning, vendor management,
financial risk management, and project governance.

CONTEXT

Project: [PROJECT NAME]
Business objective: [OBJECTIVE]
Project phase: [PHASE]
Delivery approach: [AGILE / SCRUM / KANBAN / PREDICTIVE / HYBRID]
Estimate maturity: [EARLY / PRELIMINARY / DEVELOPED / BASELINED]
Scope maturity: [DETAILS]
Target completion: [DATE]
Currency: [CURRENCY]

COST DATA

Internal labour: [VALUE / BASIS]
External development: [VALUE]
Software licences: [VALUE]
Cloud / infrastructure: [VALUE]
Integrations: [VALUE]
Data migration: [VALUE]
Testing / QA: [VALUE]
Security / compliance: [VALUE]
Training / change management: [VALUE]
Vendor / consultancy: [VALUE]
Project management / PMO: [VALUE]
Operational transition: [VALUE]
Contingency: [VALUE / %]
Other costs: [VALUE]
Total estimated budget: [VALUE]

ESTIMATING BASIS

Methods: [VENDOR QUOTES / RATE CARDS / HISTORICAL DATA /
EXPERT JUDGMENT / BOTTOM-UP / PARAMETRIC / ANALOGOUS /
CAPACITY-BASED / OTHER]

Known assumptions: [LIST]
Known exclusions: [LIST]
Financial risks: [LIST]
Cost drivers: [LIST]
Approval requirements: [IF KNOWN]

TASK

Create a professional Basis of Estimate from the available information.

1. Summarize the estimated budget, scope, maturity, and cost basis.
2. Identify the estimating method supporting each major cost category.
3. Validate cost calculations and reconcile totals, identifying
   missing, duplicated, or insufficiently defined cost areas.
4. Assess estimate confidence (High / Medium / Low) and uncertainty.
5. Document material financial assumptions, validation needs,
   and potential impacts if assumptions are incorrect.
6. Evaluate contingency against identified risks, scope maturity,
   and uncertainty; recommend retaining or reassessing it.
7. Identify exclusions and classify potential future,
   operational, or unresolved project costs.
8. Analyze key cost drivers and scenarios affecting the forecast.
9. Identify financial risks, vendor dependencies, currency exposure,
   and potential budget overruns.
10. Adapt estimates to the delivery approach and distinguish
    committed costs from forecasts and uncertain future scope.
11. Identify missing financial information and required validation.
12. Recommend management actions, approval requirements,
    and decisions before budget authorization.

Do not invent costs, rates, percentages, or financial assumptions.
Do not recommend unsupported contingency levels.
Distinguish confirmed, estimated, and unverified financial data.

OUTPUT FORMAT

1. ESTIMATE OVERVIEW
   Project | Scope | Estimate Maturity | Currency |
   Base Cost | Contingency | Total Estimate

2. ESTIMATING METHODOLOGY
   Cost Area | Method | Source / Evidence | Confidence

3. COST COMPOSITION & CONFIDENCE
   Cost Area | Estimate | Basis | Confidence | Main Uncertainty
   Include a reconciled total.

4. KEY ASSUMPTIONS
   Assumption | Cost Impact if Incorrect |
   Validation Owner | Review Date

5. CONTINGENCY REVIEW
   Amount / % | Uncertainty Drivers | Adequacy Assessment |
   Recommendation | Rationale

6. EXCLUSIONS & BUDGET GAPS
   Exclusion / Missing Cost | Classification |
   Potential Impact | Required Clarification | Owner | Priority

7. FINANCIAL RISKS & COST DRIVERS
   Risk / Driver | Change Scenario | Potential Cost Impact |
   Recommended Response | Owner

8. ESTIMATE MATURITY
   Scope Maturity | Confidence | Missing Evidence |
   Recommended Re-estimation Trigger

9. MANAGEMENT ACTIONS
   Action / Decision | Priority | Proposed Owner |
   Required Evidence | Approval Authority | Target Date

MANAGEMENT SUMMARY

- Total estimate and reconciliation status
- Three most significant financial uncertainties
- Contingency recommendation
- Missing costs and approval blockers
- Decisions required before budget approval

Use concise Markdown tables.
Mark unknown values as "Not yet defined".
Label proposed owners, forecasts, and approvals as unconfirmed.
```

---

## 2. Quality Check

Apply this control after generating the Basis of Estimate.

```text
QUALITY CHECK

Act as a Senior QA Manager and review the Basis of Estimate.

Verify:

1. Accuracy: Calculations, subtotals, contingency, and totals reconcile.
2. Completeness: Relevant cost categories, exclusions, taxes,
   currency exposure, and financial dependencies are assessed.
3. Evidence: Estimating methods, sources, assumptions, and
   confidence levels are documented and justified.
4. Risk: Major cost drivers, uncertainties, and contingency
   rationale are identified without unsupported precision.
5. Consistency: Scope, resource assumptions, delivery approach,
   cost forecasts, and estimate maturity are aligned.
6. Governance: Budget decisions, approval requirements,
   and accountable stakeholders are identified.
7. Actionability: Financial gaps have clear corrective actions,
   priorities, and proposed owners.

OUTPUT

Quality verdict: PASS / REVISE

Provide:
- Findings requiring correction
- Required corrective actions
- Budget approval blockers

Do not invent costs, calculations, contractual terms, or approvals.
Flag financial conclusions requiring independent validation.
```

---

## 3. Practical IT Use Case

### Cloud Infrastructure Migration — Budget Approval

**Scenario:** A company plans to migrate business applications from on-premises infrastructure to a cloud platform. The Project Manager must consolidate cost estimates, evaluate vendor and infrastructure assumptions, and determine whether the budget is sufficiently reliable for approval.

### Project Context

| Attribute | Details |
|---|---|
| Project | Cloud Infrastructure Migration |
| Phase | Solution Design |
| Delivery approach | Hybrid |
| Estimate maturity | Preliminary |
| Target completion | 30 September 2027 |
| Currency | EUR |
| Estimated budget | €580,000 |
| Key dependencies | Migration vendor, network connectivity, security approval, cloud capacity |
| Management decision | Determine whether the estimate supports preliminary budget approval |

### Example Input

```text
Project: Cloud Infrastructure Migration
Business objective: Migrate business applications to a cloud platform.
Project phase: Solution Design
Delivery approach: Hybrid
Estimate maturity: Preliminary
Target completion: 30 September 2027
Currency: EUR

Costs:
Internal project team: €120,000
External migration vendor: €210,000
Cloud infrastructure: €75,000
Security and compliance: €45,000
Testing and validation: €40,000
Training and transition: €30,000
Contingency: €60,000

Total estimated budget: €580,000

Estimating basis:
- Internal labour: Internal rate cards and planned effort
- Migration vendor: Preliminary vendor quotation
- Cloud infrastructure: Preliminary consumption forecast
- Security and testing: Expert estimates
- Training: Internal planning estimate

Known assumptions:
- Existing applications are compatible with the cloud platform.
- Migration can be completed without major application redesign.
- Network connectivity is sufficient.
- Cloud consumption remains within forecast levels.

Known exclusions:
- Post-migration operational support
- Future application modernization
- Additional third-party software licences

Known financial risks:
- Application compatibility issues
- Higher-than-expected cloud consumption
- Additional migration effort
- Security remediation requirements
```

### Example Output — Basis of Estimate

#### 1. Estimate Overview

The preliminary estimate is **€580,000**, covering internal resources, vendor migration services, cloud infrastructure, security, testing, training, and contingency.

| Component | Amount |
|---|---:|
| Base estimated cost | €520,000 |
| Contingency | €60,000 |
| **Total estimate** | **€580,000** |

**Reconciliation:** PASS — supplied cost categories sum to the stated total. Cost completeness remains subject to review.

#### 2. Estimating Methodology

| Cost Area | Estimating Method | Confidence |
|---|---|---|
| Internal labour | Rate card and planned effort | Medium (provisional) |
| Migration vendor | Preliminary quotation | Medium (provisional) |
| Cloud infrastructure | Consumption forecast | Low (provisional) |
| Security and testing | Expert estimate | Low (provisional) |
| Training | Internal planning estimate | Low (provisional) |

*Confidence assessments are illustrative and require supporting evidence.*

#### 3. Cost Composition & Confidence

| Cost Area | Estimate | Basis | Main Uncertainty |
|---|---:|---|---|
| Internal labour | €120,000 | Planned effort | Resource availability |
| Migration vendor | €210,000 | Preliminary quote | Final scope and contract |
| Cloud infrastructure | €75,000 | Consumption forecast | Actual usage |
| Security / compliance | €45,000 | Expert estimate | Remediation effort |
| Testing | €40,000 | Expert estimate | Compatibility defects |
| Training / transition | €30,000 | Planning estimate | Training needs |
| Contingency | €60,000 | Proposed allowance | Risk exposure |
| **Total** | **€580,000** | | |

#### 4. Key Assumptions

| Assumption | Cost Impact if Incorrect | Proposed Validation Owner | Review Date |
|---|---|---|---|
| Applications are cloud-compatible | Additional development and testing | Solution Architect | TBD |
| No major redesign is needed | Increased vendor and internal labour costs | Technical Lead | TBD |
| Network capacity is sufficient | Additional infrastructure investment | Infrastructure Lead | TBD |
| Cloud usage follows forecast | Higher operational and project costs | Cloud Architect | TBD |

#### 5. Contingency Review

| Item | Assessment |
|---|---|
| Current contingency | €60,000 |
| Percentage of base cost | 11.5% |
| Primary uncertainties | Migration complexity, cloud usage, security remediation |
| Adequacy | Not yet validated |
| Recommendation | Reassess before budget approval |

**Rationale:** The contingency cannot be confirmed as sufficient until application compatibility, vendor scope, and cloud consumption assumptions are validated.

#### 6. Exclusions & Budget Gaps

| Exclusion / Gap | Classification | Potential Impact | Required Clarification | Priority |
|---|---|---|---|---|
| Post-migration support | Operational cost | Future operating budget | Confirm support funding | High |
| Application modernization | Future project cost | Additional investment | Confirm scope boundary | High |
| Third-party licences | Excluded / unresolved cost | Potential licence expenditure | Validate licence requirements | High |
| Data transfer and egress | Unassessed cost | Additional cloud charges | Confirm consumption model | Medium |
| Taxes and currency exposure | Unassessed financial factor | Potential budget variance | Confirm pricing basis | Medium |

#### 7. Financial Risks & Cost Drivers

| Risk / Driver | Change Scenario | Potential Impact | Proposed Response |
|---|---|---|---|
| Application compatibility | Redesign becomes necessary | Additional effort and cost | Complete compatibility assessment |
| Cloud consumption | Usage exceeds forecast | Higher recurring costs | Validate usage assumptions |
| Vendor scope | Additional migration work required | Contract cost increase | Confirm scope and change control |
| Security remediation | New vulnerabilities identified | Additional implementation cost | Complete security assessment |

*Financial impacts have not been quantified because supporting estimates are unavailable.*

#### 8. Estimate Maturity

| Assessment Area | Status |
|---|---|
| Estimate maturity | Preliminary |
| Scope maturity | Not confirmed |
| Overall confidence | Not validated |
| Missing evidence | Final vendor quotation, compatibility assessment, cloud usage model |
| Re-estimation trigger | Completion of technical discovery or material scope change |

#### 9. Recommended Management Actions

| Action / Decision | Priority | Proposed Owner | Required Evidence | Target Date |
|---|---|---|---|---|
| Validate migration complexity | High | Solution Architect | Compatibility assessment | TBD |
| Confirm vendor costs | High | Vendor Manager | Final quotation | TBD |
| Validate cloud forecast | High | Cloud Architect | Consumption model | TBD |
| Reassess contingency | High | Project Manager / Finance | Updated risk and cost analysis | TBD |
| Confirm budget authority | High | Project Sponsor | Funding approval requirements | TBD |

All proposed owners and deadlines require confirmation.

### Management Decisions

1. **Budget reliability:** Validate vendor pricing, application compatibility, and cloud consumption before approving the estimate as a delivery cost baseline.
2. **Contingency:** Review the €60,000 allowance against the documented financial risks and estimate maturity.
3. **Cost completeness:** Confirm funding treatment for operational support, additional licences, and unassessed infrastructure costs.
4. **Governance:** Establish financial approval authority, re-estimation triggers, and budget change-control requirements.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The cost breakdown reconciles to €580,000, but overall estimate confidence is not established. Several cost assumptions remain unverified, and exclusions may create additional financial commitments.

**Required corrections:**
- Validate the vendor quotation and technical scope.
- Confirm cloud consumption assumptions and additional cost categories.
- Assess financial risks and contingency adequacy.
- Establish budget approval authority and confirm accountable owners.

**Budget approval blockers:** Unverified estimate confidence, incomplete cost coverage, and unresolved financial risks.

**Governance:** This prompt supports relevant PMI-aligned practices in cost estimation, planning, uncertainty management, procurement, financial control, and project governance.

The Basis of Estimate is a financial decision-support artifact. Finance, Procurement, the Project Sponsor, and relevant technical stakeholders must validate material assumptions and costs before formal budget approval. Protect confidential rates, commercial terms, financial information, and supplier pricing.
