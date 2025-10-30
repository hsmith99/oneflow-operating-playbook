---
name: "Front Desk Shifts SOP"
operating_practice: "Care – Everyday Moments"
journey_stage: "Everyday Moments"
version: "v1.1"
last_updated: "2025-01-27"
systems: ["Cloudbeds", "Yardi Voyager", "Carson/Flow App", "Slack", "Typeform", "Waves", "Zendesk"]
related_sops: ["Daily Morning Property Walkthrough SOP", "Neighbor Communication SOP"]
---

# Front Desk Shifts SOP (v1.1)

> 🔗 **[Quick Link: Jump to Process](#process)**

## Goals
| **Type** | **Goal** |
|-----------|-----------|
| **Operational** | Deliver consistent, systematic completion of all front desk responsibilities across AM and PM shifts through structured checklists, automated reporting, and clear accountability. Achieve 100% checklist completion rate with zero missed handoffs. |
| **Experiential** | Maintain Flow's hospitality standards by providing seamless, organized service that makes every Neighbor and Guest feel personally cared for and supported throughout their day. |

---

## Scope
Applies to **all Front Desk Agents** during **AM (7:00 AM - 3:00 PM)** and **PM (3:00 PM - 11:00 PM)** shifts at Flow properties. This SOP ensures comprehensive coverage of daily operations, guest services, and team coordination through structured checklists that integrate with Typeform and Slack reporting.

**Excludes:** Overnight security coverage (9 PM - 7 AM) handled by contracted security team.

---

## Roles & Responsibilities
**Process Owner:** **Front Desk Lead** — accountable for shift execution and team performance  
**Deputy:** **Operations Manager** (where staffed) or **Assistant General Manager**

| **Role** | **Responsibilities** |
|-----------|----------------------|
| **Front Desk Lead** | Oversees shift execution, trains team members, maintains service standards, conducts daily check-ins with Front Desk Agents, reviews Typeform completion rates, and escalates issues to Operations Manager. |
| **Front Desk Agent (AM/PM)** | Executes shift checklist via Typeform, maintains workspace organization, provides hospitality to Neighbors and Guests, logs issues in Zendesk, and completes handoff documentation. |
| **Operations Manager** | Supports Front Desk Lead, handles escalated issues, ensures system integration, and maintains service standards during business hours. |
| **Assistant General Manager** | Provides backup support, resolves complex issues, and ensures operational continuity during management hours. |

**Escalation Ladder:**  
Front Desk Agent → Front Desk Lead → Operations Manager → AGM → GM → Regional Operations

**Weekend/After-Hours:** On-duty Front Desk Agent handles operations with Front Desk Lead backup. All issues logged in Zendesk with "Front Desk" tag.

---

## Systems & Tools
| **System** | **Purpose** |
|-------------|-------------|
| **Cloudbeds** | Hotel operations, check-ins, check-outs, room assignments, and guest communications. |
| **Yardi Voyager** | Residential operations, move-ins, move-outs, work orders, and resident communications. |
| **Carson/Flow App** | Package management, amenity reservations, access control, and Neighbor-facing services. |
| **Slack** | Team communication, shift handoffs, incident reporting, and real-time coordination. |
| **Typeform** | Checklist completion, automated reporting, and accountability tracking. |
| **Waves** | Work order management, maintenance coordination, and issue tracking. |
| **Zendesk** | Support ticket management, escalation tracking, and customer service documentation. |

**Integration Notes:**  
- Typeform checklists automatically post completion status to #frontdesk Slack channel  
- Zendesk tickets auto-assign based on issue type and severity  
- Carson ↔ Flow App syncs access and amenity data in real-time

---

## Triggers
- **Primary Trigger:** Clock-in at shift start time (7:00 AM for AM shift, 3:00 PM for PM shift)  
- **System Chain:** Clock-in → Access Typeform checklist → Execute tasks → Submit completion → Automated Slack posting  
- **Readiness Gate:** Checklist must be completed and submitted before shift end to ensure proper handoff  
- **Fail-Safe:** If Typeform is unavailable, manual checklist completion via Google Sheets with immediate Slack notification

---

## Process

### **AM Shift Process (7:00 AM - 3:00 PM)**

| **#** | **Step / Action** | **Responsible Team Member** | **System(s)** | **Operator Experience** | **Neighbor Experience** |
|---:|--------------------|----------------------------|---------------|--------------------------|--------------------------|
| 1 | **Access AM Typeform Checklist** | **Front Desk Agent** | Typeform | Open Typeform link, begin systematic completion of all AM tasks | Seamless service begins with organized operations |
| 2 | **Complete Shared Responsibilities** | **Front Desk Agent** | Yardi, Google Sheets, Slack | Execute move-in follow-ups, post notices, log incidents, update tracking sheets | Consistent communication and service standards maintained |
| 3 | **Manage Package Room** | **Front Desk Agent** | Carson/Flow App | Organize packages, maintain cleanliness, prepare for facilities team | Easy package retrieval with organized delivery system |
| 4 | **Execute AM Shift Duties** | **Front Desk Agent** | Cloudbeds, Slack, Waves | Check arrivals/departures, coordinate cleaning, manage elevator reservations, handle vendor keys | Smooth check-ins, organized move-ins/outs, clean units ready |
| 5 | **Complete Handoff Preparation** | **Front Desk Agent** | Cloudbeds, Slack | Print registration cards, document important information for PM shift | Continuity of service between shifts |
| 6 | **Submit Completed Checklist** | **Front Desk Agent** | Typeform, Slack | Submit Typeform, receive confirmation, await automated Slack posting | Transparent operations and accountability |

> 🔹 **Tech Note:** Typeform automatically timestamps completion and posts summary to #frontdesk Slack channel  
> 🔹 **Cross-Reference:** [Daily Morning Property Walkthrough SOP](daily-morning-property-walkthrough-sop.md)  
> 🔹 **Placeholder:** [Insert link to AM Typeform checklist]

### **PM Shift Process (3:00 PM - 11:00 PM)**

| **#** | **Step / Action** | **Responsible Team Member** | **System(s)** | **Operator Experience** | **Neighbor Experience** |
|---:|--------------------|----------------------------|---------------|--------------------------|--------------------------|
| 1 | **Access PM Typeform Checklist** | **Front Desk Agent** | Typeform | Open Typeform link, review AM handoff notes, begin PM tasks | Evening service maintains same high standards |
| 2 | **Complete Shared Responsibilities** | **Front Desk Agent** | Yardi, Google Sheets, Slack | Execute move-in follow-ups, post notices, log incidents, update tracking sheets | Consistent communication across all hours |
| 3 | **Manage Package Room** | **Front Desk Agent** | Carson/Flow App | Organize packages, maintain cleanliness, prepare for facilities team | Evening package access remains organized and accessible |
| 4 | **Execute PM Shift Duties** | **Front Desk Agent** | Cloudbeds, Slack, Waves, Zendesk | Check arrivals/departures, refill supplies, confirm reservations, walk vacant units, handle tickets | Evening check-ins, amenity access, responsive maintenance support |
| 5 | **Complete Handoff Preparation** | **Front Desk Agent** | Slack, Office Organization | Organize office, restock stations, document pending items for overnight team | Clean, organized workspace for next day |
| 6 | **Submit Completed Checklist** | **Front Desk Agent** | Typeform, Slack | Submit Typeform, receive confirmation, await automated Slack posting | Complete shift accountability and transparency |

> 🔹 **Tech Note:** Typeform automatically timestamps completion and posts summary to #frontdesk Slack channel  
> 🔹 **Cross-Reference:** [Neighbor Communication SOP](neighbor-communication-sop.md)  
> 🔹 **Placeholder:** [Insert link to PM Typeform checklist]

---

## Weekend & After-Hours Coverage

**Weekend Operations:**
- **Saturday/Sunday AM:** Front Desk Agent follows standard AM process
- **Saturday/Sunday PM:** Front Desk Agent follows standard PM process  
- **Escalation:** Front Desk Lead on-call for weekend support
- **Emergency:** Security team (9 PM - 7 AM) handles overnight issues

**After-Hours (11:00 PM - 7:00 AM):**
- **Security Team:** Handles basic guest services, package logging, and emergency response
- **Escalation:** Security contacts on-call Front Desk Lead for complex issues
- **Handoff:** Security provides written summary to AM Front Desk Agent

---

## Handoff Requirements

**Required Artifacts:**
- Completed Typeform checklist with timestamp ✓
- Slack notification confirming completion ✓
- Printed registration cards for next day (PM shift) ✓
- Documented pending work orders or escalations ✓
- Clean, organized workspace ✓
- Restocked supplies and stations ✓
- Zendesk tickets updated with current status ✓

**Handoff Process:**
1. **PM to AM:** PM Agent completes checklist, organizes workspace, documents pending items
2. **AM to PM:** AM Agent reviews handoff notes, addresses pending items, maintains continuity
3. **Emergency Handoff:** If agent cannot complete shift, immediate notification to Front Desk Lead

---

## Quality Standards & Metrics

| **Category** | **Metric** | **Target** |
|---------------|------------|-------------|
| **Completion** | Checklist completion rate per shift | 100% |
| **Timeliness** | Checklist submitted within 30 minutes of shift end | 100% |
| **Accuracy** | All data entries verified and systems updated correctly | 100% |
| **Communication** | All handoff information clearly documented and shared | 100% |
| **Organization** | Workspace and supplies maintained to Flow standards | 100% |
| **Experience** | Neighbor/Guest satisfaction with front desk service | ≥ 95% positive |
| **Response Time** | Average time to address Zendesk tickets | ≤ 2 hours |

---

## Resources & Templates
- [Insert link to AM Typeform checklist]
- [Insert link to PM Typeform checklist]  
- [Insert link to Slack channel configuration]
- [Insert link to work order templates]
- [Insert link to incident report forms]
- [Insert link to handoff documentation template]
- [Insert link to emergency contact list]

---

## Screenshots & Visuals
- [Insert screenshot of Typeform checklist interface]
- [Insert screenshot of Slack notification format]
- [Insert screenshot of Cloudbeds interface for arrivals/departures]
- [Insert screenshot of package room organization standards]
- [Insert screenshot of Zendesk ticket management interface]

---

## Version Control

| **Author** | **Reviewer(s)** | **Version** | **Date** | **Changes** |
|------------|-----------------|-------------|----------|-------------|
| Author Agent | Reviewer Agent | 1.0 | 2025-01-27 | Initial version |
| Reviewer Agent | - | 1.1 | 2025-01-27 | Added process owner, escalation ladder, KPIs, weekend coverage, improved process table structure |

---

## Appendix: Typeform Checklist Templates

> ASSUMPTION: Typeform's "Import questions" supports plain text where each question is followed by hyphen-prefixed options. Blank lines separate questions. Import will create Multiple Choice questions; set each to "Multiple selection" in Typeform to behave as a checklist.

### AM Shift — Typeform Import Block

AM — Shared Responsibilities (select all completed)
- Move-in follow-up calls
- Schedule "Do not enter" work orders
- Upkeep cleanliness and organization of RX area
- Post notices to resident doors
- Log items in Lost and Found Google Sheet when turned in
- Record all incidents in Opportunity Report Log
- Update Work Google Sheets (renewals, parking violations, etc)

AM — Package Room (select all completed)
- All packages are in their proper place (no boxes outside designated areas)
- Package area cleaned and organized
- Packages organized for facilities team

AM — Shift Duties (select all completed)
- Check all Slack channels for relevant info; inform MOD if needed
- Check and answer pending emails
- Restock all FX desk stations (water, keys, index cards, etc)
- Review Cloudbeds for arrivals/no-shows/cancellations/in-house extensions
- Monitor Whistle regularly
- Cleaning coordination: arrivals assigned for cleaning
- Cleaning coordination: departures communicated
- Contact guests with pending departures and no updates
- Coordinate any room moves with cleaning team
- Elevator reservations: give mover directions / building operations
- Elevator reservations: contact all move-ins/outs from Yardi to schedule
- Elevator reservations: call to confirm G‑Calendar reservations
- Elevator reservations: resolve double bookings with Managers
- Assist directing move-in/out operations
- Record and put away overnight packages
- Verify all vendor keys are in the lockbox
- Confirm lender carts are in Flow’s possession
- Enter work orders for hotel/residential issues as reported
- Clear out move-out key fobs and return mailbox keys
- Complete any in-unit deliveries

AM — Handoff (select all completed)
- Print registration cards for remaining check-ins today
- Pass important info to PM shift; address internal action items

### PM Shift — Typeform Import Block

PM — Shared Responsibilities (select all completed)
- Move-in follow-up call
- Schedule "Do not enter" work order
- Upkeep cleanliness and organization of RX area
- Post notices to resident doors
- Log items in Lost and Found Google Sheet when turned in
- Record all incidents in Opportunity Report Log
- Update Work Google Sheets (renewals, parking violations, etc)

PM — Package Room (select all completed)
- All packages are in their proper place (no boxes outside designated areas)
- Package area cleaned and organized
- Packages organized for facilities team

PM — Shift Duties (select all completed)
- Check all Slack channels for relevant info; inform MOD if needed
- Check and answer pending emails
- Restock all FX desk stations (water, keys, index cards, etc)
- Review Cloudbeds for pending arrivals; ensure rooms assigned and clean
- Review Cloudbeds for same‑day reservations and pending departures
- Monitor Whistle regularly
- Perform PCI (pre‑check‑in arrivals)
- Refill paper and ink in the Co‑Working space
- Enter work orders for hotel and residential issues as reported
- Print and place new signage around the building
- Verify all vendor keys are in the lockbox
- Clear out move‑out key fobs and return mailbox keys
- Confirm amenity reservations
- Walk vacant units and enter work orders for needed repairs
- Print registration cards for next‑day check‑ins
- Complete internal action items; address outstanding Zendesk/Whistle items

PM — Handoff (select all completed)
- Organize and clean office
- Restock RX area and working stations
- Pass pending tickets/work orders to ON team and MOD via Slack

---

> Delivering this SOP ensures that every Front Desk shift maintains Flow's hospitality standards while providing clear accountability, systematic execution, and seamless handoffs between team members.
