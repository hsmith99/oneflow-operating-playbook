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
Applies to **all residential leases (≥ 1 month)** recorded in **Yardi Voyager**.
Excludes short-stay, hotel, and condo operations covered under the *Stay* Journey SOPs.

---

## Roles & Responsibilities
**Process Owner:** **Assistant General Manager (AGM)** – accountable for the end-to-end Move-In outcome.  
**Deputy:** **Operations Manager** (where staffed) or **Front Desk Lead**.

| **Role** | **Responsibilities** |
|-----------|----------------------|
| **Leasing Agent** | Owns all pre–move-in steps: verifying requirements, scheduling, elevator booking, and sending the Welcome Email. Co-leads the unit walkthrough and marks completion in Moved before handoff. |
| **Move-In Experience Agent** | Acts as Move-In Advocate: prepares unit touches (gift, card, keys), conducts check-ins at 48 hours and Week One, and ensures the Neighbor’s integration milestones are achieved within 30 days using Sigma dashboards. |
| **Assistant General Manager (AGM)** | Runs weekly Move-In readiness meetings, resolves blockers across functions, verifies readiness in Moved/Yardi, and approves “Go” status prior to key release to Neighbors, ensuring that all requirements are met before the Neighbor moves in. |
| **Operations Manager / Front Desk Lead** | Manages day-of logistics, elevator operations, and issue triage through Zendesk and Slack. Acts as on-duty executive for after-hours or weekend move-ins. |
| **Front Desk Team** | Greets and orients Neighbors, helps to make keys, supports with 48 Check-ins, confirms access, assists with parking and elevator use, logs issues in Zendesk, and updates #fx and #move-ins Slack channels. |
| **Chief Engineer / Maintenance Manager** | Conducts pre-maintenance inspection, creates work orders in Waves, completes maintenance work, conducts post-maintenance inspection, updates Neighbor CRM. |
| **Maintenance Team** | Completes work orders assigned by Maintenance Manager in Waves, ensures all systems operational. |
| **Cleaning Company (Third-Party)** | Deep cleans unit per AGM instructions, completes cleaning typeform upon completion. |
| **Community Engagement Lead** | Coordinates introductions (Ambassador Coffee), Flow Group invites, and ensures inclusion in the New Neighbor Event within 30 days. |

**Escalation Ladder:**  
Front Desk → Operations Manager/Front Desk Lead → AGM → GM → Regional Operations.

**Weekend/After-Hours:** On-duty Front Desk Agent handles move-in operations with Operations Manager/Front Desk Lead backup. All move-in issues logged in Zendesk with "Move-In" tag.

---

## Move-In Experience Agent Alternative Structure

**When Move-In Experience Agent is not on the team, the following structure applies:**

### **Pre-Move-In Responsibilities (Leasing Agent)**
- **Leasing Agent** handles all steps through Day 1 (Steps 1-8)
- **Leasing Agent** conducts unit walkthrough and key handoff
- **Leasing Agent** completes move-in confirmation

### **Move-In Advocate Assignment**
- **Move-In Advocate** assigned from **Front Desk Team**
- **Move-In Advocate** should be the **Front Desk Agent working on move-in day**
- **Ideal timing:** Front Desk Agent scheduled during neighbor's move-in window
- **AGM** assigns Front Desk Agent as Move-In Advocate in Moved/Sigma

### **Post-Move-In Responsibilities (Move-In Advocate)**
- **Move-In Advocate** handles all post-Day 1 activities (Steps 10-12)
- **Move-In Advocate** conducts 48-hour check-in
- **Move-In Advocate** schedules Week 1 coffee chat during 48-hour check-in
- **Coffee chat options:**
  - Move-In Advocate conducts personally
  - Schedule with **GM** or **AGM**
  - Connect Neighbor with **Ambassador**
- **Move-In Advocate** follows up on community integration:
  - Encourage attendance at New Neighbor Event
  - Connect with other residents (if desired)
  - Promote community events and activities
  - Monitor integration progress through 30 days

### **Process Adjustments**
| **Step** | **Original Responsible** | **Alternative Responsible** |
|----------|-------------------------|------------------------------|
| 6 | Move-In Experience Agent | **Leasing Agent** |
| 8 | Leasing Agent + Move-In Experience Agent | **Leasing Agent** (solo) |
| 10 | Move-In Experience Agent | **Move-In Advocate** (Front Desk Agent) |
| 11 | Move-In Experience Agent + Community Engagement Lead | **Move-In Advocate** + **GM/AGM/Ambassador** |
| 12 | AGM + Move-In Experience Agent | **AGM** + **Move-In Advocate** |

---

