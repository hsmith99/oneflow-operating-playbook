---
name: "Move-In SOP (v1.1) – Final Edited"
repository: "One Flow Operating Playbook Repository"
linked_agents: ["Flow SOP Reviewer Agent"]
last_updated: "2025-10-18"
---

# Move-In SOP (v1.1)

## Goals
| **Type** | **Goal** |
|-----------|-----------|
| **Operational** | Deliver a seamless, standardized Move-In process across all Flow communities with clear ownership, defined readiness gates, and cross-functional coordination between Leasing, Operations, Maintenance, and Housekeeping. |
| **Experiential** | Make every Neighbor feel personally welcomed, supported, and integrated into their community within 30 days of moving in. The first day should feel calm, personal, and celebratory. |

---

## Scope
Applies to **all long-term residential leases (≥ 3 months)** recorded in **Yardi Voyager** as `apartment_lease` or equivalent long-term record type across all Flow-managed U.S. properties.  
Excludes short-stay, hotel, and condo operations covered under the *Stay* Journey SOPs.

---

## Roles & Responsibilities
**Process Owner:** **Assistant General Manager (AGM)** – accountable for the end-to-end Move-In outcome.  
**Deputy:** **Operations Manager** (where staffed) or **Front Desk Lead**.

| **Role** | **Responsibilities** |
|-----------|----------------------|
| **Leasing Agent** | Owns all pre–move-in steps: verifying requirements, scheduling, elevator booking, and sending the Welcome Email. Co-leads the unit walkthrough and marks completion in Moved before handoff. |
| **Move-In Experience Agent** | Acts as Move-In Advocate: prepares unit touches (gift, card, keys), conducts check-ins at 48 hours and Week One, and ensures the Neighbor’s integration milestones are achieved within 30 days using Sigma dashboards. |
| **Assistant General Manager (AGM)** | Chairs weekly Move-In readiness meetings, resolves blockers across functions, verifies readiness in Moved/Yardi, and approves “Go” status prior to key release. |
| **Operations Manager / Front Desk Lead** | Manages day-of logistics, elevator operations, and issue triage through Zendesk and Slack. Acts as on-duty executive for after-hours or weekend move-ins. |
| **Front Desk Team** | Greets and orients Neighbors, confirms access, assists with parking and elevator use, logs issues in Zendesk, and updates #front-desk Slack channel. |
| **Maintenance** | Completes punch list and readiness inspection 48 hours before arrival, uploads photos in Moved, and confirms utilities and appliances operational. |
| **Housekeeping** | Conducts final clean and staging 24 hours before arrival, confirms “Unit Ready” status in Moved, and places Welcome Gift if delegated. |
| **Community Engagement Lead (CEL)** | Coordinates introductions (Ambassador Coffee), Flow Group invites, and ensures inclusion in the New Neighbor Event within 30 days. |

**Escalation Ladder:**  
Front Desk → Operations Manager/Front Desk Lead → AGM → GM → Regional Operations.

---

## Systems & Tools
| **System** | **Purpose** |
|-------------|-------------|
| **Yardi Voyager** | Lease and unit management; source of truth for payments, deposits, and readiness status. |
| **Moved** | Move-In checklists and coordination; integrates nightly with Yardi. Prevents key release until all requirements are marked complete. |
| **Carson / Flow App** | Access control, amenity reservations, deliveries, and Neighbor-facing onboarding. |
| **Zendesk** | Support ticketing and escalation tracking. |
| **Sigma** | Analytics platform displaying Design Your Flow survey data for personalization and integration tracking. |
| **Google Calendar** | Shared resource calendar for elevator scheduling. |

**Integration Notes:**  
- Yardi → Moved (nightly sync).  
- Typeform → Sigma (Design Your Flow responses).  
- Carson ↔ Flow App (access + amenity setup).

---

## Triggers
- **Primary Trigger:** Signed lease in Yardi Voyager.  
- **System Chain:** Yardi syncs overnight → Moved checklist auto-generates → Welcome Email triggers → tasks assigned to Leasing, Housekeeping, Maintenance, and Operations.  
- **Fail-Safe:** If sync fails by 8 AM local, Leasing manually creates Moved record and alerts AGM.  
- **Readiness Gate:** Keys cannot be released until Moved shows all requirements complete and AGM approves “Go.”

---

