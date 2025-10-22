---
name: "Yardi Operational Guide"
description: "Comprehensive guide to how Flow uses Yardi across all teams and functions"
last_updated: "2025-01-27"
systems: ["Yardi Voyager", "CRM Flex", "Maintenance IQ", "SiteManager", "VendorCafe", "ScreeningWorks", "RentCafe APIs", "Yardi APIs"]
related_docs: ["Onsite Technology Stack", "Onsite Staffing Model"]
---

# Yardi Operational Guide

## Overview

Yardi is Flow's central property management system, serving as the source of truth for all property operations, financial data, and resident information. This guide documents how each team across Flow leverages Yardi's various modules and tools to fulfill their responsibilities.

**Key Principle:** "If it didn't happen in Yardi, it didn't happen." — Jason, Director of Residential Revenue

---

## Quick Reference

### Most Common Tasks
| Task | Module | Path | Owner |
|------|--------|------|-------|
| Check resident ledger | Voyager | Resident Profile → Ledger | Front Desk |
| Process move-in | Voyager | Move-ins → Future | AGM |
| Approve invoice | Voyager | Workflow Dashboard | GM/AGM |
| Update unit availability | Voyager | Unit Availability | Leasing |
| Add resident charge | Voyager | Resident Profile → Quick Charge | AGM |
| Check work order status | Maintenance IQ | Work Order Dashboard | Maintenance |
| Process payment | Voyager | CheckScan | AGM |
| Update resident info | CRM Flex | Resident Profile | Leasing/Support |