## Systems & Tools
| **System** | **Purpose** |
|-------------|-------------|
| **Yardi Voyager** | Lease and unit management; source of truth for payments, deposits, readiness status, and document storage. All lease documents and artifacts uploaded to lease profile. |
| **Google Sheet - Neighbor CRM & Move-in Tracker** | Tracks all Neighbors, all Move-ins, and the status of each step in the Move-in process for each Neighbor. |
| **Moved** | Neighbor-facing Move-In checklist where tasks are completed by Neighbors and approved by Leasing Agents or Move-In Experience Leads as required. Integrates nightly with Yardi. Prevents key release until all requirements are marked complete. |
| **Carson / Flow App** | Access control, amenity reservations, deliveries, and Neighbor-facing onboarding. |
| **Zendesk** | Support ticketing and escalation tracking. |
| **Google Calendar** | Shared resource calendar for elevator scheduling. |
| **RingCentral** | Onsite calling mechanism for Prospect and Neighbor communications. |

**Integration Notes:**  
- Yardi → Moved (nightly sync).  
- Typeform → Sigma (Design Your Flow responses).  
- Carson ↔ Flow App (access + amenity setup).

---

## Triggers
- **Primary Trigger:** Signed lease in Yardi Voyager.  
- **System Chain:** Yardi syncs overnight → Moved checklist auto-generates → Welcome Email triggers → Neighbors added to Neighbor CRM & Move-in Tracker.
- **Readiness Gate:** Keys cannot be released until Moved shows all requirements complete and AGM approves Key Release.

---

## Process
| **#** | **Step / Action** | **Responsible Team Member** | **System(s)** | **Operator Experience** | **Neighbor Experience** |
|---:|--------------------|----------------------------|---------------|--------------------------|--------------------------|
| 1 | Verify pre–move-in requirements complete | **Leasing Agent** | Yardi, Moved | Leasing confirms deposits, rent, and insurance; updates status in Moved. | Receives checklist confirmation email. |
| 2 | Send Welcome Email + Portal Access | **Leasing Agent** | Moved | Leasing triggers Welcome Email template with checklist and building info. | Receives clear timeline and portal access. |
| 3 | Schedule Move-In Date + Elevator | **Leasing Agent** | Google Calendar, Moved | Leasing books elevator slot; posts to Slack #front-desk. | Receives confirmation with logistics and parking details. |
| 4 | Assign Move-In Advocate | **Assistant General Manager (AGM)** | Moved, Sigma | AGM assigns Advocate; Advocate reviews Design Your Flow data in Sigma. | Receives intro message from their Advocate. |
| 5 | Unit Turn/Make Ready Process (synchronous with steps 1-4) | **Chief Engineer / Maintenance Manager**, **AGM**, **Leasing Agent**, **Cleaning Company** | Waves, Typeform, Neighbor CRM, Slack | **Maintenance:** Pre-inspection → work orders in Waves → maintenance work → post-inspection. **Cleaning:** AGM coordinates with cleaning company via Slack → deep clean → cleaning typeform submission. **Inspection:** AGM and Leasing Agent complete final unit inspection typeforms. Status updates automatically to Neighbor CRM. | Unit ready before move-in
| 6 | Prepare Keys + Access + Welcome Gift (24h) | **Move-In Experience Agent** | Carson, Moved | Advocate stages Welcome Gift and card, tests access credentials. | Finds personalized gift waiting in unit. |
| 7 | Place Packages in Unit | **Leasing Agent** or **Move-In Experience Agent** | Neighbor CRM | Check for any packages received for Neighbor, place in unit before move-in. | Packages waiting in unit upon arrival. |
| 8 | Day-of Arrival Greeting + Orientation | **Front Desk Team** | Carson, Zendesk | Front Desk greets Neighbor, confirms Moved Ready, provides access. | Feels warmly welcomed and supported. |
| 9 | Unit Walkthrough + Key Handoff | **Leasing Agent** + **Move-In Experience Agent** | Moved, Yardi | Leasing + Advocate walkthrough; resolve issues; confirm satisfaction. | Feels confident, at home, and supported. |
| 10 | Complete Move-In Confirmation | **Leasing Agent** (with **AGM** verification) | Moved, Yardi | Leasing marks checklist complete; AGM verifies no open items. | Receives notification of completion. |
| 11 | 48-Hour Check-In | **Move-In Experience Agent** | RingCentral, Neighbor CRM | Advocate calls Neighbor via RingCentral phone call, logs feedback and notes in Neighbor CRM, routes issues to appropriate team. | Appreciates proactive care. |
| 12 | Week-One Coffee + Introductions | **Move-In Experience Agent** + **Community Engagement Lead** | Sigma, Carson | Advocate schedules coffee, connects to Ambassadors and Flow Groups. | Begins building relationships. |
| 13 | 30-Day Integration Review | **Assistant General Manager (AGM)** + **Move-In Experience Agent** | Sigma | AGM + Advocate confirm Neighbor attended event or joined group; log completion. | Feels fully integrated into community. |

---

## Unit Turn/Make Ready Process

The Unit Turn/Make Ready process runs **synchronously** with pre-move-in steps (Steps 1-4) and ensures the unit is ready before the Neighbor arrives. This process has three critical phases: **Maintenance**, **Cleaning**, and **Inspection**.

