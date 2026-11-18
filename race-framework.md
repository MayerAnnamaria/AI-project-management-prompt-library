## 3. Practical IT Use Case

### Competing Priorities — Urgent Scope Change vs. Delivery Deadline

**Scenario:** An IT Project Manager is coordinating a CRM implementation scheduled for release in four weeks.

The Sales Director requests an additional reporting dashboard, arguing that it is business-critical. However, the development team is fully allocated, two high-priority defects remain unresolved, and the implementation vendor has an outstanding integration dependency.

The Project Manager must determine whether to accept, defer, or trade off the request without jeopardizing the release.

**Management challenge:** How should the Project Manager balance business value, delivery capacity, quality, and stakeholder expectations?

### Project Context

| Attribute | Current Position |
|---|---|
| Project | Enterprise CRM Implementation |
| Delivery approach | Hybrid / Agile development |
| Planned release | 4 weeks |
| Development capacity | 40 person-days available before release |
| Existing committed work | 35 person-days |
| Available capacity buffer | 5 person-days |
| New stakeholder request | Sales performance dashboard |
| Estimated additional effort | 12 person-days |
| Open defects | 2 High-priority defects |
| External dependency | Vendor API integration awaiting certification |
| Sponsor priority | Protect committed release date |

The new request exceeds the remaining capacity by **7 person-days**, even before considering additional defect remediation or integration delays.

### Example RACE Prompt

```text
ROLE

You are a Senior IT Project Manager experienced in
Agile and Hybrid delivery, stakeholder management,
scope control, capacity planning, and risk management.

ASK

Evaluate an urgent business change request competing
with existing delivery commitments.

Recommend the most appropriate management option
while balancing business value, schedule, quality,
team capacity, and project governance.

CONTEXT

Project: Enterprise CRM Implementation

Release deadline: 4 weeks

Delivery capacity:
40 person-days remaining.

Existing committed work:
35 person-days.

Available buffer:
5 person-days.

New stakeholder request:
Sales performance dashboard.

Estimated effort:
12 person-days.

Business justification:
Sales Director considers the dashboard
critical for the upcoming reporting cycle.

Current delivery risks:
- 2 unresolved High-priority defects
- Vendor API certification outstanding
- No additional development capacity confirmed

Sponsor priority:
Protect the agreed release date.

Decision authority:
Project Sponsor / Change Control Board,
according to project governance.

EXPECTED OUTPUT

1. Executive Summary
2. Capacity and Schedule Impact
3. Three Management Options
4. Comparison of Business Value, Risk, and Trade-offs
5. Recommended Option with Rationale
6. Stakeholder Communication Approach
7. Decision Required and Approval Owner

RULES

- Do not automatically accept the urgent request.
- Do not assume that all committed work has equal priority.
- Distinguish business urgency from technical necessity.
- Consider the impact on quality and existing commitments.
- Do not assume additional capacity is available.
- Flag unknown dependencies and estimation uncertainty.
- Separate the PM recommendation from formal approval.
- Do not invent project facts or commitments.
```

### Example AI Output

#### 1. Executive Summary

The requested Sales dashboard requires 12 person-days, while only 5 person-days remain unallocated before release.

The request therefore creates a minimum capacity shortfall of 7 person-days if added without replacing existing work. This excludes any further effort arising from defect resolution or vendor integration issues.

Accepting the request without re-prioritization would introduce avoidable schedule and quality exposure.

**Recommended approach:** Evaluate the dashboard for a later release unless the business owner can demonstrate that it is essential for the current launch. If it must be delivered now, identify and formally approve equivalent scope trade-offs.

#### 2. Capacity Impact

| Capacity Measure | Person-Days |
|---|---:|
| Total remaining capacity | 40 |
| Existing commitments | 35 |
| Available buffer | 5 |
| New dashboard estimate | 12 |
| Total demand if accepted | 47 |
| Capacity shortfall | 7 |

The calculation assumes the 35 person-days of existing work and the new 12-person-day estimate are comparable and that no work has been displaced.

#### 3. Management Options