### Emergency Contacts
- **Yardi Technical Issues:** Yardi Team (Slack #yardi-support)
- **System Down:** Regional Operations
- **Data Sync Issues:** Llu (Backend Engineer)
- **Training Questions:** Department Lead

---

## Yardi Ecosystem at Flow

### Yardi Functionality - Business Function Importance Map
[**Yardi Feature & Business Function Importance Map**](https://docs.google.com/spreadsheets/d/13O5BLxcCKWxYFkBzA7EsrcwtecraN4i8IfQlkITg5ec/edit?gid=0#gid=0) - Comprehensive mapping of Yardi tools, their descriptions, roles, and importance levels across Flow's operations.

### Core Modules
- **Yardi Voyager** — The central database and primary interface for most operations
- **CRM Flex** — Leasing-focused interface for prospect and resident management
- **Maintenance IQ** — Mobile-first maintenance work order management
- **SiteManager** — Website and marketing management
- **VendorCafe** — Vendor management and invoice processing
- **ScreeningWorks** — Application screening and approval
- **RentCafe APIs** — Website integration and resident portal
- **Yardi APIs** — Backend integration for Flow's custom applications

### Integration Points
- **Moved** — Syncs nightly with Yardi for move-in/move-out workflows
- **Carson/Flow App** — Connects to Yardi for resident data and payments
- **Sigma** — Pulls data from Yardi for advanced analytics
- **Waves** — Maintenance work orders sync with Yardi
- **Zendesk** — Support tickets reference Yardi resident data

---

## Team Usage Patterns

### 🏢 **Property Management Teams**

#### General Managers (GMs)
**Primary Tools:** Voyager Community Dashboard, Reports, Financials

**Daily Workflow:**
- Start with **Community Dashboard** for property overview and key metrics
- Review **Resident Activity** reports for move-ins, move-outs, and renewals
- Check **Unit Statistics** for rent growth and market analysis
- Use **BoxScore Summary** as primary leasing dashboard
- Process **Invoice Register** for AP approvals
- Monitor **Work Order Reports** for maintenance status

**Key Reports:**
- **Unit Statistics Report** — Most important for rent growth analysis
- **BoxScore Summary** — Leasing funnel and conversion metrics
- **Budget Comparison** — Monthly variance analysis with notes
- **Aged Receivables** — Delinquency management
- **Eviction Report** — Legal proceedings tracking

**Pain Points:**
- 12-month occupancy reports don't work reliably
- Need better elevator reservation and vendor scheduling visibility
- Manual processes for variance report compilation

#### Assistant General Managers (AGMs)
**Primary Tools:** Voyager, Move-in/Move-out workflows, Collections

**Daily Workflow:**
- Process **Move-ins** — verify requirements, post charges, update status
- Handle **Move-outs** — create statements, process deposits
- Manage **Deposit Accounting** — close ledgers within 5 days
- Process **CheckScan** for cashier's check payments
- Monitor **Delinquency Reports** — post late fees and notices
- Use **Quick Charge** for resident fees and charges

**Key Functions:**
- **Move-in Processing** — Verify all requirements before key release
- **Collections Management** — Late fees, notices, eviction tracking
- **Deposit Accounting** — Final statements and refund processing
- **Resident Ledger Management** — Charges, payments, adjustments

**Critical Workflows:**
- Move-in statement reconciliation
- Utility charge verification with Conservice
- Security deposit refund processing
- Late fee application and notice generation

---

### 🏠 **Leasing Teams**

#### Leasing Managers
**Primary Tools:** CRM Flex, Voyager Reports, ScreeningWorks

**Daily Workflow:**
- Start with **CRM Dashboard** for leasing metrics and occupancy
- Manage **CRM Queue** for prospect communication
- Review **Documents Tab** for application progress
- Use **ScreeningWorks** for application approvals
- Pull **BoxScore Summary** and **Rent Roll** for analysis
- Process **Agent Performance Reports** for commissions

**Key Functions:**
- **Prospect Management** — CRM queue, guest cards, applications
- **Lease Execution** — Digital signing through CRM Flex
- **Commission Tracking** — Agent performance and bonus calculations
- **Market Analysis** — Rent roll analysis and pricing insights

**Pain Points:**
- No email notifications from Yardi
- Limited analytics for quality control
- Manual commission reconciliation process

#### Leasing Specialists
**Primary Tools:** CRM Flex, Voyager (limited)

**Daily Workflow:**
- Check **CRM Calendar** for daily appointments
- Process **CRM Queue** for prospect communication
- Use **Guest Card Management** for application tracking
- Calculate charges with **Prorated Calculator**
- Search prospects using **CRM Search** function
- Update **Unit Availability** for prospect alternatives

**Key Functions:**
- **Prospect Communication** — Emails, texts, calls
- **Application Processing** — Document collection and verification
- **Unit Selection** — Availability checking and alternatives
- **Lease Preparation** — Terms, charges, move-in scheduling

---

### 🛠️ **Maintenance Teams**

#### Facilities & Maintenance Directors
**Primary Tools:** Maintenance IQ, Voyager Reports, VendorCafe

**Daily Workflow:**
- Review **Unit Turn Dashboard** for make-ready management
- Use **Make Ready Manager** for project coordination
- Monitor **Work Order Dashboard** for team workload
- Process **VendorCafe** invitations and approvals
- Track **Weekly Trend Analytics** for performance metrics
- Coordinate with **VENDORShield** for insurance verification

**Key Functions:**
- **Unit Turn Management** — Make-ready project coordination
- **Work Order Analytics** — Team performance and completion rates
- **Vendor Management** — Insurance verification and approval
- **Maintenance Scheduling** — Technician assignment and prioritization

**Pain Points:**
- Voyager and Maintenance IQ sync issues
- No journey from inspection to ledger charges
- Limited work order status tracking

#### Maintenance Technicians
**Primary Tools:** Maintenance IQ Mobile App

**Daily Workflow:**
- Receive work orders via **Maintenance IQ Mobile**
- Update work order status and completion
- Upload photos and resolution notes
- Coordinate with **VendorCafe** for third-party work
- Use **Work Order Management** for categorization

---

### 💰 **Accounting Teams**

#### Property Controllers
**Primary Tools:** Voyager Financial Reports, Workflow Dashboard

**Daily Workflow:**
- Review **Financial Reports** — Income Statement, Budget Comparison
- Process **Workflow Dashboard** for invoice approvals
- Monitor **Aged Receivables** for collections
- Use **General Ledger** for journal entries
- Reconcile **Bank Functions** daily
- Process **Payables** for vendor payments

**Key Functions:**
- **Financial Reporting** — Monthly P&L and variance analysis
- **Invoice Processing** — Workflow approvals and payments
- **Bank Reconciliation** — Daily cash management
- **Journal Entries** — Manual adjustments and accruals

#### AP/AR Specialists
**Primary Tools:** Payables, VendorCafe, CheckScan

**Daily Workflow:**
- Process **Payable Analytics Aging Report** for payment prioritization
- Use **Commit Payments** for vendor payment processing
- Manage **VendorCafe** for vendor onboarding and insurance
- Process **CheckScan** for check payments
- Monitor **Invoice Register Dashboard** for new invoices
- Track **Aged Payables** for outstanding payments

**Key Functions:**
- **Vendor Management** — Onboarding, insurance verification, payments
- **Invoice Processing** — Scanning, coding, workflow management
- **Payment Processing** — ACH, checks, payment methods
- **VendorCafe Management** — Insurance compliance and documentation

---

### 📊 **Pricing Teams**

#### Revenue Directors
**Primary Tools:** Voyager Reports, SiteManager

**Daily Workflow:**
- Analyze **Unit Statistics** for rent growth analysis
- Review **Rent Roll** for market vs actual rent
- Use **Lease Expiration** for renewal planning
- Process **Concession Burn Off** for effective rent calculation
- Update **Market Rent Schedule** for pricing changes
- Manage **ILS Special Override** for marketing

**Key Functions:**
- **Pricing Analysis** — Market rent vs actual rent analysis
- **Renewal Management** — Lease expiration and renewal offers
- **Concession Management** — Specials and effective rent calculation
- **Marketing Integration** — Website and ILS pricing updates

---

### 🔧 **Engineering Teams**

#### Backend Engineers
**Primary Tools:** Yardi APIs, RentCafe APIs

**Key APIs Used:**
- **GetResidentData** — Resident ledger history
- **GetUnitInformation** — Unit data for applications
- **GetUserPropertyAccess** — User permissions
- **ImportResidentTransactions** — Charge and payment processing
- **RentCafe APIs** — Website integration and prospect management

**Integration Work:**
- **Flow App Integration** — Resident data and payment processing
- **Website Integration** — Floorplans, pricing, availability
- **Data Pipeline** — Yardi to Snowflake for analytics
- **API Development** — Custom integrations and automations

---

## Critical Workflows

### Move-In Process
1. **Leasing** creates application in CRM Flex
2. **ScreeningWorks** processes background check
3. **Leasing Manager** approves application
4. **Assistant PM** processes move-in in Voyager
5. **Moved** syncs with Yardi for checklist
6. **Maintenance** completes unit readiness
7. **Front Desk** provides keys and access

### Move-Out Process
1. **Assistant PM** processes move-out in Voyager
2. **Maintenance** completes inspection via Google Form
3. **Assistant PM** creates move-out statement
4. **Deposit Accounting** processes refund
5. **Accounting** cuts and sends check

### Invoice Processing
1. **Vendor** submits invoice via VendorCafe or email
2. **AP Team** codes and routes through workflow
3. **Property Manager** approves based on amount
4. **Controller** approves high-value invoices
5. **AP Team** processes payment via ACH or check

---

## System Integration Points

### Yardi ↔ Moved
- **Sync:** Nightly data synchronization
- **Purpose:** Move-in/move-out checklist management
- **Key Data:** Resident info, unit status, requirements

### Yardi ↔ Carson/Flow App
- **Integration:** Real-time resident data
- **Purpose:** Resident portal and payment processing
- **Key Data:** Ledger, payments, access control

### Yardi ↔ Sigma
- **Integration:** Data pipeline to Snowflake
- **Purpose:** Advanced analytics and reporting
- **Key Data:** All operational and financial metrics

### Yardi ↔ Waves
- **Integration:** Work order synchronization
- **Purpose:** Maintenance request management
- **Key Data:** Work orders, completion status, charges

---

## Common Issues & Solutions

### Data Sync Problems
**Issue:** Voyager and Maintenance IQ out of sync
**Solution:** 
1. Check last sync time in Maintenance IQ
2. Contact Yardi Team if >24 hours
3. Manual reconciliation if critical

**Prevention:** Regular data validation checks

### System Performance
**Issue:** Yardi running slowly
**Solution:**
1. Clear browser cache
2. Check internet connection
3. Contact Yardi Team if persistent
4. Use alternative browser

### Access Issues
**Issue:** Can't access specific module
**Solution:**
1. Check user permissions with Yardi Team
2. Verify property access rights
3. Contact Department Lead for role verification

### Login Problems
**Issue:** Can't log into Yardi
**Solution:**
1. Reset password via Yardi Team
2. Check if account is locked
3. Verify correct URL and property selection
4. Contact Yardi Team for account issues

---

## Common Pain Points & Solutions

### Data Sync Issues
**Problem:** Voyager and Maintenance IQ out of sync on completed work orders
**Solution:** Regular data validation and manual reconciliation

### Manual Processes
**Problem:** Variance report compilation takes 3-4 hours monthly
**Solution:** Automated reporting and template standardization

### Limited Notifications
**Problem:** No email alerts from Yardi for critical events
**Solution:** External monitoring and manual check processes

### Search Limitations
**Problem:** Voyager search is less powerful than CRM Flex
**Solution:** Use CRM Flex for resident searches, Voyager for reports

---

## Best Practices

### Data Entry
- Always use **Quick Charge** for resident fees
- Update **Resident Profile** with current contact information
- Add detailed **Memos** for resident interactions
- Use **Attachments** for important documents

### Reporting
- Set up **Favorite Reports** for daily use
- Export to Excel for detailed analysis
- Use **Hyperlinks** to drill down into details
- Cross-reference with **Sigma** for validation

### Workflow Management
- Process **Workflow Dashboard** daily
- Add detailed **Notes** to invoices
- Use **VendorCafe** for all vendor management
- Follow **Escalation Protocols** for approvals

---

## Property Size Considerations

### Small Properties (<100 units)
- **GM:** May handle both GM and AGM functions
- **Leasing:** Single Leasing Agent may handle all functions
- **Maintenance:** Limited Maintenance IQ usage, focus on Voyager
- **Support:** Front Desk handles most resident inquiries
- **Key Focus:** Essential functions only, simplified workflows

### Medium Properties (100-300 units)
- **Standard roles:** Follow guide as written
- **Backup coverage:** Cross-train key functions
- **System usage:** Full Yardi module utilization
- **Support:** Dedicated Support team with specialized functions
- **Key Focus:** Full Yardi capabilities with backup procedures

### Large Properties (300+ units)
- **Specialized roles:** Dedicated team members for each function
- **Advanced features:** Full utilization of all Yardi capabilities
- **Reporting:** Enhanced analytics and custom reports
- **Support:** Multiple specialized support roles
- **Key Focus:** Advanced features, automation, and optimization

---

## Weekend & After-Hours Access

### System Availability
- **Yardi Voyager:** 24/7 access
- **CRM Flex:** 24/7 access
- **Maintenance IQ:** 24/7 access
- **Support:** Yardi Team available via Slack #yardi-support

### Emergency Procedures
1. **System Down:** Contact Regional Operations immediately
2. **Data Issues:** Contact Yardi Team via Slack
3. **Critical Functions:** Use backup procedures (paper-based)
4. **Escalation:** GM → Regional Operations → Yardi Team

### Backup Procedures
- **Move-ins:** Paper-based checklist if Yardi unavailable
- **Maintenance:** Phone-based work order management
- **Invoices:** Manual approval process with email confirmations
- **Payments:** CheckScan backup with manual ledger updates

---

## Training & Onboarding

### New Team Member Checklist
- [ ] **Yardi Team Setup** - User account and permissions
- [ ] **Role-Specific Training** - Department-specific workflows
- [ ] **System Access** - All required modules and functions
- [ ] **Backup Procedures** - Emergency protocols
- [ ] **Escalation Paths** - Who to contact for issues

### Skill Development Path
1. **Basic User** - Essential functions for role
2. **Intermediate User** - Advanced features and reporting
3. **Power User** - Cross-functional knowledge and training
4. **System Admin** - Yardi Team level access and support

### Training Resources
- **Yardi Team** - System setup and basic training
- **Department Leads** - Role-specific workflows
- **ClientCentral** - Yardi knowledge base
- **Internal Documentation** - Flow-specific processes

---

## Neighbor Impact & Experience

### How Yardi Improves Neighbor Service
- **Faster Response Times** - Quick access to resident information
- **Accurate Billing** - Automated charge calculations and payments
- **Better Communication** - Centralized resident data and preferences
- **Proactive Service** - Maintenance tracking and preventive care

### Neighbor-Facing Functions
- **Move-in Process** - Streamlined requirements and documentation
- **Maintenance Requests** - Real-time status updates and tracking
- **Payment Processing** - Secure, convenient payment options
- **Lease Management** - Digital lease signing and document storage

### Service Recovery
- **Data Issues** - How to handle Neighbor concerns about billing
- **System Downtime** - Communication protocols for service interruptions
- **Access Problems** - Alternative methods for critical functions

---

## Training Resources

### New Team Members
1. **Yardi Team** — System setup and basic training
2. **Role-Specific Training** — Department-specific workflows
3. **ClientCentral** — Yardi knowledge base and support
4. **Internal Documentation** — Flow-specific processes

### Ongoing Support
- **Yardi Team** — Technical issues and system updates
- **Department Leads** — Workflow and process questions
- **ClientCentral** — Self-service support and documentation

### Screenshots & Visuals
- [Placeholder: Voyager - Community Dashboard view]
- [Placeholder: CRM Flex - Dashboard interface]
- [Placeholder: Maintenance IQ - Mobile app interface]
- [Placeholder: Workflow Dashboard - Invoice approval screen]
- [Placeholder: CheckScan - Payment processing interface]

---

## Future Improvements

### Planned Enhancements
- **Workflow Dashboard** improvements for H2
- **My Approvals** interface for better approval management
- **Invoice Register Dashboard** enhancements
- **Maintenance IQ** sync improvements

### Integration Opportunities
- **Automated Reporting** — Reduce manual variance report compilation
- **Real-time Sync** — Improve data consistency across systems
- **Mobile Optimization** — Better mobile interfaces for field teams
- **API Expansion** — More robust integration capabilities

---

> This guide serves as the definitive reference for how Flow leverages Yardi across all teams and functions. For specific technical questions or system issues, contact the Yardi Team or refer to ClientCentral for additional resources.
