---
name: "Unit Move-In Readiness SOP"
operating_practice: "Foundational Journey"
journey_stage: "Join"
last_updated: "2025-01-27"
systems: ["Yardi Voyager", "Neighbor CRM & Move-in Tracker", "Waves", "Typeform", "Google Scripts", "Slack"]
related_sops: ["Move-In SOP", "Unit Readiness Checklist", "Maintenance Request SOP"]
---

# Unit Move-In Readiness SOP

## Goals
| **Type** | **Goal** |
|-----------|-----------|
| **Operational** | Ensure every Neighbor is delighted by their first impression of their unit. Achieve 100% satisfaction rate with zero complaints from new move-ins. |
| **Experiential** | Make sure Neighbors feel their unit is clean and fully functional when they move in, creating an immediate sense of home and belonging. |

---

## Scope
Applies to **all residential units** preparing for move-in across all Flow-managed properties. This SOP covers the unit turn/make ready process ensuring every unit meets Flow's hospitality standards for cleanliness, functionality, and presentation.

---

## Roles & Responsibilities
- **Owner:** **Assistant General Manager (AGM)** — accountable for end-to-end unit readiness outcome
- **Deputy:** **Chief Engineer / Maintenance Manager**

| **Role** | **Responsibilities** |
|-----------|----------------------|
| **Chief Engineer / Maintenance Manager** | Conduct pre-maintenance inspection, create work orders in Waves, complete maintenance work, conduct post-maintenance inspection, update Neighbor CRM via typeform. |
| **Maintenance Team** | Complete work orders assigned by Maintenance Manager in Waves, address technical issues, ensure all systems operational. |
| **Cleaning Company (Third-Party)** | Deep clean unit per AGM instructions, complete cleaning typeform upon completion. |
| **Assistant General Manager (AGM)** | Coordinate with cleaning company via Slack, conduct post-cleaning inspection via Final Unit Inspection typeform, approve "Unit Ready" status in Neighbor CRM. |
| **Leasing Agent** | Conduct final pre-move-in unit inspection via Final Unit Inspection typeform, verify readiness before move-in. |

**Escalation Ladder:**  
Maintenance/Cleaning → Chief Engineer / Maintenance Manager → AGM → GM → Regional Operations

**Weekend/After-Hours:** On-duty Maintenance Manager handles readiness operations with AGM backup. All readiness issues logged in Zendesk with "Unit Readiness" tag.

---

## Systems & Tools
- **Neighbor CRM & Move-in Tracker** — Source of truth for unit turn/make ready status (Google Sheets)
- **Typeform** — Three inspection forms: Maintenance, Cleaning, Final Unit Inspection
- **Slack** — Real-time notifications from typeform submissions to dedicated channels
- **Yardi Voyager** — Unit status and move-in scheduling (status updated when unit ready)
- **Waves** — Maintenance work order tracking and completion
- **Google Scripts** — Automated status updates to Neighbor CRM & Move-in Tracker

> 🔹 **Tech Note:** Typeform responses automatically flow to Slack and update Neighbor CRM & Move-in Tracker via Google Scripts. Unit status in Yardi is updated when unit is marked ready.  
> 🔹 **Data Flow:** Typeform → Slack → Google Scripts → Neighbor CRM & Move-in Tracker → Yardi

---

## Triggers
- **Primary Trigger:** Unit needs to be prepared for move-in (either post-construction in lease-up or unit turn after previous resident)
- **System Chain:** Neighbor CRM & Move-in Tracker identifies unit → Work orders created in Waves → Typeform inspections completed → Status updates via Google Scripts
- **Fail-Safe:** If typeform submissions fail, manual status updates can be made directly in Neighbor CRM & Move-in Tracker
- **Readiness Gate:** Unit cannot be marked ready until:
  - All Waves work orders completed
  - Post-maintenance inspection passed (Maintenance Manager)
  - Cleaning completed and confirmed
  - Final inspections passed (AGM & Leasing Agent)

---

## Process

There are three critical phases to making a unit ready: **Maintenance**, **Cleaning**, and **Inspection**. Inspections take place before and after each phase to ensure quality standards are met throughout the process.

### **1. Maintenance**

| **#** | **Step / Action** | **Responsible** | **System(s)** | **Operator Experience** | **Deliverable** |
|-------:|-------------------|-----------------|---------------|--------------------------|-----------------|
| 1 | **Pre-Maintenance Inspection** | Chief Engineer / Maintenance Manager | Waves, Typeform | Identify what needs to be fixed/set up, create work orders in Waves | Waves work orders created |
| 2 | **Complete Maintenance Work** | Maintenance Team | Waves | Address all work orders, ensure everything operational | All work orders marked complete |
| 3 | **Post-Maintenance Inspection** | Chief Engineer / Maintenance Manager | Typeform, Neighbor CRM | Inspect completed work via Maintenance Inspection typeform, create additional work orders if needed | Typeform submitted → Status updated in Neighbor CRM |

### **2. Cleaning**

| **#** | **Step / Action** | **Responsible** | **System(s)** | **Operator Experience** | **Deliverable** |
|-------:|-------------------|-----------------|---------------|--------------------------|-----------------|
| 4 | **Daily Coordination with Cleaning Company** | AGM | Slack | AGM messages cleaning company with units to clean tomorrow via Slack | Cleaning assignments communicated |
| 5 | **Complete Deep Clean** | Cleaning Company | N/A | Perform comprehensive deep cleaning of unit | Unit cleaned to luxury standards |
| 6 | **Confirm Cleaning Completion** | Cleaning Company | Typeform | Complete cleaning typeform with unit number, cleaner name, time details, and checklist | Typeform submitted → Status updated in Neighbor CRM |

### **3. Final Inspection**

