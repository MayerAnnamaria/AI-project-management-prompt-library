# Stakeholder Complaint Response

![Version](https://img.shields.io/badge/Version-0.0.1-44AFE2)
![Status](https://img.shields.io/badge/Status-Initial_Draft-FF9F1C)
![Validation](https://img.shields.io/badge/Validation-Pending-lightgrey)

**Prompt ID:** STAKE-004 | **Category:** Stakeholder Management

---


## 1. Ready-to-Use Prompt

**Purpose:** Prepare professional, factual, and empathetic responses to stakeholder complaints while ensuring clear accountability, corrective actions, and follow-up commitments.

**Use case:** Respond to formal concerns about IT service disruptions, project delays, system defects, poor communication, implementation failures, or vendor performance during delivery, deployment, or operational transition.

Copy the prompt and replace the placeholders with your project information.

```text
ROLE

You are a Senior IT Project Manager experienced in stakeholder
management, service recovery, difficult communication,
incident escalation, and international technology delivery.

CONTEXT

Project: [PROJECT NAME]
Project phase: [DELIVERY / TESTING / DEPLOYMENT / HYPERCARE]
Delivery approach: [AGILE / PREDICTIVE / KANBAN / HYBRID]
Stakeholder role: [ROLE]
Complaint category: [SERVICE / QUALITY / DELAY / COMMUNICATION / OTHER]
Complaint received: [DATE / TIME]
Response deadline: [DATE / TIME / NOT PROVIDED]

STAKEHOLDER COMPLAINT

[PASTE EXACT COMPLAINT]

INVESTIGATION AND RESPONSE DATA

Confirmed facts: [VERIFIED INFORMATION]
Unverified claims: [DETAILS]
Known business impact: [DETAILS]
Immediate cause: [IF CONFIRMED]
Root cause: [CONFIRMED / UNDER INVESTIGATION]
Confirmed process failures: [DETAILS]
Corrective actions completed: [LIST]
Investigation still required: [DETAILS]
Planned preventive actions: [LIST]
Next update commitment: [DATE / TIME]
Responsible contact: [ROLE / CHANNEL]
Relevant incident / issue reference: [IF AVAILABLE]
Required escalation or review: [DETAILS]

TASK

Prepare a professional stakeholder complaint response
and identify the necessary management follow-up.

STEP 1 — ASSESS THE COMPLAINT

1. Identify the stakeholder's main concerns and business impact.
2. Distinguish:
   - Verified facts
   - Confirmed failures
   - Unverified allegations
   - Ongoing investigations
3. Separate the complaint from the technical incident record.
4. Determine whether the issue requires escalation
   to Service Management, Security, Legal, Compliance,
   Communications, or executive governance.
5. Identify missing evidence before making conclusions.

STEP 2 — DRAFT THE RESPONSE

6. Acknowledge the concern and its operational impact.
7. Explain verified facts in clear, non-technical language.
8. Accept responsibility for confirmed process failures
   without making unsupported legal admissions.
9. Explain corrective actions already completed.
10. Describe ongoing investigations and next steps.
11. Provide a specific next-update commitment.
12. Include an appropriate stakeholder contact.
13. Maintain a professional, empathetic, accountable,
    factual, and non-defensive tone.

STEP 3 — DEFINE CORRECTIVE AND PREVENTIVE ACTIONS

14. Distinguish immediate service restoration from
    long-term root cause prevention.
15. Identify actions, responsible roles, and target dates.
16. Recommend process improvements for recurring issues.
17. Define the evidence needed to validate corrective actions.
18. Identify when stakeholder feedback or formal closure
    confirmation should be requested.
19. Update the complaint register and link relevant
    incident, issue, risk, or vendor records.

STEP 4 — VALIDATE COMMUNICATION QUALITY

20. Review the draft for:
    - Defensive or dismissive wording
    - Unsupported blame
    - Excessive technical detail
    - Unverified explanations
    - Vague corrective actions
    - Unrealistic promises
    - Missing update commitments
21. Recommend targeted revisions before distribution.

RULES

- Do not invent facts, causes, actions, dates, or commitments.
- Do not treat every complaint allegation as confirmed.
- Do not claim the root cause is known if investigation continues.
- Acknowledge impact without assuming contractual liability.
- Avoid assigning blame to individuals or vendors without evidence.
- Do not promise that an issue will never recur.
- Commit to an update date when resolution timing is uncertain.
- Escalate sensitive matters through organizational procedures.
- Keep confidential or personal information appropriately protected.

OUTPUT FORMAT

1. STAKEHOLDER RESPONSE — READY TO SEND

Subject: [SPECIFIC COMPLAINT REFERENCE]

Dear [STAKEHOLDER],

[Acknowledge complaint and operational impact]

[Summarize confirmed facts and explain what happened]

[Acknowledge confirmed process failures]

[Describe corrective actions already completed]

[Explain ongoing investigation and next steps]

[Provide next update date and responsible contact]

Kind regards,
[AUTHORIZED PROJECT REPRESENTATIVE]

2. COMPLAINT ASSESSMENT

Concern | Confirmed Facts | Unverified Information |
Business Impact | Required Investigation

3. CORRECTIVE AND PREVENTIVE ACTION PLAN

Action | Type | Proposed Owner |
Target Date | Verification Evidence | Status

Type:
Immediate Correction / Corrective Action /
Preventive Improvement

4. ESCALATION AND GOVERNANCE

Issue | Severity / Impact | Escalation Required |
Responsible Role | Linked Project Record

5. STAKEHOLDER FOLLOW-UP

Next Update | Responsible Contact |
Closure Criteria | Stakeholder Confirmation Required

6. COMPLAINT REGISTER ENTRY

Complaint ID | Category | Date Received |
Owner | Current Status | Resolution / Next Action

MANAGEMENT SUMMARY

- Main stakeholder concern
- Confirmed service or project failure
- Current corrective actions
- Remaining investigation gaps
- Next communication and escalation requirements

Use professional, concise language.
Separate stakeholder-facing text from internal management analysis.
```

---

## 2. Quality Check

Apply this independent review before issuing the response.

```text
QUALITY CHECK

Act as a Senior PMO Quality Assurance Manager
specializing in stakeholder communication and service recovery.

Review the response against the original complaint
and available investigation evidence.

Verify:

1. Accuracy: All factual statements are supported
   by the provided evidence.

2. Acknowledgment: The response recognizes the
   stakeholder's concern and actual business impact.

3. Accountability: Confirmed failures are acknowledged
   without unsupported blame or legal admissions.

4. Clarity: Technical explanations are understandable
   to the intended audience.

5. Corrective Actions: Completed actions are distinguished
   from planned or proposed improvements.

6. Commitments: Next steps, update deadlines, and
   responsible contacts are explicit and realistic.

7. Tone: Wording is professional, empathetic,
   non-defensive, and solution-oriented.

8. Escalation: Security, legal, regulatory, privacy,
   and other sensitive matters are appropriately flagged.

9. Governance: Complaint, incident, and corrective-action
   records remain traceable and consistent.

OUTPUT

Quality verdict: PASS / REVISE
Findings: [ISSUES REQUIRING CORRECTION]
Required corrections: [CORRECTIVE ACTIONS]
Unverified Statements: [FACTUAL GAPS]
Approval blockers: [CRITICAL UNRESOLVED ITEMS]

Do not invent facts, completed actions,
root causes, approvals, or response commitments.
```

---

## 3. Practical IT Use Case

### CRM Implementation — Service Interruption and Communication Failure

**Scenario:** During a CRM rollout, a production configuration change causes a service interruption. Customer service agents cannot access CRM records, and the project team fails to provide timely stakeholder communication.

The Customer Service Director submits a formal complaint. The Project Manager must acknowledge the operational impact, explain confirmed facts, describe immediate recovery actions, and commit to further updates.

### Project Context

| Attribute | Details |
|---|---|
| Project | CRM System Replacement |
| Phase | Deployment / Hypercare |
| Incident | CRM Service Interruption |
| Service interruption | 09:17–10:42 |
| Duration | 85 minutes |
| Main concern | Service availability and poor communication |
| Stakeholder | Customer Service Director |
| Response owner | Project Manager |
| Root cause | Under investigation |
| Management objective | Restore confidence and prevent repeated communication failures |

### Example Input

```text
Project: CRM System Replacement
Phase: Deployment / Hypercare

Complaint received:

"The CRM was unavailable for more than an hour
this morning without warning.

Our agents could not access customer records,
and we received no update from the project team
until after the service was restored.

This is the second communication problem
during this rollout."

Confirmed facts:

- CRM unavailable from 09:17 to 10:42.
- Interruption occurred after a production
  configuration change.
- CRM service has been restored.
- Planned stakeholder notification was not issued.
- Incident communication began at 10:15.
- Root cause review remains in progress.

Corrective actions completed:

- Configuration change reverted.
- Further production changes temporarily paused.
- Deployment checklist updated.
- Service Manager added to the approval process.

Next update:
15:00 CET on 18 November 2026.

Contact:
Project Manager / Service Manager.

Investigation gaps:
- Exact technical root cause
- Effectiveness of new approval controls
- Whether the alleged previous communication issue
  is documented
```

### Example Output — Stakeholder Complaint Response

#### 1. Stakeholder Response — Ready to Send

**Subject: Response to CRM Service Interruption and Communication Concerns**

Dear [Customer Service Director],

Thank you for raising your concerns regarding the CRM service interruption and the communication provided during the incident.

We recognize that the outage affected your team's ability to access customer information and that the lack of timely communication made the situation more difficult to manage.

Our investigation confirms that the CRM was unavailable between **09:17 and 10:42 CET**, following a production configuration change. Service has since been restored.

We have also confirmed that the planned stakeholder notification was not issued. This did not meet the expected communication process, and we recognize the need to address it.

As immediate corrective measures, the configuration change has been reverted, further production changes have been temporarily paused, and the deployment checklist has been updated. The Service Manager has also been added to the approval process.

The technical root cause investigation remains ongoing. We will provide a further written update by **15:00 CET on 18 November 2026**, including the investigation findings available at that time and any additional preventive actions.

If you would like to discuss the operational impact directly, please contact the Project Manager or Service Manager.

Thank you for bringing these concerns to our attention.

Kind regards,  
[Project Manager]

#### 2. Complaint Assessment

| Concern | Confirmed Position | Further Investigation |
|---|---|---|
| CRM outage | Service unavailable for 85 minutes | Detailed technical root cause |
| Business impact | Customer records inaccessible | Full operational impact |
| Missing notification | Planned notification not issued | Communication process failure |
| Incident communication | Started at 10:15 | Timeliness against required process |
| Previous communication failure | Stakeholder reports recurrence | Confirm historical records |

**Management assessment:** The complaint includes a confirmed service disruption and communication failure. The reported recurrence requires verification before being treated as an established pattern.

#### 3. Corrective and Preventive Action Plan

| Action | Type | Proposed Owner | Status |
|---|---|---|---|
| Revert affected configuration | Immediate Correction | Technical Lead | Completed |
| Restore CRM availability | Immediate Correction | Service Team | Completed |
| Pause further production changes | Containment | Project Manager | Completed |
| Update deployment checklist | Corrective Action | Project Manager | Completed |
| Add Service Manager to approval process | Corrective Action | Project Manager | Completed |
| Complete technical root cause analysis | Investigation | Technical / Service Lead | In Progress |
| Validate revised communication controls | Preventive Improvement | Service Manager | Proposed |
| Review historical complaints | Investigation | Project Manager | Proposed |

Proposed owners and planned improvements require confirmation.

#### 4. Escalation and Governance

| Issue | Potential Impact | Required Action | Linked Record |
|---|---|---|---|
| CRM outage | Operational disruption | Complete incident review | Incident Record |
| Missing notification | Stakeholder confidence | Verify process controls | Complaint Register |
| Production-change risk | Potential recurrence | Review change authorization | Change Register |
| Repeated communication concern | Escalation risk | Examine previous incidents | Complaint History |

**Governance principle:** The technical incident and stakeholder complaint should remain distinct but linked records.

#### 5. Stakeholder Follow-Up

| Item | Commitment |
|---|---|
| Next update | 18 November 2026, 15:00 CET |
| Responsible contact | Project Manager / Service Manager |
| Root cause review | In progress |
| Corrective-action validation | Required |
| Complaint closure | Pending investigation and follow-up |
| Stakeholder confirmation | To be requested after response |

The update deadline is a communication commitment, not a guaranteed root cause resolution date.

#### 6. Complaint Register Entry

| Field | Value |
|---|---|
| Complaint ID | To be assigned |
| Category | Service Disruption / Communication |
| Stakeholder | Customer Service Director |
| Owner | Project Manager |
| Status | Investigating / Response Drafted |
| Related incident | To be linked |
| Next action | Complete investigation and provide update |
| Closure status | Open |

### Management Decisions

1. **Service recovery:** Confirm that the restored CRM service remains stable and that appropriate monitoring is active.
2. **Communication control:** Validate the revised deployment notification and approval process.
3. **Root cause analysis:** Establish why the disruption occurred and whether additional preventive measures are required.
4. **Stakeholder confidence:** Provide the committed update and verify whether the stakeholder's concerns have been adequately addressed.

### Applied Quality Review

**Quality verdict: REVISE**

**Findings:** The response acknowledges the operational impact, communicates verified facts, and describes completed recovery actions. However, the root cause investigation remains incomplete, and the effectiveness of the revised communication controls has not yet been demonstrated.

**Required corrections:**
- Validate that the deployment checklist and approval changes are operational.
- Confirm the remaining root cause investigation timeline.
- Investigate the reported previous communication failure.
- Confirm complaint ownership and relevant escalation requirements.
- Review the final response with the appropriate Service or Business Manager.

**Approval blockers:** Unconfirmed effectiveness of preventive measures and incomplete investigation evidence for any definitive root-cause statements.

**Governance:** Supports PMI-aligned stakeholder engagement, communication management, issue resolution, conflict management, service recovery, and project governance.

Stakeholder complaint responses must be based on verified information and authorized communication commitments. AI cannot determine legal liability, regulatory obligations, or disciplinary responsibility. Protect confidential customer information, security details, incident records, and sensitive stakeholder communications.