## Process
| **#** | **Step / Action** | **System(s)** | **Operator Experience** | **Neighbor Experience** |
|---:|--------------------|---------------|--------------------------|--------------------------|
| 1 | Verify pre–move-in requirements complete | Yardi, Moved | Leasing confirms deposits, rent, and insurance; updates status in Moved. | Receives checklist confirmation email. |
| 2 | Send Welcome Email + Portal Access | Moved | Leasing triggers Welcome Email template with checklist and building info. | Receives clear timeline and portal access. |
| 3 | Schedule Move-In Date + Elevator | Google Calendar, Moved | Leasing books elevator slot; posts to Slack #front-desk. | Receives confirmation with logistics and parking details. |
| 4 | Assign Move-In Advocate | Moved, Sigma | AGM assigns Advocate; Advocate reviews Design Your Flow data in Sigma. | Receives intro message from their Advocate. |
| 5 | Conduct Unit Readiness Inspection (48h) | Moved, Yardi | Maintenance & Housekeeping confirm punch and cleanliness; upload photos. | Confident unit is spotless and functional. |
| 6 | Prepare Keys + Access + Welcome Gift (24h) | Carson, Moved | Advocate stages Welcome Gift and card, tests access credentials. | Finds personalized gift waiting in unit. |
| 7 | Day-of Arrival Greeting + Orientation | Carson, Zendesk | Front Desk greets Neighbor, confirms Moved Ready, provides access. | Feels warmly welcomed and supported. |
| 8 | Unit Walkthrough + Key Handoff | Moved, Yardi | Leasing + Advocate walkthrough; resolve issues; confirm satisfaction. | Feels confident, at home, and supported. |
| 9 | Complete Move-In Confirmation | Moved, Yardi | Leasing marks checklist complete; AGM verifies no open items. | Receives notification of completion. |
| 10 | 48-Hour Check-In + Micro-Survey | Zendesk, Sigma | Advocate messages Neighbor, logs feedback, routes issues. | Appreciates proactive care. |
| 11 | Week-One Coffee + Introductions | Sigma, Carson | Advocate schedules coffee, connects to Ambassadors and Flow Groups. | Begins building relationships. |
| 12 | 30-Day Integration Review | Sigma | AGM + Advocate confirm Neighbor attended event or joined group; log completion. | Feels fully integrated into community. |

---

## Required Artifacts (Leasing → Operations Handoff)
Attached within **Moved** prior to key release:  
1. Lease, deposit, rent, insurance proof  
2. Unit Ready confirmation (photos, punch list)  
3. Elevator booking confirmation  
4. Carson access provisioned  
5. Design Your Flow summary (Sigma link)

---

## Quality Standards & Metrics
| **Category** | **Metric** | **Target** |
|---------------|------------|-------------|
| **Compliance** | All Move-In requirements complete prior to keys. | 100% |
| **Readiness** | Unit marked Ready ≥ 48h pre-arrival. | 100% |
| **Timeliness** | Average arrival-to-keys time. | ≤ 15 minutes |
| **Reliability** | Move-Ins with no day-of escalation. | ≥ 98% |
| **Experience** | 48-hour satisfaction score. | ≥ 90% positive |
| **Integration** | New Neighbors joined ≥1 Flow Group or event by Day 30. | ≥ 80% |

---

## Move-In Experience Agent Preparation Checklist (Typeform Draft)

**Purpose:** Ensure Move-In Experience Agent completes all preparation tasks for seamless Neighbor integration and move-in day execution.

### Preparation Checklist:

#### Personalization Review
- [ ] **Design Your Flow Data Reviewed** - Accessed Sigma dashboard and reviewed Neighbor's survey responses
- [ ] **Welcome Gift Selected** - Chose appropriate gift based on Neighbor's interests and preferences
- [ ] **Personalized Card Written** - Crafted warm, personal welcome message referencing their interests
- [ ] **Special Requests Noted** - Documented any specific accommodations or preferences from survey

#### Access & Logistics Preparation
- [ ] **Digital Keys Tested** - Verified Carson access credentials work properly
- [ ] **Elevator Booking Confirmed** - Confirmed scheduled time slot in Google Calendar
- [ ] **Parking Assignment Verified** - Confirmed parking spot and prepared access instructions
- [ ] **Move-In Day Timeline Shared** - Sent detailed logistics email to Neighbor

#### Community Integration Planning
- [ ] **Flow Groups Identified** - Reviewed Neighbor interests and matched to relevant Flow Groups
- [ ] **Ambassador Connections** - Identified appropriate Ambassadors for introductions
- [ ] **Welcome Event Scheduled** - Confirmed Neighbor's inclusion in upcoming New Neighbor Event
- [ ] **Coffee Meeting Planned** - Scheduled Week-One coffee with relevant community members

#### Communication & Follow-up Setup
- [ ] **Neighbor Notified** - Sent confirmation message with move-in day details
- [ ] **Team Briefed** - Updated Front Desk and Operations on any special considerations
- [ ] **Follow-up Scheduled** - Set calendar reminder for 48-hour check-in
- [ ] **Integration Milestones Set** - Planned 30-day integration goals and checkpoints

### Completion Requirements:
- All items must be checked before move-in day
- Neighbor must receive comprehensive preparation communication
- Team must be fully briefed on special accommodations
- Community integration plan must be documented in Sigma

---

## Resources & Templates
- Welcome Email Template (Moved)  
- Unit Readiness Checklist (Maintenance & Housekeeping)  
- Elevator Booking Calendar  
- Design Your Flow Survey (Typeform)  
- Sigma Dashboard – Move-In Personalization  
- New Neighbor Welcome Event SOP  
- One-Pager – Front Desk Move-In Quick Guide
- [Placeholder: Link to Move-In Experience Agent Preparation Checklist (Typeform)]

---

## Screenshots & Visuals
- Moved: Move-In Checklist view  
- Sigma: Integration Dashboard  
- Carson: Account Setup  

---

## Version Control
| **Author** | **Reviewer(s)** | **Version** | **Date** |
|-------------|------------------|--------------|-----------|
| Flow SOP Author Agent | Flow SOP Reviewer Agent | v1.0 | 2025-10-18 |
| Flow SOP Reviewer Agent | COO, GM, Front Desk, Neighbor Personas | v1.1 | 2025-10-18 |
| Harrison Smith | — | v1.2 (Pending Approval) | — |

---

> Delivering this SOP ensures that every Neighbor’s first day at Flow feels like coming home—not moving house.