### **Maintenance**
1. **Pre-Maintenance Inspection:** Chief Engineer / Maintenance Manager inspects unit and creates work orders in Waves
2. **Work Order Completion:** Maintenance Team completes all work orders
3. **Post-Maintenance Inspection:** Chief Engineer / Maintenance Manager inspects completed work via Maintenance Inspection typeform

### **Cleaning**
1. **Daily Coordination:** AGM messages cleaning company via Slack with units to clean tomorrow
2. **Deep Clean:** Cleaning company performs comprehensive deep cleaning
3. **Confirmation:** Cleaning company completes Cleaning Completion typeform

### **Final Inspection**
1. **AGM Inspection:** AGM conducts post-cleaning inspection via Final Unit Inspection typeform
2. **Leasing Agent Inspection:** Leasing Agent conducts final pre-move-in inspection via Final Unit Inspection typeform
3. **Unit Ready Status:** AGM reviews all completed typeforms and updates unit status to "Ready" in Yardi

> 🔹 **Cross-Reference:** For complete details on this process, including typeform structures and quality standards, see [Unit Move-In Readiness SOP](unit-move-in-readiness-sop.md).  
> 🔹 **System Integration:** All typeform submissions automatically update Neighbor CRM & Move-in Tracker and post to Slack channels via Google Scripts.

---

## Required Artifacts (Leasing → Operations Handoff)

**Tracking & Approval:** Tasks completed by Neighbors and tracked in **Moved** (approved by Leasing Agents or Move-In Experience Leads as required).  
**Document Storage:** All documents and artifacts uploaded to **lease profile in Yardi Voyager**.

**Required Items Prior to Key Release:**
1. Lease, deposit, rent, insurance proof (uploaded to Yardi)  
2. Unit Ready confirmation (all typeform inspections complete - see Unit Readiness SOP)  
3. Welcome Gift and Note placed in unit  
4. Packages placed in unit (if received)  
5. Elevator booking confirmation  
6. Carson access provisioned  
7. Design Your Flow summary (Sigma link)

> 🔹 **Unit Readiness (Maintenance/Cleaning):** A unit is ready from a maintenance and cleaning perspective when:
> - All Waves work orders completed
> - Post-maintenance inspection passed (Maintenance Manager)
> - Cleaning completed and confirmed
> - Final inspections passed (AGM & Leasing Agent)
>
> 🔹 **Move-In Readiness:** A move-in is ready for move-in day when:
> - Unit is ready (see above)
> - Neighbor has completed all required tasks in Moved (approved by Leasing/Move-In Experience Leads)
> - All documents uploaded to Yardi lease profile
> - Welcome Gift and Note placed in unit
> - Packages placed (if any received)
> - Elevator booked
> - Carson access provisioned

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

## Move-In Experience Checklist

**Purpose:** Ensure Leasing Agents, Move-In Experience Agents, and Move-in Advocates complete all preparation tasks for seamless Neighbor integration and move-in day execution.

### Prior to Move-In Day:
#### Personalization Review
- [ ] **Design Your Flow Data Reviewed** - Accessed Sigma dashboard and reviewed Neighbor's survey responses
- [ ] **Welcome Gift Selected** - Chose appropriate gift based on Neighbor's interests and preferences
- [ ] **Personalized Card Written** - Crafted warm, personal welcome message referencing their interests
- [ ] **Special Requests Noted** - Documented any specific accommodations or preferences from survey

#### Access & Logistics Preparation
- [ ] **Digital Keys Tested** - Verified Carson access credentials work properly
- [ ] **Elevator Booking Confirmed** - Confirmed scheduled time slot in Google Calendar

#### Communication & Follow-up Setup
- [ ] **Neighbor Notified** - Sent confirmation message with move-in day details
- [ ] **Team Briefed** - Updated Front Desk and Operations on any special considerations
- [ ] **Follow-up Scheduled** - Set calendar reminder for 48-hour check-in
- [ ] **Integration Milestones Set** - Planned 30-day integration goals and checkpoints

### Post-Move-In Day:
#### Community Integration Planning
- [ ] **48-Hour Check-in Completed** - Checked in with Neighbors via Ringcentral and logged in Neighbor CRM.
- [ ] **Added Neighbors to Whatsapp Community** - Added Neighbors to Whatsapp Community and sent welcome message.
- [ ] **Flow Groups Identified** - Reviewed Neighbor interests and matched to relevant Flow Groups
- [ ] **Ambassador Connections** - Identified appropriate Ambassadors for introductions
- [ ] **Invited to New Neighbor Welcome Event** - Confirmed Neighbor's inclusion in upcoming New Neighbor Event
- [ ] **Coffee Meeting Planned** - Scheduled Week-One coffee with relevant community members

### Completion Requirements:
- All "Prior to Move-In Day" items must be checked before move-in day
- All "Post-Move-In Day" items completed within 30 days of move-in
- Neighbor must receive comprehensive preparation communication
- Team must be fully briefed on special accommodations

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

> Delivering this SOP ensures that every Neighbor’s first day at Flow feels like coming home—not moving house.