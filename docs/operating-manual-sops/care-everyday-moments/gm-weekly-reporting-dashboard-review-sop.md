---
name: "GM Weekly Reporting Dashboard Review SOP"
operating_practice: "Care – Everyday Moments"
journey_stage: "Everyday Moments"
version: "v1.0"
last_updated: "2025-01-27"
systems: ["Sigma", "Yardi Voyager", "Snowflake", "Zendesk", "Moved", "Carson/Flow App"]
related_sops: ["Move-In SOP", "Front Desk Shifts SOP"]
---

# GM Weekly Reporting Dashboard Review SOP (v1.0)

> 🔗 **[Quick Link: Jump to Process](#process)**

## Goals
| **Type** | **Goal** |
|-----------|-----------|
| **Operational** | Establish systematic weekly review of Sigma dashboards to monitor property health, financial performance, operational metrics, and community engagement. Enable data-driven decision-making, early issue identification, and proactive course correction across all aspects of property operations. |
| **Experiential** | Ensure property leadership maintains clear visibility into Neighbor satisfaction, community engagement trends, and service quality metrics that directly impact the Flow Experience. Translate dashboard insights into actionable improvements that enhance care, belonging, and operational excellence. |

---

## Scope
Applies to **General Managers (GMs)** at all Flow properties conducting weekly dashboard reviews in **Sigma**.

**Frequency:** Weekly review session scheduled every **Monday morning** (or first business day of the week).

**Time Allocation:** 45-60 minutes for comprehensive dashboard review and action planning.

**Excludes:** Daily operational checks (covered in daily workflows), ad-hoc reporting requests, and real-time monitoring dashboards accessed throughout the week.

---

## Roles & Responsibilities
**Process Owner:** **General Manager** — accountable for weekly review execution, action planning, and follow-up.  
**Deputy:** **Assistant General Manager** (executes review if GM unavailable on Monday)

| **Role** | **Responsibilities** |
|-----------|----------------------|
| **General Manager** | Conducts comprehensive weekly Sigma dashboard review on Monday morning (or first business day), identifies trends and outliers, documents insights, creates action plans, communicates findings to leadership team, and tracks action item completion. |
| **Assistant General Manager** | Acts as deputy for review execution if GM unavailable on Monday. Provides operational context and data verification during review sessions, executes action items assigned during review, and supports GM with on-the-ground validation of dashboard metrics. |
| **Operations Manager** | Provides hotel/residential operations context, validates front desk and guest experience metrics, and implements operational improvements identified during review. |
| **Regional Director of Operations** | Reviews GM dashboard review notes and action plans, provides strategic guidance, and ensures property-level insights inform regional strategy. |
| **Data & Analytics Team** | Maintains dashboard accuracy, updates metrics definitions, responds to GM questions about data interpretation, and creates new dashboards based on property needs. |

**Escalation Ladder:**  
GM → Regional Director of Operations → Head of Data & Analytics (for data questions)  
**Action Item Escalation:** Assigned Owner → GM → Regional Director (if deadline missed)  
**Metric Threshold Escalation:** GM identifies threshold breach → Immediate notification to Regional Director → Strategic response plan

---

## Systems & Tools
| **System** | **Purpose** |
|-------------|-------------|
| **Sigma** | Primary analytics platform providing real-time dashboards on property health, financial performance, leasing metrics, operations, and community engagement. Frontend UI for Snowflake data warehouse. |
| **Snowflake** | Data warehouse containing cleaned, transformed, and aggregated data from Yardi Voyager, Moved, Zendesk, Carson, and other Flow systems. |
| **Yardi Voyager** | Source system for residential financials, lease data, unit status, and AR/collections metrics displayed in Sigma. |
| **Moved** | Source system for move-in readiness, completion rates, and Neighbor onboarding metrics. |
| **Zendesk** | Source system for support ticket volume, response times, resolution rates, and satisfaction scores. |
| **Carson/Flow App** | Source system for amenity usage, delivery metrics, and engagement activity. |

**Integration Notes:**  
- Sigma dashboards pull data from Snowflake (updated nightly via data pipelines)  
- Yardi → Snowflake → Sigma decisions are updated within 24 hours  
- Real-time metrics (occupancy, Zendesk tickets) refresh more frequently  
- Historical trends and aggregations may take up to 48 hours to reflect in dashboards  

**Fail-Safes:**  
- **Sigma Unavailable:** GM accesses Yardi Voyager reports directly and documents review in weekly notes template. Escalate to Data & Analytics team for system status.  
- **Snowflake Data Delay:** GM verifies data freshness timestamp. If > 48 hours old, proceed with available data and note limitations in review notes.  
- **Dashboard Missing/Inaccessible:** Document missing dashboard in review notes, contact Data & Analytics team for immediate restoration, and use backup reports from source systems.

---

## Triggers
- **Primary Trigger:** Start of business week (Monday morning or first business day)  
- **System Chain:** Weekly calendar reminder → Access Sigma workspace → Navigate to Property Dashboard Collection → Begin systematic review  
- **Readiness Gate:** All required dashboards must be accessible and data must be current (within 48 hours). If gate fails, proceed with available data and document limitations.  
- **Deputy Trigger:** If GM is unavailable on Monday, AGM automatically executes review by end of first business day  
- **Fail-Safe:** If Sigma is unavailable, GM accesses Yardi Voyager reports directly and documents review in weekly notes template

---

## Process

### **Weekly Dashboard Review Process**

| **#** | **Step / Action** | **Responsible Team Member** | **System(s)** | **Operator Experience** | **Neighbor Impact** |
|---:|--------------------|----------------------------|---------------|--------------------------|----------------------|
| 1 | **Access Sigma Workspace** | **General Manager** | Sigma | Log into Sigma, navigate to Property Dashboard Collection, verify all dashboards are accessible and data is current (within 48 hours). | Dashboard insights drive property-level improvements that enhance overall experience |
| 2 | **Review Property Health Scorecard** | **General Manager** | Sigma (Property Health Scorecard) | Review Property Health Scorecard for overall property performance across financial, operational, and experiential metrics. Note any red flags or declining trends. | Early identification of issues prevents service degradation |
| 3 | **Review Financial Performance** | **General Manager** | Sigma (Financial Dashboard, Yardi integration) | Review revenue, occupancy, rent growth, concession burn-off, delinquency rates, and AR aging. Compare current period to budget and identify variances. | Financial health enables investment in amenities, services, and community programs |
| 4 | **Review Leasing Metrics** | **General Manager** | Sigma (Leasing Dashboard, BoxScore data) | Analyze conversion rates, lead volume, tour-to-lease metrics, move-in pipeline, and renewal rates. Identify blockers or opportunities. | Strong leasing metrics indicate healthy community demand and retention |
| 5 | **Review Operational Performance** | **General Manager** | Sigma (Operations Dashboard, Zendesk integration) | Review work order completion rates, maintenance response times, front desk shift completion, move-in readiness scores, and unit turn times. | Operational excellence ensures Neighbors experience reliable, responsive service |
| 6 | **Review Community Engagement** | **General Manager** | Sigma (Community Dashboard, Carson/Flow App data) | Analyze amenity usage, Flow Group participation, event attendance, move-in integration milestones, and community satisfaction trends. | High engagement metrics indicate strong belonging and community connection |
| 7 | **Document Insights & Anomalies** | **General Manager** | Sigma, Google Docs/Sheets | Record key findings, trends, outliers, and questions in weekly review notes template. Flag items requiring investigation or action. | Systematic documentation ensures no insights are lost and facilitates follow-up |
| 8 | **Create Action Plan** | **General Manager** | Google Docs/Sheets, Slack | Prioritize action items based on impact and urgency, assign owners, set deadlines, and document in weekly action plan template. | Action plans translate insights into concrete improvements |
| 9 | **Communicate Findings** | **General Manager** | Slack, Weekly Team Meeting | Share dashboard summary with leadership team via Slack, discuss key findings in weekly leadership meeting, and assign action items to appropriate team members. | Transparent communication ensures team alignment and accountability |
| 10 | **Schedule Follow-Up Reviews** | **General Manager** | Google Calendar, Sigma | Schedule follow-up reviews for action items, set calendar reminders for critical metric monitoring, and book time for deeper dives into specific dashboards as needed. | Regular follow-up ensures action items are completed and improvements are implemented |

> 🔹 **Tech Note:** Sigma dashboards refresh automatically based on data pipeline schedules. GM should verify data freshness timestamp on each dashboard before review.  
> 🔹 **Cross-Reference:** [Move-In SOP](../foundational-journey/move-in-sop.md) for move-in metrics interpretation  
> 🔹 **Placeholder:** [Insert link to Property Dashboard Collection in Sigma]  
> 🔹 **Placeholder:** [Insert link to Weekly Review Notes Template]

---

## Dashboard Review Framework

### **1. Property Health Scorecard**
**Review Focus:** Overall property health composite score, trend direction, and component breakdown.

**Key Metrics:**
- Property Health Score (composite)
- Financial Health Index
- Operational Health Index
- Community Engagement Index
- Trend indicators (improving/declining/stable)

**Action Triggers:**
- **Health score decline > 5 points week-over-week:** Document in review notes, create immediate action plan, notify Regional Director within 24 hours  
- **Any component index below threshold:** Assign owner to investigate root cause, create action item with 7-day deadline, escalate to Regional Director if systemic issue  
- **Three consecutive weeks of declining trend:** Schedule deep-dive review with Data & Analytics team, develop intervention plan, escalate to Regional Director for strategic response

### **2. Financial Performance Dashboard**
**Review Focus:** Revenue, occupancy, rent growth, and financial stability.

**Key Metrics:**
- Occupancy Rate (current and trailing 12-month)
- Revenue vs. Budget variance
- Rent Growth (market rent, effective rent, rent per square foot)
- Concession burn-off rate
- Delinquency rate and AR aging
- Bad debt expense trends

**Action Triggers:**
- **Occupancy decline > 2% week-over-week:** Create action item for Leasing Manager, review marketing campaigns, notify Regional Director if decline persists two weeks  
- **Revenue variance > 5% from budget:** Assign AGM to investigate components (rent, concessions, ancillary), create action plan with financial recovery timeline, escalate to Regional Director if variance > 10%  
- **Delinquency rate > 3% or trending upward:** Assign AGM to review AR aging detail, create collection action plan, escalate to Regional Director if rate > 5%  
- **AR aging > 30 days for > 5% of residents:** Assign AGM to review individual accounts, execute collection protocols, escalate accounts > 60 days to Regional Director

### **3. Leasing Metrics Dashboard**
**Review Focus:** Leasing funnel performance, conversion rates, and pipeline health.

**Key Metrics:**
- Lead volume (website inquiries, tours scheduled)
- Tour-to-application conversion rate
- Application-to-lease conversion rate
- Move-in pipeline (next 30 days)
- Renewal rate and lease expiration schedule
- Average time-to-lease

**Action Triggers:**
- **Conversion rate decline > 5% month-over-month:** Assign Leasing Manager to analyze funnel stage, review tour quality and pricing, create improvement plan with 30-day deadline  
- **Move-in pipeline < expected volume:** Assign Leasing Manager to review lead generation, tour scheduling, and application processing, create pipeline recovery plan  
- **Renewal rate < target threshold:** Assign AGM and Leasing Manager to review renewal outreach, retention incentives, and resident satisfaction data, create retention strategy  
- **Average time-to-lease increase > 3 days:** Assign Leasing Manager to review application processing, screening delays, and leasing team capacity, create efficiency improvement plan

### **4. Operational Performance Dashboard**
**Review Focus:** Service delivery, maintenance efficiency, and operational reliability.

**Key Metrics:**
- Work order completion rate (Waves)
- Average maintenance response time
- Front desk shift checklist completion rate (Typeform)
- Move-in readiness scores (Unit Readiness SOP compliance)
- Unit turn time (vacancy to ready)
- Zendesk ticket volume and resolution time

**Action Triggers:**
- **Work order completion rate < 95%:** Assign Chief Engineer to review work order backlog, capacity constraints, and prioritization, create completion improvement plan with weekly check-ins  
- **Average response time > 48 hours:** Assign Chief Engineer to review dispatch efficiency and technician availability, create response time improvement plan, escalate if > 72 hours  
- **Front desk checklist completion < 100%:** Assign Front Desk Lead to review completion rates by shift, identify gaps, create accountability plan, escalate to Operations Manager if persists  
- **Move-in readiness < 100% on-time:** Assign AGM to review Unit Readiness SOP compliance, identify bottlenecks in maintenance/cleaning/inspection phases, create improvement plan  
- **Unit turn time > 7 days:** Assign AGM to review unit turn process, identify delays in maintenance or cleaning coordination, create efficiency improvement plan  
- **Zendesk ticket volume spike > 20% week-over-week:** Assign Operations Manager to analyze ticket categories, identify root causes, create resolution plan, escalate if spike > 50% or recurring

### **5. Community Engagement Dashboard**
**Review Focus:** Neighbor participation, belonging metrics, and community health.

**Key Metrics:**
- Amenity usage rates (Carson/Flow App)
- Flow Group participation
- Event attendance rates
- Move-in integration milestones (30-day completion)
- Community satisfaction scores (from surveys)
- "Design Your Flow" completion and personalization usage

**Action Triggers:**
- **Amenity usage decline > 10% month-over-month:** Assign Community Engagement Lead to review amenity accessibility, programming, and resident awareness, create engagement improvement plan  
- **Flow Group participation < 20% of eligible residents:** Assign Community Engagement Lead to review group offerings, promotion, and onboarding, create participation growth strategy  
- **Event attendance < 15% of community:** Assign Community Engagement Lead to review event types, scheduling, and promotion channels, create attendance improvement plan  
- **Move-in integration completion < 80% at trajectory:** Assign Move-In Experience Agent (or Move-In Advocate) to review 30-day integration milestones, identify gaps in coffee chats or event invitations, create completion improvement plan  
- **Satisfaction scores < 4.0 (5-point scale):** Assign GM to review satisfaction survey feedback, identify themes, create service improvement action plan, escalate to Regional Director if scores < 3.5

---

## Documentation Requirements

### **Weekly Review Notes Template**

**Date:** [MM/DD/YYYY]  
**Reviewed By:** [GM Name]  
**Review Time:** [Start] - [End] minutes

**Dashboard Summary:**
- Property Health Score: [Score] ([Trend: ↑/↓/→])
- Financial Health: [Status] ([Key Metric])
- Leasing Health: [Status] ([Key Metric])
- Operational Health: [Status] ([Key Metric])
- Community Engagement: [Status] ([Key Metric])

**Key Findings:**
1. [Finding with context and trend]
2. [Finding with context and trend]
3. [Finding with context and trend]

**Anomalies & Questions:**
- [Anomaly or data inconsistency requiring investigation]
- [Question for Data & Analytics team]

**Action Items:**
| **Priority** | **Action Item** | **Owner** | **Deadline** | **Status** |
|--------------|-----------------|-----------|--------------|------------|
| High | [Action] | [Owner] | [Date] | [Open/In Progress/Complete] |
| Medium | [Action] | [Owner] | [Date] | [Open/In Progress/Complete] |
| Low | [Action] | [Owner] | [Date] | [Open/In Progress/Complete] |

**Follow-Up Items:**
- [Follow-up from previous week]
- [Item requiring Regional Director review]

---

## Handoff Requirements

**Weekly Review Artifacts:**
- Completed Weekly Review Notes template ✓
- Action Plan with assigned owners and deadlines ✓
- Slack summary shared with leadership team ✓
- Follow-up calendar reminders scheduled ✓
- Critical items escalated to Regional Director ✓

**Communication Handoff:**
1. **GM → Leadership Team:** Dashboard summary and action items via Slack #leadership channel
2. **GM → Regional Director:** Weekly summary email with key findings and any regional concerns
3. **GM → Data & Analytics Team:** Questions or data issues flagged for investigation

---

## Quality Standards & Metrics

| **Category** | **Metric** | **Target** |
|---------------|------------|-------------|
| **Completeness** | Weekly review completion rate | 100% (every Monday) |
| **Timeliness** | Review completed within first 2 business days of week | 100% |
| **Thoroughness** | All five dashboard categories reviewed | 100% |
| **Actionability** | Action items created for identified issues | ≥ 80% of issues |
| **Follow-Through** | Action items completed by deadline | ≥ 90% |
| **Communication** | Leadership team receives summary within 24 hours | 100% |
| **Data Quality** | Dashboard data freshness < 48 hours | 100% |

---

## Resources & Templates
- [Insert link to Sigma Property Dashboard Collection]
- [Insert link to Weekly Review Notes Template (Google Doc)]
- [Insert link to Weekly Action Plan Template (Google Sheet)]
- [Insert link to Dashboard Metric Definitions Document]
- [Insert link to Data & Analytics Team contact list]
- [Insert link to Regional Director reporting template]

---

## Screenshots & Visuals
- [Insert screenshot of Sigma Property Dashboard Collection homepage]
- [Insert screenshot of Property Health Scorecard]
- [Insert screenshot of Financial Performance Dashboard]
- [Insert screenshot of Leasing Metrics Dashboard]
- [Insert screenshot of Operational Performance Dashboard]
- [Insert screenshot of Community Engagement Dashboard]
- [Insert screenshot of Weekly Review Notes Template]

---

## Version Control

| **Author** | **Reviewer(s)** | **Version** | **Date** | **Changes** |
|------------|-----------------|-------------|----------|-------------|
| Author Agent | Reviewer Agent | 1.0 | 2025-01-27 | Initial version |
| Reviewer Agent | - | 1.1 | 2025-01-27 | Added AGM deputy ownership, expanded fail-safes, enhanced action triggers with escalation paths, integrated Dashboard Review Framework into process steps, improved process table granularity |

---

> **ASSUMPTION:** Sigma dashboards include Property Health Scorecard, Financial Performance, Leasing Metrics, Operational Performance, and Community Engagement dashboards. Specific metric definitions and thresholds may vary by property or regional standards. GM should consult with Data & Analytics team for dashboard customization requests.  
>  
> Delivering this SOP ensures that every General Manager systematically reviews property performance through data-driven insights, enabling proactive leadership decisions that maintain Flow's standards of operational excellence and community care.