| **#** | **Step / Action** | **Responsible** | **System(s)** | **Operator Experience** | **Deliverable** |
|-------:|-------------------|-----------------|---------------|--------------------------|-----------------|
| 7 | **Post-Cleaning Inspection** | AGM | Typeform, Neighbor CRM | Inspect cleaned unit via Final Unit Inspection typeform | Typeform submitted → Status updated in Neighbor CRM |
| 8 | **Final Pre-Move-In Inspection** | Leasing Agent | Typeform, Neighbor CRM | Final unit inspection via Final Unit Inspection typeform before move-in day | Typeform submitted → Status updated in Neighbor CRM |
| 9 | **Approve "Unit Ready"** | AGM | Neighbor CRM, Yardi | Review all completed typeforms in Neighbor CRM, update unit status to "Ready" in Yardi | Unit status: "Ready" in Yardi |

> 🔹 **Cross-Reference:** This process runs synchronously with pre-move-in steps in the [Move-In SOP](move-in-sop.md)  
> 🔹 **Readiness Definition:** A unit is ready when all three phases are complete (maintenance work done, cleaning done, inspections passed)  
> 🔹 **Documentation:** Every inspection must be completed via typeform, with responses automatically updating Neighbor CRM & Move-in Tracker status

---

## Typeform Structures

### **1. Maintenance Inspection Typeform**

**Purpose:** Pre-maintenance and post-maintenance inspections by Chief Engineer / Maintenance Manager

**Technical Focus Items:**
- Water Meter Installed
- CWE hardware Installed
- Thermostat Installed
- Wire Closet Demo/Patched
- Closet Installed
- Shades Installed
- Bedroom Blackouts + Metal Chain Confirmed
- Refrigerator - Clean, cold, ice maker working, no odors
- Stove - Clean, all burners working, oven heats properly
- Dishwasher - Clean, cycles complete properly, no leaks
- Washer & Dryer - Clean, no lint, functioning properly
- Microwave - Clean, heats properly, door seals correctly
- HVAC - Air conditioning/heating working, filters clean
- Taps & Shower - All faucets work, no leaks, hot water available
- Lighting - All fixtures working, bulbs in every lamp

### **2. Cleaning Completion Typeform**

**Purpose:** Cleaning company confirms completion of deep clean

**Fields:**
- Unit number
- Name of cleaner
- Date of cleaning
- Time started
- Time completed
- Checklist: "Yes/No I cleaned this space" running through all normal deep cleaning items for luxury apartments
- Are there any issues to report?

### **3. Final Unit Inspection Typeform**

**Purpose:** Final inspections by AGM and Leasing Agent

**Questions:**
- Please confirm that you are inspecting [unit_number]
- First name
- Last name
- Refrigerator - Clean, cold, ice maker working, no odors
- Stove - Clean, all burners working, oven heats properly
- Dishwasher - Clean, cycles complete properly, no leaks
- Washer & Dryer - Clean, no lint, functioning properly
- Microwave - Clean, heats properly, door seals correctly
- HVAC - Air conditioning/heating working, filters clean
- Taps & Shower - All faucets work, no leaks, hot water available
- Lighting - All fixtures working, bulbs in every lamp
- Are there any other issues with the Appliances & Systems?
- Floors - Clean, no stains, appropriate for flooring type
- Walls - Clean, no scuffs or marks, touch-ups complete
- Windows - Clean inside and out, screens intact, blinds working
- Bathroom - Spotless, all fixtures working, no mold or mildew
- Kitchen - Clean counters, cabinets, sink, no food residue
- Closets - Clean, shelves wiped down, doors working properly
- Are there any other issues with the Cleanliness & Presentation of the Unit?
- Smoke Detectors - Working, batteries fresh, no chirping
- Locks - All doors and windows lock properly
- Key Access - Neighbor keys are able to open and lock the door
- Electrical Outlets - All working, no exposed wiring
- Are there any other issues with the Safety & Functionality of the Unit?
- Is there anything else to report?
- unit_number
- move_in_date
- Submitted At
- Token

> 🔹 **Note:** All three typeforms automatically post responses to Slack and update Neighbor CRM & Move-in Tracker via Google Scripts

---

## Handoff to Move-In SOP
**Unit Ready Checklist** (confirmed in Neighbor CRM & favors status in Yardi):
1. All Waves work orders completed ✓
2. Post-maintenance inspection passed ✓
3. Cleaning completed and confirmed ✓
4. Final inspections passed (AGM & Leasing) ✓
5. Unit status updated to "Ready" in Yardi ✓

Once all items are complete, unit status is updated in Yardi and move-in can proceed per Move-In SOP.

---

## Quality Standards & Metrics
| **Category** | **Metric** | **Target** |
|---------------|------------|------------|
| **Readiness** | Units marked "Ready" before move-in date | 100% |
| **Completeness** | All three dimensions complete before "Ready" status | 100% |
| **Satisfaction** | Zero complaints from new move-ins | 100% |
| **Timeliness** | Average time to complete all three dimensions | ≤ 48 hours |
| **Documentation** | All typeform inspections completed for each unit | 100% |

---

## Resources & Templates
- [Maintenance Inspection Typeform]
- [Cleaning Completion Typeform]
- [Final Unit Inspection Typeform]
- [Unit Readiness Checklist]
- [Maintenance Punch List Template]
- [Housekeeping Standards Guide]

---

## Screenshots & Visuals
- [Placeholder: Neighbor CRM & Move-in Tracker - Unit readiness status view]
- [Placeholder: Waves - Work order interface]
- [Placeholder: Typeform - Inspection forms]
- [Placeholder: Slack - Typeform notifications]

---

> Delivering this SOP ensures that every Neighbor's first moment in their Flow home feels like coming home — not moving house.
