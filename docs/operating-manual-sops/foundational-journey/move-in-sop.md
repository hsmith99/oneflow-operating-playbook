---
name: "Move-In SOP (v1.1) – Final Edited"
repository: "One Flow Operating Playbook Repository"
linked_agents: ["Flow SOP Reviewer Agent"]
last_updated: "2025-10-18"
---

# Move-In SOP (v1.1)

> 🔗 **[Quick Link: Jump to Process](#process)**

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
| **Leasing Agent** | Owns all pre–move-in steps: verifying requirements, scheduling, and sending the Welcome Email. Co-leads the unit walkthrough and marks completion in Moved before handoff. |
| **Move-In Experience Agent** | Acts as Move-In Advocate: prepares unit touches (gift, card, keys), conducts check-ins at 48 hours and Week One, and ensures the Neighbor’s integration milestones are achieved within 30 days using Sigma dashboards. |
| **Assistant General Manager (AGM)** | Runs weekly Move-In readiness meetings (Monday), assigns Move-In Advocates for all known move-ins, leads daily move-in huddles with key stakeholders to stay on top of upcoming move-ins and address blockers, resolves blockers across functions, verifies readiness in Moved/Yardi, and approves "Go" status prior to key release to Neighbors, ensuring that all requirements are met before the Neighbor moves in. |
| **Operations Manager / Front Desk Lead** | Manages day-of logistics, elevator operations, and issue triage through Zendesk and Slack. Acts as on-duty executive for after-hours or weekend move-ins. |
| **Front Desk Team** | Greets and orients Neighbors, helps to make keys, supports with 48 Check-ins, confirms access, assists with parking and elevator use, logs issues in Zendesk, and updates #fx and #move-ins Slack channels. Verifies elevator bookings by checking Moved and Google Calendar; adds reserved elevator times to Neighbor CRM & Move-in Tracker. **When trained and assigned as Move-In Advocate:** Supports and completes move-in requirements with Neighbors upon arrival if Leasing team is unavailable. |
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
- **Leasing Agent** handles all steps through Day 1 (Steps 2-4, 6-9, 11)
- **Leasing Agent** conducts unit walkthrough and key handoff (or Front Desk Team if trained and assigned as Advocate)
- **Leasing Agent** completes move-in confirmation (or Front Desk Team if trained and assigned as Advocate, with AGM verification)

### **Move-In Advocate Assignment**
- **Move-In Advocate** assigned from **Front Desk Team**
- **Move-In Advocate** should be the **Front Desk Agent working on move-in day**
- **Ideal timing:** Front Desk Agent scheduled during neighbor's move-in window
- **AGM** assigns Front Desk Agent as Move-In Advocate in Moved/Sigma

### **Post-Move-In Responsibilities (Move-In Advocate)**
- **Move-In Advocate** handles all post-Day 1 activities (Steps 12-14)
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
| 7 | Move-In Experience Agent | **Leasing Agent** |
| 10 | Leasing Agent + Move-In Experience Agent | **Leasing Agent** (solo) or **Front Desk Team** (if trained and assigned as Advocate) |
| 11 | Leasing Agent (with AGM verification) | **Leasing Agent** (with AGM verification) or **Front Desk Team** (if trained and assigned as Advocate, with AGM verification) |
| 12 | Move-In Experience Agent | **Move-In Advocate** (Front Desk Agent) |
| 13 | Move-In Experience Agent + Community Engagement Lead | **Move-In Advocate** + **GM/AGM/Ambassador** |
| 14 | AGM + Move-In Experience Agent | **AGM** + **Move-In Advocate** |

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
- Yardi → Carson/Flow App: Flow App invite via Carson is **automatic** and sent once AGM hits the "move-in button" in Yardi after keys are received and all requirements are complete. No manual action needed.

---

## Triggers
- **Primary Trigger:** Signed lease in Yardi Voyager.  
- **System Chain:** Yardi syncs overnight → Moved checklist auto-generates → Welcome Email triggers → Neighbors added to Neighbor CRM & Move-in Tracker.
- **Readiness Gate:** Keys **cannot** be released until ALL of the following are complete in Moved and verified:
  - Move-in balance paid via **certified funds** (security deposit + first month's rent)
  - Electricity set up by Neighbor
  - Proper renters insurance verified
  - All documents uploaded to Yardi lease profile
  - Service elevator reservation confirmed in Google Calendar
  - AGM approves Key Release in Moved

---

## Process

### Weekly & Daily Meetings

**Weekly Move-In Meeting (Monday):**
- **Led by:** Assistant General Manager (AGM)
- **Attendees:** Leasing, Front Desk Lead, Operations Manager (if staffed), Chief Engineer / Maintenance Manager
- **Purpose:** Review all known upcoming move-ins, assign Move-In Advocates for all move-ins scheduled for the coming week, identify blockers, and ensure coordination across functions.

**Daily Move-In Huddle:**
- **Led by:** Assistant General Manager (AGM)
- **Attendees:** Key stakeholders from all functions (Leasing, Front Desk, Operations, Maintenance)
- **Purpose:** Review upcoming move-ins, address blockers, hold each other accountable for readiness tasks, and update Neighbor CRM & Move-in Tracker with current status.

---

| **#** | **Step / Action** | **Responsible Team Member** | **System(s)** | **Operator Experience** | **Neighbor Experience** |
|---:|--------------------|----------------------------|---------------|--------------------------|--------------------------|
| 1 | **Weekly Move-In Meeting (Monday)** | **Assistant General Manager (AGM)** | Neighbor CRM, Moved, Sigma | AGM runs meeting, reviews all known move-ins, assigns Move-In Advocates to all move-ins scheduled for coming week, identifies blockers. | N/A - Internal coordination |
| 2 | Verify pre–move-in requirements complete | **Leasing Agent** | Yardi, Moved | Leasing confirms **move-in balance paid via certified funds** (security deposit + first month's rent), **electricity set up**, and **proper renters insurance** verified. Updates status in Moved. All documents uploaded to Yardi lease profile. | Receives checklist confirmation email. |
| 3 | Send Welcome Email + Portal Access | **Leasing Agent** | Moved | Leasing triggers Welcome Email template with checklist and building info. | Receives clear timeline and portal access. |
| 4 | Schedule Move-In Date + Service Elevator | **Neighbor** (via Moved), **Front Desk Team** (verification) | Google Calendar, Moved, Neighbor CRM | Neighbor schedules **service elevator reservation** (3-hour slot) in Google Calendar via Moved and confirms task complete in Moved. **Front Desk Team checks Moved and calendar to ensure all move-ins have reserved service elevator; adds reserved times to Neighbor CRM & Move-in Tracker. This is CRITICAL - every move-in must have a service elevator reservation before keys are handed over.** | Schedules service elevator reservation via Moved; receives confirmation. |
| 5 | Assign Move-In Advocate (for move-ins appearing during week) | **Assistant General Manager (AGM)** | Moved, Sigma | AGM assigns Advocate for move-ins that appear after Monday meeting; Advocate reviews Design Your Flow data in Sigma. | Receives intro message from their Advocate. |
| 6 | Unit Turn/Make Ready Process (synchronous with steps 2-5) | **Chief Engineer / Maintenance Manager**, **AGM**, **Leasing Agent**, **Cleaning Company** | Waves, Typeform, Neighbor CRM, Slack | **Maintenance:** Pre-inspection → work orders in Waves → maintenance work → post-inspection. **Cleaning:** AGM coordinates with cleaning company via Slack → deep clean → cleaning typeform submission. **Inspection:** AGM and Leasing Agent complete final unit inspection typeforms. Status updates automatically to Neighbor CRM. | Unit ready before move-in
| 7 | Prepare Keys + Access + Welcome Gift (24h) | **Move-In Experience Agent** | Carson, Moved | Advocate stages Welcome Gift and card, tests access credentials. | Finds personalized gift waiting in unit. |
| 8 | Place Packages in Unit | **Leasing Agent** or **Move-In Experience Agent** | Neighbor CRM | Check for any packages received for Neighbor, place in unit before move-in. | Packages waiting in unit upon arrival. |
| 9 | Day-of Arrival Greeting + Orientation | **Front Desk Team** | Carson, Zendesk | Front Desk greets Neighbor. **CRITICAL:** Before proceeding, Front Desk verifies ALL move-in requirements complete in Moved (certified funds payment, electricity, insurance, documents, AGM approval, service elevator reservation). If any requirement incomplete, **DO NOT hand over keys** - escalate to AGM immediately. | Feels warmly welcomed and supported. |
| 10 | Unit Walkthrough + Key Handoff | **Leasing Agent** + **Move-In Experience Agent** (or **Front Desk Team** if trained and assigned as Advocate) | Moved, Yardi | Leasing + Advocate walkthrough; resolve issues; confirm satisfaction. **CRITICAL:** Keys are ONLY handed over after ALL requirements verified (certified funds, electricity, insurance, documents, AGM approval, service elevator reservation). **If Leasing unavailable and Front Desk Agent is trained Move-In Advocate:** Front Desk Agent supports and completes move-in requirements with Neighbor. | Feels confident, at home, and supported. |
| 11 | Complete Move-In Confirmation | **Leasing Agent** (with **AGM** verification) or **Front Desk Team** (if trained and assigned as Advocate, with AGM verification) | Moved, Yardi | Leasing or Front Desk Agent marks checklist complete only after keys are received. AGM verifies no open items, then hits "move-in button" in Yardi which triggers automatic Flow App/Carson invite to Neighbor. | Receives notification of completion and Flow App invite. |
| 12 | 48-Hour Check-In | **Move-In Experience Agent** | RingCentral, Neighbor CRM | Advocate calls Neighbor via RingCentral phone call, logs feedback and notes in Neighbor CRM, routes issues to appropriate team. | Appreciates proactive care. |
| 13 | Week-One Coffee + Introductions | **Move-In Experience Agent** + **Community Engagement Lead** | Sigma, Carson | Advocate schedules coffee, connects to Ambassadors and Flow Groups. | Begins building relationships. |
| 14 | 30-Day Integration Review | **Assistant General Manager (AGM)** + **Move-In Experience Agent** | Sigma | AGM + Advocate confirm Neighbor attended event or joined group; log completion. | Feels fully integrated into community. |

---

## Unit Turn/Make Ready Process

The Unit Turn/Make Ready process runs **synchronously** with pre-move-in steps (Steps 2-5) and ensures the unit is ready before the Neighbor arrives. This process has three critical phases: **Maintenance**, **Cleaning**, and **Inspection**.

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
1. **Move-in balance paid via certified funds** — Security deposit and first month's rent paid via certified funds (certified check or money order). Payment verified and uploaded to Yardi lease profile  
2. **Electricity set up** — Neighbor has set up electricity account in their name. Confirmation uploaded to Yardi lease profile  
3. **Proper renters insurance** — Renters insurance proof uploaded to Yardi lease profile and verified for compliance  
4. **All documents uploaded to Yardi** — Lease, deposit, rent payment, insurance proof, and all required documents uploaded to lease profile in Yardi Voyager  
5. **Unit Ready confirmation** — All typeform inspections complete (Maintenance, Cleaning, Final Inspection) - see Unit Readiness SOP  
6. **Service elevator reservation** — Neighbor has reserved service elevator in Google Calendar via Moved. Front Desk verifies reservation and logs reserved times in Neighbor CRM & Move-in Tracker  
7. **Welcome Gift and Note placed in unit** — Personalized gift and card placed in unit 24 hours before move-in  
8. **Packages placed in unit** — Any packages received for Neighbor placed in unit before move-in (if applicable)  
9. **AGM approval for key release** — AGM has verified all requirements complete in Moved and approved key release

**Carson/Flow App Access:** Invite is **automatic** and sent once AGM hits the "move-in button" in Yardi after keys are received and all requirements are complete. No manual action needed.

> 🔹 **Unit Readiness (Maintenance/Cleaning):** A unit is ready from a maintenance and cleaning perspective when:
> - All Waves work orders completed
> - Post-maintenance inspection passed (Maintenance Manager)
> - Cleaning completed and confirmed
> - Final inspections passed (AGM & Leasing Agent)
>
> 🔹 **Move-In Readiness:** A move-in is ready for move-in day when:
> - Unit is ready (see above)
> - **Move-in balance paid via certified funds** (security deposit + first month's rent)
> - **Electricity set up** by Neighbor
> - **Proper renters insurance** verified
> - Neighbor has completed all required tasks in Moved (approved by Leasing/Move-In Experience Leads)
> - All documents uploaded to Yardi lease profile
> - Welcome Gift and Note placed in unit
> - Packages placed (if any received)
> - **Service elevator reserved** (Neighbor schedules via Moved; verified by Front Desk in Google Calendar)
> - AGM has approved key release in Moved
>
> **Note:** Carson/Flow App invite is **automatic** and sent once AGM hits the "move-in button" in Yardi after keys are received and all requirements are complete.

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

## Guide to Being a Move-In Advocate (Front Desk Team)

**Purpose:** This guide provides Front Desk Agents with a comprehensive checklist for executing the Move-In Advocate role when assigned by AGM. Use this guide to ensure you deliver a seamless, personalized move-in experience that makes every Neighbor feel welcomed, supported, and connected to their new community.

**When You're Assigned:** The AGM will assign you as Move-In Advocate during the weekly Move-In meeting (Monday) or when a move-in appears during the week. You'll be assigned in Moved/Sigma, and ideally, you'll be the Front Desk Agent working on the move-in day.

**Your Role:** As Move-In Advocate, you are the Neighbor's primary point of contact for their first 30 days at Flow. You ensure they feel personally cared for, connected to the community, and supported throughout their integration journey.

---

### Pre Day 1 Checklist

**Complete these tasks before the Neighbor's move-in day:**

#### Personalization & Preparation
- [ ] **Review "Design Your Flow" Survey Data** — Access Sigma dashboard and review the Neighbor's survey responses to understand their interests, preferences, and special requests
- [ ] **Coordinate Welcome Gift** — Confirm with Move-In Experience Agent (if staffed) or AGM that personalized gift and card are placed in unit 24 hours before move-in. If you're placing the gift, select appropriate gift based on their interests from survey
- [ ] **Write Personalized Welcome Card** — Craft a warm, personal welcome message referencing their interests from the survey (e.g., "Welcome! We noticed you love yoga — we have a yoga Flow Group that meets Tuesdays!"). Place card with gift in unit
- [ ] **Review Special Requests** — Document any specific accommodations, accessibility needs, or preferences mentioned in survey or lease notes
- [ ] **Verify Unit Readiness** — Confirm unit status shows "Ready" in Moved/Yardi. If not ready, escalate to AGM immediately

#### Access & Logistics
- [ ] **Verify Service Elevator Reservation** — **CRITICAL:** Verify Neighbor has reserved the service elevator in Google Calendar via Moved. If not booked, contact Neighbor immediately to schedule. Add reserved times to Neighbor CRM & Move-in Tracker. **Every move-in must have a service elevator reservation before keys are handed over.**
- [ ] **Check for Packages** — Review package log and check if any packages have arrived for the Neighbor. If packages exist, coordinate with team to place them in unit before move-in
- [ ] **Verify All Move-In Requirements Complete** — **CRITICAL:** Before any key handoff, verify ALL requirements are complete in Moved:
  - ✅ Move-in balance paid via **certified funds** (security deposit + first month's rent)
  - ✅ Electricity set up by Neighbor
  - ✅ Proper renters insurance verified
  - ✅ All documents uploaded to Yardi lease profile
  - ✅ AGM has approved key release in Moved
- [ ] **Note on Carson/Flow App Access** — Carson/Flow App invite is automatic and will be sent once AGM hits the "move-in button" in Yardi after keys are received and all requirements are complete. No manual action needed.

#### Communication & Team Briefing
- [ ] **Notify Neighbor of Your Role** — Send brief introduction message (via RingCentral or preferred contact method) introducing yourself as their Move-In Advocate and confirming move-in details
- [ ] **Brief Front Desk Team** — Update #frontdesk Slack channel with move-in details, special considerations, and confirm you're handling as Advocate
- [ ] **Schedule 48-Hour Check-In Reminder** — Set calendar reminder for 48 hours after move-in day to conduct check-in call
- [ ] **Plan Week 1 Coffee Chat** — Begin thinking about who to connect Neighbor with (Ambassador, GM/AGM, or other community members) based on their interests

#### System Preparation
- [ ] **Access Neighbor CRM & Move-in Tracker** — Ensure you have access to Neighbor's entry in Google Sheet and can update status
- [ ] **Review Unit Details** — Familiarize yourself with unit number, floor, building location, and any unit-specific notes
- [ ] **Prepare Walkthrough Materials** — Have Moved checklist available, know how to access unit via Carson, and understand building amenities to point out during walkthrough

---

### On Day 1 Checklist

**Complete these tasks during the Neighbor's move-in day:**

#### Initial Greeting & Arrival
- [ ] **Welcome Neighbor Warmly** — Greet Neighbor by name when they arrive at front desk. Express genuine excitement about their move-in
- [ ] **Verify All Move-In Requirements Complete** — **CRITICAL:** Before proceeding, verify ALL move-in requirements are complete in Moved:
  - ✅ Move-in balance paid via **certified funds** (security deposit + first month's rent)
  - ✅ Electricity set up by Neighbor
  - ✅ Proper renters insurance verified
  - ✅ All documents uploaded to Yardi lease profile
  - ✅ AGM has approved key release in Moved
  - ✅ Service elevator reservation confirmed in Google Calendar
- [ ] **DO NOT Hand Over Keys if Requirements Not Met** — If any requirement is incomplete, explain to Neighbor what's needed and escalate to AGM immediately. Keys cannot be released until ALL requirements are complete.
- [ ] **Offer Refreshments** — Offer water, coffee, or snacks to make them feel welcome and comfortable

#### Unit Walkthrough & Key Handoff
- [ ] **Conduct Unit Walkthrough** — Walk Neighbor to their unit. Point out building amenities on the way (mailroom, package room, elevators, amenities)
- [ ] **Complete Unit Inspection** — Walk through unit together, checking:
  - All lights and switches working
  - Appliances functioning (refrigerator, stove, HVAC)
  - Windows and doors opening/closing properly
  - Water pressure and temperature
  - Any damage or issues noted
- [ ] **Document Issues Immediately** — Log any issues found in Zendesk with "Move-In" tag and assign to appropriate team (Maintenance, Operations, etc.)
- [ ] **Point Out Welcome Gift** — Direct Neighbor's attention to personalized gift and card in unit. Share why you selected it based on their interests
- [ ] **Confirm Packages in Unit** — Verify any packages are present and point them out
- [ ] **Verify Service Elevator Access** — Confirm movers/Neighbor know how to access and use the service elevator for their reservation window
- [ ] **Note on Flow App Access** — Inform Neighbor that their Flow App invite (via Carson) will be sent automatically once AGM processes the move-in in Yardi after keys are received and all requirements are complete. They'll receive an email invitation.

#### Information & Orientation
- [ ] **Provide Building Orientation** — Share key information:
  - Mailroom location and mailbox number
  - Package room location and process
  - Parking information and passes (if applicable)
  - Elevator use and reservation process
  - Amenity locations and reservation process
  - Emergency contacts and procedures
- [ ] **Walk Through Flow App/Carson Features** — Show Neighbor how to:
  - Reserve amenities
  - Request maintenance
  - Access deliveries
  - Connect with neighbors
- [ ] **Share Community Information** — Mention upcoming events, Flow Groups, and New Neighbor Welcome Event. Invite them to check out community calendar
- [ ] **Provide Contact Information** — Share your direct contact info (if appropriate) and explain when to reach you vs. front desk general line

#### Move-In Completion
- [ ] **Verify Keys Handed Over After All Requirements Met** — Confirm that keys were only handed over after ALL requirements verified (certified funds payment, electricity, insurance, documents, AGM approval)
- [ ] **Complete Move-In Confirmation** — Mark checklist complete in Moved. Verify with AGM if required before marking complete
- [ ] **Notify AGM to Process Move-In in Yardi** — Confirm with AGM that move-in should be processed in Yardi (hitting "move-in button") which triggers Flow App/Carson invite to Neighbor
- [ ] **Update Neighbor CRM** — Log move-in completion in Neighbor CRM & Move-in Tracker. Note any special considerations or issues
- [ ] **Post to Slack Channels** — Update #fx and #move-ins Slack channels with move-in completion status and any notes for team
- [ ] **Hand Off to Moving Team** — If movers are present, provide directions and coordinate service elevator access during their reservation window. Assist with move-in logistics as needed
- [ ] **Confirm Follow-Up Scheduled** — Remind Neighbor you'll check in with them in 48 hours. Confirm best contact method

---

### Post Day 1 Checklist

**Complete these tasks after move-in day (within 30 days):**

#### Immediate Follow-Up (48 Hours)
- [ ] **48-Hour Check-In Call** — Call Neighbor via RingCentral (or preferred method) 48 hours after move-in. Use warm, conversational tone:
  - How are they settling in?
  - Are they experiencing any issues or concerns?
  - Do they have questions about the building or community?
  - Are they comfortable with access and systems?
- [ ] **Log Feedback in Neighbor CRM** — Document all feedback, questions, and concerns in Neighbor CRM & Move-in Tracker
- [ ] **Route Issues to Appropriate Team** — If Neighbor reports issues, create Zendesk tickets or escalate to Maintenance, Operations, etc. Follow up to ensure resolution
- [ ] **Add to WhatsApp Community** — Add Neighbor to WhatsApp Community (if applicable) and send welcome message introducing them

#### Week 1 Integration (Days 1-7)
- [ ] **Schedule Week 1 Coffee Chat** — During 48-hour check-in, invite Neighbor to coffee chat. Options:
  - Conduct personally (if comfortable)
  - Schedule with GM or AGM
  - Connect with appropriate Ambassador
- [ ] **Identify Flow Group Matches** — Review Neighbor's interests from "Design Your Flow" survey and match to relevant Flow Groups. Send invitations during coffee chat
- [ ] **Invite to New Neighbor Welcome Event** — Confirm Neighbor is invited to upcoming New Neighbor Welcome Event. Share date, time, and what to expect
- [ ] **Follow Up on Reported Issues** — Check status of any Zendesk tickets created during move-in. Ensure all issues are resolved and follow up with Neighbor to confirm satisfaction

#### Community Connection (Days 8-21)
- [ ] **Connect with Ambassadors** — Introduce Neighbor to appropriate Ambassadors based on interests. Facilitate introduction via email, WhatsApp, or in-person
- [ ] **Promote Community Events** — Share upcoming community events that align with Neighbor's interests. Encourage attendance
- [ ] **Encourage Flow Group Participation** — Follow up on Flow Group invitations. Check if Neighbor has joined and attended any meetings
- [ ] **Facilitate Neighbor Connections** — If Neighbor expresses interest, help connect them with other residents who share similar interests (with permission)

#### 30-Day Integration Review (Day 30)
- [ ] **Conduct 30-Day Integration Review** — Check in with Neighbor (via call or in-person) to assess integration progress:
  - Have they attended the New Neighbor Welcome Event?
  - Have they joined any Flow Groups?
  - Have they connected with Ambassadors or other neighbors?
  - How do they feel about their community connection?
- [ ] **Document Integration Milestones** — Log completion status in Neighbor CRM & Move-in Tracker. Update Sigma dashboard with integration progress
- [ ] **Confirm Event Attendance or Group Membership** — Verify Neighbor has attended event or joined group. If not, offer additional support or connections
- [ ] **Transition to Ongoing Support** — Confirm Neighbor feels integrated and understands ongoing support channels (Front Desk, Community Engagement Lead, etc.)
- [ ] **Update AGM on Integration Status** — Share integration completion status with AGM for their 30-Day Integration Review with Move-In Advocate

#### Ongoing Support (As Needed)
- [ ] **Monitor Integration Progress** — Continue checking in periodically if Neighbor hasn't achieved integration milestones. Offer additional support or alternative connections
- [ ] **Respond to Questions** — Be available to answer questions about building, community, or resources as they arise
- [ ] **Celebrate Integration Wins** — Acknowledge and celebrate when Neighbor joins groups, attends events, or makes connections. Reinforce their belonging

---

### Escalation & Support

**When to Escalate:**
- **Missing Move-In Requirements:** If Neighbor arrives but requirements not complete (certified funds, electricity, insurance) → **DO NOT hand over keys.** Escalate to AGM immediately for resolution
- **No Service Elevator Reservation:** If Neighbor has not reserved service elevator → Contact Neighbor immediately to schedule. Escalate to AGM if reservation cannot be made before move-in time
- **Unit Readiness Issues:** If unit is not marked "Ready" 24 hours before move-in → Escalate to AGM immediately
- **Access Problems:** If Carson access doesn't work → Escalate to Operations Manager or Front Desk Lead
- **Move-In Delays:** If Neighbor needs to delay move-in → Notify AGM and Leasing Agent
- **Critical Maintenance Issues:** If unit has critical issues (no heat, water, etc.) → Create urgent Zendesk ticket and escalate to Maintenance Manager and AGM
- **Neighbor Concerns:** If Neighbor expresses significant dissatisfaction → Escalate to AGM and GM immediately
- **Integration Challenges:** If Neighbor struggling with integration after 30 days → Escalate to Community Engagement Lead and AGM

**Support Resources:**
- **AGM:** For move-in readiness, unit issues, or process questions
- **Front Desk Lead:** For front desk procedures, access issues, or daily operations
- **Operations Manager:** For hotel/operational questions or escalations
- **Community Engagement Lead:** For Flow Groups, events, or community connections
- **Zendesk:** For all issue tracking and ticketing

---

### Success Metrics

**Your success as Move-In Advocate is measured by:**
- **Move-In Experience:** Neighbor feels warmly welcomed and supported on Day 1
- **48-Hour Satisfaction:** Neighbor reports positive experience in 48-hour check-in
- **30-Day Integration:** Neighbor has attended New Neighbor Event or joined Flow Group by Day 30
- **Issue Resolution:** All move-in issues resolved within 48 hours
- **Community Connection:** Neighbor feels connected to community and understands how to engage

**Remember:** You are the face of Flow during one of the most important moments in a Neighbor's journey. Your warmth, attention to detail, and genuine care make the difference between a good move-in and a memorable one that creates lasting community connection.

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