# Flow Onsite Technology Stack — Agent Training Context

## Purpose
This document trains AI agents (Author and Reviewer) on Flow’s operational systems.  
Agents must understand **which tools** are used onsite, **who uses them**, and **how they integrate** across the Neighbor and Guest journey.

When generating or reviewing SOPs, always reference the correct systems by name and use consistent terminology.  
For example: “Moved” (not “the move-in app”), “Carson” (not “the building system”), etc.

---

## System Overview by Function

### 🧭 Lead to Lease Lifecycle
**Systems:** HubSpot, DeepSky Lighthouse, Yardi CRM Flex, Blue Moon, Yardi Voyager

- **HubSpot** — Marketing and prospecting CRM for early-stage leads.  
- **DeepSky Lighthouse** — Flow’s proprietary application and lease creation tool; integrates directly with Yardi Voyager.  
- **Yardi CRM Flex** — Tracks applications and manages the prospect-to-lease process.  
- **Blue Moon** — Legal lease generation platform that ensures compliance and syncs with Yardi Voyager.  
- **Yardi Voyager** — The property management and accounting system of record.

> **Integration sequence:** HubSpot → Lighthouse → CRM Flex → Blue Moon → Yardi Voyager

---

### 🏢 Property Operations
**System:** Yardi Voyager  
- Used for AP, AR, P&L, property accounting, pricing, and occupancy.  
- Central source of truth for all lease and unit data.  
- Connects to Assurant for renter’s insurance and delinquency tracking.

---

### 📦 Move-Ins and Move-Outs
**System:** Moved  
- Manages upcoming move-ins and move-outs via checklist-style workflows.  
- Syncs nightly with Yardi Voyager.  
- Displays requirement completion (rent, deposit, insurance, survey, elevator booking).  
- Used by Leasing Agents, Move-In Advocates, and Operations Managers.

---

### 🧑‍🤝‍🧑 Neighbor Experience Platform
**Systems:** Carson, Flow App  
- **Carson** — Staff-side dashboard for access, deliveries, and amenity bookings.  
- **Flow App** — Neighbor-side app that connects to Carson for digital keys, rent, maintenance, and events.

> Always specify Carson for staff workflows and Flow App for neighbor-facing actions.

---

### 🧰 Maintenance Operations
**System:** Waves (DeepSky)  
- Internal maintenance management platform.  
- Used to log, track, and complete service requests via mobile and web.  
- Syncs with Yardi for chargeback and closure tracking.

---

### 💬 Communications
**Systems:** Mailchimp, Yardi RentCafe, HubSpot, Slack, RingCentral, Google Workspace  

- **Mailchimp:** Used for newsletters and event updates.  
- **RentCafe:** Used for emergency communication (since unsubscribes don’t block delivery).  
- **HubSpot:** Prospect communications and drip campaigns.  
- **Slack:** Internal team coordination (front desk, leasing, maintenance, housekeeping, etc.).  
- **RingCentral:** Call routing and neighbor support hotline.  
- **Google Workspace:** Shared files, calendars, and operations documentation.

> Agents: When SOPs mention “notify neighbors” or “send alerts,” use Mailchimp for community, RentCafe for urgent notices.

---

### 🛏 Hotel Operations
**System:** Cloudbeds  
- Used by Front Desk and Operations Managers for short-stay and hotel units.  
- Handles reservations, check-ins, check-outs, and integration with housekeeping.

---

### ☕️ Food & Beverage Operations
**System:** Toast  
- POS and order management for cafés and grocery offerings.  
- Integrates with Drops for loyalty multipliers.

---

### 🎉 Community Engagement & Belonging
**Systems:** WhatsApp, Google Sheets, Superblocks Events App  

- **WhatsApp:** Hosts Flow Groups and Flow Clubs (community communication).  
- **Google Sheets:** Tracks event metrics and ambassador activities.  
- **Superblocks:** Event check-in and participation tracking.

> Reviewer Agents: Verify that SOPs referring to “community events” specify Superblocks for attendance logging.

---

### 🧾 Support & Feedback
**Systems:** Zendesk, Typeform  

- **Zendesk:** Support tickets and property-specific queues.  
- **Typeform:** Surveys and satisfaction feedback.

---

### 🧮 Compliance & Utilities
**Systems:** Blue Moon, Assurant, Florida Power & Light (FPL)  

- **Blue Moon:** Lease legal compliance.  
- **Assurant:** Renters insurance verification.  
- **FPL:** Utilities for Florida properties (mention local equivalent elsewhere).

---

### 📊 Data & Analytics
**System:** Sigma  

- Flow’s analytics and reporting platform.  
- Used for real-time dashboards on leasing, AR, operations, and community engagement.  
- Pulls “Design Your Flow” survey data for Move-In Advocates before orientation meetings.

> When generating reports or check-ins in SOPs, reference Sigma as the data source.

---

## 🧩 Integration Map

| Category | System(s) | Integration Path |
|-----------|------------|------------------|
| Lead to Lease | HubSpot → Lighthouse → CRM Flex → Blue Moon → Yardi Voyager | Leasing lifecycle |
| Move-Ins | Moved ↔ Yardi | Move-in checklist + sync |
| Neighbor Experience | Carson ↔ Flow App | Front desk ↔ Neighbor |
| Maintenance | Waves ↔ Yardi | Work orders + charges |
| Communication | Mailchimp / RentCafe | Broadcast + emergency alerts |
| Community | WhatsApp / Superblocks / Sheets | Events + engagement tracking |
| Support | Zendesk / Typeform | Service + feedback |
| Analytics | Sigma | Dashboards + survey data |

---

## 🧠 Agent Guidance

### For the Author Agent:
- When describing workflows, always include **the system name and purpose**.  
  Example: “Leasing Agent confirms all move-in requirements are complete in *Moved*.”
- Reference **integration triggers** when a process moves between systems.  
  Example: “Upon lease execution in *Blue Moon*, the data syncs to *Yardi Voyager*.”

### For the Reviewer Agent:
- Verify the **right system** is used for the described function.  
  Example: If a SOP mentions “logging maintenance requests,” it should reference *Waves*, not *Carson*.  
- Flag missing or incorrect system references as `[TECH-CLARITY]` comments in reviews.

---

## 🧩 Related Training Docs
- `onsite_staffing_model_training.md` (team roles and responsibilities)
- `style_guide.md` (format and tone)
- `move_in_reference_pattern.md` (example of correct system references in action)