| Option | Business Benefit | Delivery Impact | Main Risk |
|---|---|---|---|
| **A. Accept now** | Dashboard available at launch | Exceeds capacity by at least 7 days | Schedule slippage, quality pressure |
| **B. Defer to next release** | Value delivered later | Protects current baseline | Stakeholder dissatisfaction |
| **C. Reprioritize existing scope** | Potential delivery at launch | Requires removing or deferring other work | Loss of previously committed functionality |

**Option A — Accept without changing commitments**

Not recommended under the current capacity assumptions. The plan exceeds available capacity, and no additional resources or schedule extension have been approved.

**Option B — Defer the dashboard**

Preserves the existing release scope and allows the team to focus on committed delivery, defect resolution, and integration readiness.

The business impact of deferring the dashboard must still be assessed.

**Option C — Reprioritize existing scope**

Could accommodate the dashboard if at least 7 person-days of existing work can be removed or postponed. However, the Project Manager must confirm that the displaced work is genuinely deferrable and that the estimates remain valid.

#### 4. Recommended Management Decision

**Recommend Option B — Defer the dashboard, subject to business-impact validation.**

This option best aligns with the Sponsor's stated priority to protect the release date while maintaining attention on existing quality and integration risks.

However, the Sales Director's business justification should be assessed before reaching a final decision.

If the dashboard is essential for regulatory, contractual, or critical operational reasons, Option C should be considered through formal change control.

### 5. Stakeholder Communication

**Proposed message to the Sales Director**

> Thank you for highlighting the dashboard requirement. I understand its importance for the upcoming reporting cycle.
>
> Our current delivery plan has five person-days of available capacity, while the dashboard is estimated at twelve. Adding it without reprioritizing existing work would create a delivery shortfall and increase risk to the planned release.
>
> I recommend reviewing the business impact and assessing whether the dashboard can be scheduled for the next release. If delivery at launch is essential, we can evaluate which existing scope items could be deferred and present the trade-offs for approval.

This approach acknowledges business value without promising unapproved scope, capacity, or deadlines.

### 6. Required Management Actions

| Action | Proposed Owner | Required Outcome |
|---|---|---|
| Validate dashboard urgency and business impact | Sales Director / Product Owner | Confirm whether the request is launch-critical |
| Review effort estimate and dependencies | Development Lead | Validate the 12-person-day estimate |
| Identify potentially deferrable scope | Product Owner / Project Manager | Establish feasible trade-offs |
| Assess schedule and quality exposure | Project Manager / QA Lead | Quantify delivery impact |
| Present change options | Project Manager | Obtain an informed management decision |
| Approve scope or baseline changes | Authorized Change Authority | Record formal decision |

### 7. Decision Required

The Project Sponsor or designated Change Control Board must decide whether to:

- **Defer** the dashboard to a later release.
- **Approve scope substitution** after reviewing the displaced functionality.
- **Approve a revised delivery baseline** if additional scope is required without equivalent trade-offs.

No baseline change should be treated as approved until the authorized decision is recorded.

### Applied Quality Check

**Quality verdict: PASS — with management validation required**

The RACE prompt produces a decision-oriented assessment rather than a generic prioritization list. It includes capacity calculations, alternative options, delivery trade-offs, stakeholder communication, and approval responsibilities.

**Outstanding validation:**

- Confirm dashboard business criticality.
- Validate effort estimates and available capacity.
- Assess whether existing scope can safely be deferred.
- Confirm the effect of unresolved defects and vendor dependencies.
- Obtain formal approval for any scope or baseline change.

### Management Value

This example demonstrates five essential project-management competencies:

1. **Prioritization:** Distinguishing urgent stakeholder requests from essential delivery commitments.
2. **Impact analysis:** Quantifying capacity shortfalls and delivery exposure.
3. **Trade-off management:** Comparing business value, schedule, scope, and quality.
4. **Stakeholder management:** Explaining constraints constructively without creating unrealistic commitments.
5. **Governance:** Converting competing demands into an evidence-based decision for the appropriate authority.

**Key principle:** A Project Manager should not simply choose which stakeholder request sounds most urgent. Effective project management means **making trade-offs visible, protecting delivery commitments, and enabling informed decisions.**
