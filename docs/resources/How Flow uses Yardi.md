# **How Flow uses Yardi**

Authors: [Harrison Smith](mailto:hsmith@flow.life)   
Last Major Revision: Feb 15, 2024  
Related Documents: [Yardi: Feature \<\> Business Function Importance Map](https://docs.google.com/spreadsheets/u/0/d/13O5BLxcCKWxYFkBzA7EsrcwtecraN4i8IfQlkITg5ec/edit)  
Status: **Draft** | In-Review | Final

## **Summary**

This document comprises detailed notes from internal user research sessions with team members from every function of Flow that engages with Yardi. In each session, the goal was to understand and capture how that individual uses and depends on Yardi to fulfill their responsibilities. Throughout, I sought to gather a sense of their key pain points, and the things they like most about the system. Each session was recorded, and you can find the recordings linked below. 

Most importantly, the information below is distilled into a map of every feature of Yardi we use by its importance to each function of the business. Importance is subjective, of course. However, the ‘Importance Scoring’, if you will, is based on how critical the feature or functionality is to the responsibilities of that function of the business, based on the interviews below. You can find this map here: [Yardi: Feature \<\> Business Function Importance Map](https://docs.google.com/spreadsheets/u/0/d/13O5BLxcCKWxYFkBzA7EsrcwtecraN4i8IfQlkITg5ec/edit).

## **Meeting Recordings**

[Stakeholder Interviews](https://drive.google.com/drive/folders/13RMBh7tiHNZyXAlTjXeiQDXxh_vszMo9?usp=sharing)  
[Yardi Team](https://drive.google.com/drive/folders/1lB5Y3cZF0GNWKcIvdxM9y0pV1xFwx2TN?usp=drive_link)  
[Property Management](https://drive.google.com/drive/folders/1BcuEWvggQQzMnN2tmBfSrRg6kL8P08yM?usp=drive_link)  
[Leasing](https://drive.google.com/drive/folders/1dX90AgXEe5OCN_xbzZHd3sCzGcyVOu_j?usp=drive_link)  
[Support](https://drive.google.com/drive/folders/11cxOcOruzoAL64nDE0Zz4NMeMUh1Gpo5?usp=drive_link)  
[Facilities & Maintenance](https://drive.google.com/drive/folders/1UBr25Lz3ipA8-KoSh2M2plxsPFMfbTs5?usp=drive_link)  
[Pricing](https://drive.google.com/drive/folders/1XPNEhMxsm6vBAAPoxoZurGf4yD5Oke9o?usp=drive_link)  
[Property Accounting](https://drive.google.com/drive/folders/1OQHAfElMiOGpsJoFnkTtybHie8GComde?usp=drive_link)  
[Physical / CapEx](https://drive.google.com/drive/folders/1hEwEMqHU8tMpwIP_M6XyxUKHmSgbaZPL?usp=drive_link)  
[Data & Analytics](https://drive.google.com/drive/folders/1I-QInqeQMQb7QK12oRLIKAaqa58GllG4?usp=drive_link)  
[Engineering](https://drive.google.com/drive/folders/1L8EZhzZo56cQRS9AGUmCiClf3KBtWIar?usp=drive_link)

## **Meeting Notes**

## **Yardi Team**

### **Hila \- Head of Yardi**

* Hila  
  * Voyager: the grandfather of everything  
    * Reporting  
    * Ledgers  
    * What can you not do in Voyager that you can’t do in other modules?  
  * CRM Flex  
    * Leasing agents won’t use Voyager \- they’ll use CRM Flex and access Screening Works through CRM Flex.  
  * Maintenance IQ  
    * Used by Maintenance Techs on their phone in app-form  
  * ProcuretoPay (in Elevate and Voyager)  
    * Approval for maintenance orders  
    * What is elevate?  
  * Lots of tools under ‘Elevate’  
    * You can access everything in Voyager but Elevate is the nicest way to interact with the system  
  * AP/AR will use Elevate  
  * Client Central \- knowledge-base for Yardi and support portal  
  * Marketing done via Site Manager  
  * Business functions using Yardi  
    * Leasing  
      * Add Anthony  
    * RX  
    * Maintenance  
      * Add Andy  
    * Property Management  
    * Asset Management  
    * Revenue  
    * Analytics  
    * Engineering (API)  
      * Talk to [Arjuna Sondhi](mailto:asondhi@flow.life) about payments integration  
    * Website  
      * Marketing and management of the property websites (and resident apps/rent payment portals)  
    * Building marketing  
    * Accounting  
      * Speak to Robert  
        * Controllers  
        * Vs Evelyn and Negesti doing AP/AR  
    * CapEx   
      * Worth a quick call with Ayda  
      * Using it for invoices  
  * What challenges is your team typically dealing with?  
  * Residents have their own ledger where their charges go  
    * Ledgers are per resident  
      * But based on their lease  
      * Hila: tcode won’t change if someone transfers units  
  * Talk to Yardi team about how they manage building marketing 

### **Jamie \- Yardi Frontend Engineer**

- Team works from their Jira support ticket board, assigning tickets to themselves based on their specialities.  
- Working across all the modules, though most of the admin functionality is in Voyager.  
- Typical Admin Usecases:  
  - Adding GL Codes  
  - Formatting and building the Account Trees based on GL codes  
    - For most Financial Reports we have a custom account tree. If the option is not there we use the Yardi default.  
- Team also helps the business units to complete tasks that they could have completed themselves.  
- Team will also spend time correcting manual errors on the ledger eg. a double charge on a lease.  
- Transitions:  
  - Will load cleaned data in via an ETL report into Yardi.  
- Also upload Sonder rent payments through ETL.  
  - Bulk payments added to the ledger (for Commercial leases)  
- Roommates are able to pay rent and get the same app as any tenants  
  - Login to the app doesn’t change even if they transfer or get promoted  
- Will set up Floorplans for new Unit Types via RentCafe Sitemanager  
  - Content & Settings \-\> Floorplans \-\> Add a Floorplan \-\> Attach the unit type for that floorplan  
  - New Unit Types are added in Voyager directly  
- Integrations are set up via Voyager \-\> Interfaces \-\> Configuration \-\> Add an Interface Vendor \-\> Select vendors \-\> Apply the interface to a given property.

### **Llu \- Yardi Backend Engineer**

- Llu is essentially our Yardi plumber, making sure things run smoothly through the Yardi pipes.  
  - Anything that touches resident or staff experience  
  - Any data issues  
  - Reporting  
  - Automated tasks to take administrative burden off of the Staff  
- At its core Voyager is a big accounting database with other functionality built on top of it  
  - A product of it’s time eg. created for a nuclear household with a primary tenant  
  - In the real work multiple people can be on a lease, in Voyager the primary tenant is the first class citizen in terms of data and processes.  
    - Roommates have to be promoted to the status of a primary tenant.  
- Over time Voyager has been built upon to serve various usecases.   
- In the database there is one large table called Trans with over 100 columns with different types of transactions  
  - Register Report in Yardi lets you see all the transactions  
  - Consider this the master ledger for the entire system  
    - Work to the individual ledger from hPerson field  
- Every single charge is part of a batch  
  - By design  
  - Every charge has a batch number on it  
  - We post rent charges each day in a single batch  
- When people make payments they go into a batch  
- A batch is usually a set of common transactions  
  - Though you can create a manual match  
- In the scope of Voyager a tenant is a Lease  
  - If a tenant renews their lease they remain on the same ledger  
  - Roommates share the same ledger on the lease  
- Everything in Rentcafe CRM Flex is a more focused version of Voyager, focused on Leasing.   
  - Though in Voyager you cannot search as cleanly, at an individual level, as you can in CRM Flex.  
    - Much easier to search for documents; send invites to the apps; and see the relationship between different residents.  
    - Easier to find work orders at the individual level  
    - More focused on the resident experience, at least for support.  
- Llu transforms excel sheets into SQL statements to add term based pricing in bulk  
  - To do this manually you would have to go unit by unit via the CRM Flex  
- Llu produces custom reports and sets up reports in Voyager  
  - Including automated reports  
- Llu sets up the different Yardi modules, like ScreeningWorks or Procure to Pay  
- Llu also manages the Yardi file tree  
  - Attachments loaded in when we do a transition  
- Transitions:  
  - If the other management company uses Yardi, it’s 1-1  
  - If the management company uses a different software, their objects and tables need to be converted to our formats.  
  - There is a dark period when everything happens manually and in paper at the property (4-7 days)   
    - Takes time to bring everything in in ETL files  
      - Data dumps in Excel, CSVs, Json  
      - Manipulate them as necessary  
  - We use Redirect consulting services to support the transitions.  
- Elevate (focuses on particular modules)  
  - Included Maintenance IQ  
  - Payment Processing and Procure to Pay   
    - We use Yardi’s payment processor within the Rentcafe application  
    - Llu is not sure how the payment processor works

## **Property Management**

### **Dor \- Head of Operations & Revenue**

- Mostly use Voyager and the CRM  
  - Use the CRM to make sure the team is completing their responsibilities like clearing the queue; clean the MeetElise queue.  
    - Uses the CRM to hold the team accountable  
- Mostly use Voyager for Reporting  
  - Look at tour notes for all properties, ensuring the team adds notes and getting insight into the state of the leasing flow.  
    - For example, interested in the feedback on the converted RBBs  
  - Uses Voyager to cross-check Sigma  
    - BoxScore Summary  
    - Unit Availability Detail  
    - Rent Roll  
  - Also uses Voyager to analyze why trends look the way they do in Sigma  
    - Use Yardi to dive into the database  
- Doesn’t go into the ledgers very much, though will when we focus more on the Revenue number and less on Occupancy.  
  - Looks at the ledger every month in the financials  
- Uses AP workflows to approve marketing spend at the property level  
- People consider Yardi to be the truth because it is the source of truth, biasing us to not check for manual errors

### **Chris B \- GM**

* Voyager  
  * Property manager is critical to leveraging Yardi at the building \- sitting in the middle of the web  
  * Reports  
    * Set up favorite reports:  
      * Residential   
    * Leverage the calendar on the activities happening in the day  
    * Move-ins and move-outs show Johnny’s workload  
    * Don’t really use the unit reporting \- Sigma is better  
    * Exporting to Excel is used heavily  
      * Eg. exporting delinquency report; or vehicle report  
      * Used to filter for specific usecases and questions  
    * Daily Activity Report  
      * Focused on Month to Month  
    * Resident activity detail  
      * A load of individual reports  
      * Leverage for monthly renewal bonuses  
      * Leverage to cross reference with commission report from Leasing Manager \- number of Move-ins.  
    * Resident activity high level  
      * Core metrics over a custom timeframe  
      * Can go into detail from here and then use excel  
      * Each blue hyperlink allows us to go into a detailed report for each metric  
    * Eviction report  
      * Then export to excel and do the analysis themself  
    * BoxScore Summary  
      * Availability  
      * Resident Activity  
      * Conversion Rates  
        * Essentially a Leasing Dashboard  
    * For those who provide Notice \- we only find out why they provide notice after they move-out (their move-out reason)  
    * Favorite report: Unit statistics  
      * All the information I care about when it comes to our rent growth  
      * Market rent \- what we are offering  
      * Also gives you rent per square foot  
        * Always wants to know this  
      * Use this report over the Effective Rent report, which is sometimes wrong  
    * Other than for Occupancy, I don’t use Sigma  
    * 12 month occupancy never works  
      * Would be amazing to have  
      * Why is this?  
    * Concession burn-off is a really good report \- used to calculate how much we will spend on concessions each month  
      * Helps you know when to drop concessions off  
      * Will use every month if we are concession heavy  
    * Lease expiration \- used to try and offer longer or shorter leases to amortize expirations and even them out.  
  * Financials  
    * Use the Financials section to produce variance reports each month for the Accounting Team. Working with Robert on the Accounting Team.  
      * Adding notes directly in Yardi  
      * Notes on variance between budget and actual  
      * Notes on bills on General Ledgers are linked to in the variance report and used to add high-level notes for each line-item in the variance report.  
        * If the notes from the bill are reflected on the variance report it would save 3-4 hours at least on the days when this report needs to be compiled.  
    * General Ledger report  
      * Used to get into the detail of why we spend what  
      * Will often export to excel to be able to filter  
  * AP/AR  
    * Invoice Register  
      * Used to approve invoices that are added  
      * Important to add detailed notes  
      * Cross-reference charges with invoices  
      * If Chris is unsure, he screenshots and speaks with Evelyn to resolve it  
      * Does this daily  
  * Resident Support/Issue Resolution  
    * Use resident person record to get contact information to reach out to a resident and understand charges on their ledger  
    * Use work order function to check on the status of individual work orders when residents complain.  
  * Prospect Guest Card  
    * Used to verify different commissions \- eg broker commission invoice  
  * Not using Yardi to manage the Security team  
  * Never goes into other Yardi modules  
  * “I perceive it as an accounting platform for analytics.”  
  * I would love to know when elevators are being reserved; when vendors are coming to the property.  
    * More of the operations of the property

### **Johnny \- Assistant PM**

* ‘Sometimes you love it, sometimes you hate it’  
* Used to use Onesite, and found it to be more user friendly  
* Just use Voyager and occasionally ScreeningWorks  
* Perceives his role and making sure everything is recorded and accurate in the system  
  * Particularly the collections part  
* Every day, look at ‘Move-ins’  \- ‘future’ residents that need to be added to the system as a resident  
  * If someone is transferring units they shows up here  
  * Go to the move-in statement and check that it matches the system  
  * Once you hit the ‘Move-in’ function, they system produces the charges the resident needs to pay and we need to check if the move-in statement reconciles.  
  * Update the Agent to the Leasing Specialist  
  * From time to time the Leasing Agent will do the math wrong calculating Move-in charges  
    * Manually produce the move-in statements  
  * Need to select each charge to add them to the ledger  
  * After checking \- ‘post’ the move-in  
  * Then go back to the ledger and check everything is accurate  
* Process move-in cheques with the Yardi System Checkscan (only cashier’s cheque)  
  * Use Checks because we require certified funds  
  * ‘If you let someone pay online they can dispute that later on if they want to’  
* Also reconcile resident ledger charges using their profile eg. to see if they have a vehicle.  
* If a resident pays too much they will automatically get a credit  
* Yardi will automatically switch utility charges if a resident transfers.  
* Conservice is integrated into Yardi and they add utilities to the resident automatically.  
  * Conservice sends Johnny a report to review each month and once he gives them the green light they add the utilities to the system. Manual review.  
* Renter’s Insurance  
  * Assurant tracks policies for us  
  * Also review insurance on the data \-\> Renter’s Insurance interface.  
    * Double checking that we have received everything (before residents move-in)  
* Check the lease agreement (name, apartment number, lease dates)  
  * Check that the Early Termination amount is correct  
  * Check that the Lease has all the right addendums eg. pet addendums  
* Extremely manual and detail oriented  
  * Keep track of changes from this auditing in a google sheet  
* Move-outs  
  * Make sure we get the physical keys before moving them out.  
    * Ensure we don’t make the unit ready until they have truly left  
    * Just move the resident out (change of status)  
* Once a resident is Moved out, they move to the Deposit Accounting tab  
  * Close the ledger, close the account \- creating the move-out statement  
  * Try and complete within 5 days of the resident moving out  
  * Florida Law: resident must receive move-out statement within 30 days of moving out  
  * Check if the resident gave ‘proper notice’ (60 day notice, else 1 month of rent insufficient notice fee)  
  * Check that utilities are applied correctly up to the move-out day  
    * Check on the ledger  
  * Move-out statement generation: function \-\> Deposit Accounting  
    * Do it largely based on the history of the resident  
    * Initial scan to see if anything seems off, and then investigate by reconciling with Conservice  
    * Check maintenance inspection of the unit prior to completing the Move-out statement, applying damage charges as necessary.  
      * Inspection is completed by the technician via a Google Form, with responses in a Google sheet, including links to photos that are stored in the drive.  
      * The Assistant PM reviews the photos and makes the final judgment.  
    * Check the handwritten move-out form and verify that we have an address to send the cheque to and input that address to the Forwarding Address field.  
    * We send one cheque with multiple names if roommates are on the lease. To one forwarding address.  
    * Add Move-out statements to the resident’s account.  
    * Use Zendesk to communicate with the residents even post-move-out \- allows RX team to support with questions or issues.  
    * Accounting sends cheques to the residents.  
* Note: utility charges are two months delayed ie. in march you pay january’s utilities  
* Everyone comes to the Assistant PM for any lease related charges  
* Apply late fees properly on the 6th day of each month and then create three-day letters to pay or vacate (manually, posted on the door).  
  * To get the report of all residents with a balance (that haven’t paid their rent yet): Reports \-\> Receivables \-\> Residential Analytics \-\> Financial Aged Receiveables \-\> Summary type: Resident  
  * Uses this report to update a google sheet tracker (Delinquency) for each month and add notes.  
  * Have to actively seek out the information \- no alerts from Yardi  
  * No way to track delinquency over time or collection of late funds over time.  
    * Keen to see collection percentage  
  * Combine with the rent roll to get the month-to-date billing  
  * Roommates that are on the lease are equally responsible for every charge on the lease, regardless of how the Yardi interface shows the roommates.  
  * There is a lease, then a ledger  
* Use Yardi to send create notice to cure documents to residents

### **Roxana \- GM**

- Reporting in Yardi is my favorite  
- Lives out of Voyager  
- Resident activity is my number one priority  
- Alerts \- anything that happened yesterday that we didn’t do that we need to do today  
  - Nice feature  
- Team meeting with maintenance every morning  
  - 72 hours as a standard to close work orders  
  - Use the maintenance section to understand why work orders are open and plan the day with the team.  
  - Maintenance team calls residents who don’t give permission to enter. After 3 failed calls, close the work order and leave a note for the resident.  
- Unit statistics  
  - For the leasing team  
  - Discuss separately with the leasing team after meeting with maintenance  
- Don’t use many of the quick links below the date in the dashboards  
- Open batches \- money that needs to be posted  
- Completed WO Followup section  
  - Orlando calling residents to check they are satisfied with their work order.  
- Look at the calendar for appointments to ensure the leasing team is occupied all day  
- Roles report \-\> Payscan Approver  
  - Roxana pays the bills  
  - Pays invoice once per week on Tuesday  
  - Roxana is the only person that manages payables  
- Financial Analytics  
  - Budget comparison  
  - Enter notes for each line item  
    - Links to invoices above  
    - Hyperlinks take you to the invoice to add context  
  - “Yardi does financials very well”  
- Operations Analytics  
  - Unit Availability Detail \- pulled on a daily basis; units by status  
    - Able to go into each unit via hyperlinks  
  - Monday report to Chris etc.  
    - Operations report  
    - Leverage the BoxScore summary  
      - Summary of the property  
      - Filter by UnitType for detail, by Property for Summary  
- Work Order Analytics  
  - Look at Completed Activity, summarized by Category  
  - Understand how the team is spending their time  
- Use Maintenance IQ \-\> WO Analytics to produce Monday Operations report  
  - Discuss Monday report on Thursday operations report  
- Spend a limited amount of time looking at individual resident profiles  
  - Use Memos a lot to note interactions with residents  
    - Struggle to get the team to document conversations in the memo  
    - Sometimes the team will download email conversations and add them as an attachment  
  - Will look at the ledger and add quick charges  
- ‘I really don’t work in excel’ \- its ownership specific if they want specific reporting that Yardi doesn’t innately offer.  
- Pulling reports on Monday; processing invoices on Tuesday  
- Roxana executes leases for renewals  
  - Needs to go into Bluemoon to cross-check renewals that have signed their lease.  
    - Don’t work in CRM (where you can execute leases): use Bluemoon directly for renewals.  
  - Attach leases to the profile in Yardi  
- Walk property in the morning; emails in the middle of the day, reporting in the afternoon  
- “I don’t want to spend a lot of time reporting or using the technology, I want to be walking the property”

### **Michelle \- Assistant GM**

- Use Voyager every single day  
- Only use CRM if she is helping the leasing team with something  
- Check on Pending Applications  
- Always look at Move-ins, Move-outs, and Deposit Accounting  
- Move-ins  
  - Walk the apartments in addition to the Leasing team  
- Move-outs  
  - Do the move-out inspections with the Maintenance supervisor  
  - Run water, run the dishwasher  
  - Have 5 days to close out Deposit Accounting  
  - Have 15 days to notify the resident if we make a claim against their security deposit  
  - Note: rent responsible residents pay (and have a move out date) until their lease ends or we find someone to take over the lease.  
  - Confirmation \- keys returned or written \- to go into the apartment after they move-out  
- Deposit accounting  
  - Create the move-out statement of final charges  
  - Go to the post office every friday and send their move out statement (from Yardi) and a notice to impose claim (from their security deposit) via certified mail to their new address.  
  - Have to do everyone who moves out in a week in that week  
- Pull delinquency reports every day  
  - Receivable Analytics \-\> delinquency only  
- Post three day notice to pay on the monday following the first day of the month  
  - And close their online account  
    - Change via their profile \-\> Late Fee & Account  
  - Only take payment via a cashiers check  
- If residents don’t pay, evict them via their profile (initially set move-out date to next year because we don’t know when we will get them out of the unit, then update the move-out date when we do)  
  - Writ of possession (sheriff comes and takes back possession of the apartment)  
- Resident Analytics \-\> renTo give Roxana a better understanding of financials for her financials call  
- t roll to see the difference between market and actual rents week over week  
- Leverage slack to manage charges to existing residents (particularly over the weekend)  
- Add charges via the resident’s profile \-\> quick charge is a big functions we use (one time)  
  - Residents are asked to pay the one time fees in full immediately  
    - Until it is paid for we don’t give them things, even fobs  
    - If Michelle is here we get them to pay on the spot if they need something immediately  
  - Or add a Lease Charge \-\> recurring charge  
- Attachments are really important  
  - Team labels attachments in the ‘Type’ field to organize appropriately  
  - Adding attachments is extremely time consuming in Voyager (easy in CRM)  
  - Eg. for notices to enter posted on door, Michelle scans the file and then adds it to the profile  
- Michelle adds renewal proposals (for the leasing team) manually  
  - Proposed rent data is used to populate the renewal letter to be given to the resident  
- Residents \-\> Residential Correspondence  
  - Renewals and small balances (less than $1000)  
    - For small balances we don’t give them a 3 day notice to pay, we just ask them to pay as soon as possible  
  - Create Renewal Letter, filter for lease months, generate documents \-\> leverages proposed rent data from above.  
  - Then attach documents and show on portal and email documents (don’t like using this function because it’s not friendly, instead the team calls and emails more personably).  
    - Also print out the renewal offers and post them on the door  
- For residents that provide notice more than 75 days in advance, the team doesn’t put them on notice in Yardi, so Jason generates an offer for them and the team offers them a renewals.  
- If anyone NSFs twice, we only let them pay in certified funds  
- Yardi System CheckScan  
  - To scan in cashiers check  
  - People really like the checks  
    - Particularly older residents  
    - Also allows people to avoid service fees  
    - People just come down and put checks in a box  
  - We accept personal checks as well  
  - Checkscan won’t let you post the batch until the calculation total is accurate  
    - Or if you don’t print the report  
  - Once posted, payments are posted on the resident’s portal and ledger  
- Use Resident Payment Method report to check the residents that need to be switched from cash only back to any payment method  
- Set residents in eviction to ‘Do not accept’ payments because we need the full amount from them including legal fees. If we accept a $ from them, their eviction is canceled.

## **Leasing**

### **Peter D \- Leasing Manager**

* Yardi is our CRM platform for the sales team \- managing leads and appointments and availability  
* CRM  
  * First thing in the day \- appointments, guest cards  
    * Check calendar via CRM and make sure the team is aware of how many appointments they have  
    * Always have to actively seek out information \- Yardi doesn’t send emails or notifications  
    * Orange means the appointment is assigned to an agent, blue means assigned to MeetElise  
  * Outside of notes on the appointment, there’s no way to verify if a tour is confirmed.  
  * CRM queue used to work leads and do quality control  
    * Listen in on call recording  
    * Hosts all our emails   
    * No way to separate out prospects and residents in the queue  
      * Residents should email via Zendesk (forward emails in CRM to Zendesk)  
    * Will assign items in the queue. Agents can assign items to themselves in the queue.  
    * Limited analytics for quality control  
      * No idea of who answers the phone, or how quickly agents clear their queue, total call volume (receive from Ringcentral in an email)  
    * See multiple properties but can filter to a single property  
  * Dashboard \- operate from here most of the time  
    * Occupancy  
    * Leasing Activity  
    * Documents \- work out of this tab a lot; provides the stage an application is at in the queue.  
      * Can’t see this view elsewhere  
      * Use to facilitate and coach the team to make sure we are following up.  
  * CRM has functionality to countersign leases  
    * Proofread the document  
  * Leasing Manager becomes involved when an applicant is ready for approval  
    * Screening completed, proof of income documents put together, application completed  
    * Looking at documents through Voyager (guest card) \- reviewing attachments that an Agent has flagged as important for approving the applicant.   
    * Also verify co-applicants. Primary tenant is whoever inputs their name in the application first.  
    * Then go to ScreeningWorks and review the status of the application.  
    * If things don’t seem to look right, review the application form and their employment data.  
      * Occurs 5-10% of the time  
  * Only use ScreeningWorks to verify that an applicant meets the criteria  
  * For renewals  
    * Use CRM to reach out to residents and countersign all renewals (in Leases to Countersign)  
  * For commissions  
    * Dedicated Agent Performance report in CRM  
* Voyager  
  * Prefer Voyager because it’s a lot more black and white and granular. Very straightforward for reporting, with more detail.  
  * As a manager a lot of the job is reporting and so he uses Voyager  
  * Calendar in CRM is more accurate than in Voyager  
  * Regularly pulls BoxScore (key metrics for Leasing) and RentRoll  
    * Will often download reports and filter/perform calculations in Excel  
    * Eg. ‘what is the average rent we are receiving for x unit type?’  
      * Often Dor, Operations teams trying to get insights on the ground  
  * Analyze availability and current and future available units   
    * In order to empower the team to give alternative solutions to prospects that they might not have been able to see on the website.  
    * And current evictions \- so we can entertain the possibility that that unit will be available soon.  
  * Commissions and bonuses  
    * Use BoxScore summary; download Resident Activity report for new move-ins and reconcile with dedicated Agent Performance report in CRM.  
    * Need to ask the leasing agents to verify the roster

### **Adrian \- Leasing Specialist**

- Use the CRM more. Use Voyager only if there’s something the CRM can’t do.  
- Big asset that the dashboard shows our numbers clearly.  
- Always check to see what we have for the day, and in the afternoon preempt the upcoming tours for the next day, checking in with them.  
- Split the tours in the morning  
  - If a leasing specialist sends a reach out to an open prospect, they claim that prospect  
- Use the textboss app to communicate with prospects via text and CRM to send emails.  
  - Once a prospect is here we give them a personal number to text with us  
  - Emails are preset with templates  
- Yardi will show multiple profiles if someone inquires twice, leading to duplication.  
- Clear out the queue every day  
- CRM does ‘matches’ on names to see if there are duplicated profiles.  
- Take web requests and create Guest Cards, inputting manually from the lead eg. from Zillow.  
- Using the search function all the time to look up prospects and cross check past prospects with a new prospect in the queue.  
- Use SiteManager email functionality via the CRM to communicate with the property.  
- Reports:  
  - Rentable Items Directory to see what non-unit items are available to rent out like storage or bike storage.  
- Use Voyager to understand current availability  
- Always have to cross check the calendar in CRM and Voyager because sometimes there are discrepancies.  
- Managing applications occurs individually in each guest card  
  - Sending the residents the lease, adjusting rental options, adding occupants  
- Adding occupants \-\> don’t choose occupant type (demographics should be calculated)  
  - Will put parents as Roommates (considered as Leasee) if the parents are paying the rent (and sometimes don’t make 5x rent) or providing supplemental income (instead of putting guarantor \- if a guarantor isn’t paying rent)  
- Select and change units through the guest card  
- Will do a one-time courtesy swap to change to another apartment without an application fee.  
- Applications  
  - Send for screening within one day of the prospect applying. The prospect will get a link from NovaCredit to be screened. Once accepted, Adrian will draft the move-in statement and send it to Peter D to be approved.  
  - Attach all documents to the guest card in CRM.  
  - Able to manually update application forms (or add to them with additional info)  
- Becomes annoying to change small details because you have to update those details at each manual step.

## **Support & RX**

### **Eyad \- RX Director**

- As a resident directory  
  - To confirm if someone is a resident and get their contact information to reach out to them  
    - Hyperlink in the profile to call them with one click (CRM Flex)  
- Working predominantly from the CRM Flex  
- Use the CRM if a resident is booking an event space \- notifying Johnny to add amenity booking fees to the ledger.  
- Mainly using it as a reference to support workflows taking place in Zendesk.  
- Occasionally reference reports: Demographic, Unit Availability  
  - Eg. is there anyone in the building that works with this company  
- Anything resident-related that pertains to community experience like Community Commerce, or Events, occurs outside of Yardi  
- Often preferred name isn’t set up properly  
- Use it to confirm the lease status of a resident that wants to engage with Community experiences and host events.  
- Use CRM to look at work orders that residents inquire about.

### **Ria \- RX Manager**

* Looking up information when residents move-in or have a problem or a question (eg. charges)  
  * Work orders  
  * Vehicles  
  * Roommates  
* Create addendums to the lease  
  * Currently we only generate the Notice to vacate  
    * Form does give residents text lines that they can fill out  
    * Most people are not very willing to provide a reason why they are moving out  
  * Do this through CRM  
    * Profile \-\> documents \-\> one-off documents \-\> manage documents  
      * Doesn’t work 80% of the time and have to go through Bluemoon directly  
      * Integrated to Bluemoon  
      * Hard to find addendums and documents attached to people in Voyager  
    * Forms don’t transfer over when residents transfer  
* CRM vs Voyager comes down to personal preference  
* ScreeningWorks response appears on the Guest Card so the team views that to respond to queries about the status of applications.  
* Use Roommates section of CRM a lot  
  * For example for lock-outs to see who is authorized to go into the unit  
* Lockouts is done through Voyager  
  * Verify that the person who says they are locked out is a resident  
* You can see in Attachments in Voyager which forms are available for the individual to see in their portal (app or website)  
* Use CRM to view the resident’s portal directly  
  * When helping to troubleshoot if a resident can’t find something or understand something in their portal  
  * ‘Resident Services’ pulls up their account as if they are logged in  
  * Most of the time focused on troubleshooting payment accounts on their portal  
* Reading ledgers  
  * When residents transfer they get a new record, ledger, and t-code because they are closing an account.  
  * Typically we have to return their deposit to them  
  * Sometimes there are issues with fees on a resident’s ledger \- will export to excel or a pdf and then analyze and speak with Assistant PM.  
  * Read ledgers if someone makes a late payment and wants the fee waived, which we do as a courtesy one time and therefore need to check their ledger.  
* Use Voyager calendar to plan appointments (tours), move-ins and move-outs every day  
  * And contact people to schedule their move-ins  
  * Often they use voyager to check on the status of their security deposit  
    * How much they will be refunded and when the cheque was cut in New York  
  * Takes 30-40 days after a resident moves out to get their deposit back to them  
* Vehicles  
  * Yardi and our camera system are integrated  
  * If a vehicle is registered in Yardi, they will get a permit in PPM  
    * Takes about 12 hours to create the permit  
  * Registering a vehicle means adding it to the Vehicle Information area in their profile in Yardi  
    * One vehicle per leaseholder  
    * Can’t have non-occupants using the garage without paying the fee  
    * Verification of documents takes admin work  
      * We currently require vehicle registration documents or proof of being listed on insurance as an authorized driver  
        * Important for security and auditing cars in the garage and working with police.  
* Add memos in Yardi if a resident is involved in an incident  
  * Use zendesk for general issues  
* Use Yardi to add documents for the resident as they go through their Lease (working with Johnny).  
* Use CRM typically to add charges  
  * Profile \-\> Activity \-\> Charge \-\> Add charge codes  
  * Don’t need approval for small charges that are within a policy like Key Charges  
  * For larger concessions goes back to Johnny.  
* Typically use Voyager mostly to pull reports.  
* RX team members involved with Renewal use CRM to generate renewals  
  * Do the paperwork for transfers, but Peter D implements them in Yardi  
  * Generally we use paper forms for anything that doesn’t work directly with Bluemoon  
* Work orders  
  * Getting regular reports of do-not-enter work orders to schedule maintenance based on the resident’s preference  
  * Look up Work Orders when residents inquire about status  
* Reporting  
  * Pull move-in move-out reports and send them to hotwire so wifi is transferred for different units and set up before residents move in.  
    * Automated  
  * Pull resident detail report on a monthly basis to make sure we have contact details for each person theoretically in the building.  
  * Parcel pending will get updated rent rolls daily   
  * PPM get vehicle information reports daily/multiple times per day  
* Yardi integration with Carson is used to troubleshoot issues with Carson account access

### **Bobbi \- Resident Support**

* ‘Yardi is one of my sidekicks’  
* Use CRM because it’s an easier look and trained on the software  
* Resolving issues with charges, eg. for vehicles  
  * Note: for rental vehicles, they need to be added directly to PPM  
* Level 1 support: trying to solve the problem using information in Yardi, and escalating where appropriate.  
  * Escalate if residents won’t accept the answer provided by the RX Team  
* Providing lease charge information to residents if they inquire about charges or inquire about potential charges if they break their lease.  
  * Make an internal note in zendesk if a resident decides to move out.  
* Look up the Move-out statement to respond to inquiries about Move-out charges/deposits.  
* If there is a complaint about a resident, look up relevant information about the resident in Yardi and make a decision about whether to ask the Assistant PM to serve the resident with a notice to cure.  
* Go to CRM to check on the status of work orders that residents inquire about.  
  * Responding on behalf of the Maintenance team.  
* Sometimes there are discrepancies between CRM and Maintenance IQ, and in those cases the team submits a ticket to the Yardi team.  
* Use Yardi to respond to inquiries from other properties that a past resident is applying to live in.  
  * Release information only if the other property has proof of approval/application.  
* Use the calendar in the CRM to review who is assigned to different tours to properly greet prospects and connect them with the leasing agent.  
* Use the prorated calendar in Yardi to calculate how much residents will have to pay for a new charge that month.  
  * Then tag Johnny in Zendesk to add the charge to their lease.  
* If a resident needs help uploading documents, the RX Team will upload for them.  
* RX Team will look at new Move-ins report to reach out to new residents and check they are satisfied  
* Use Rentcafe Sitemanager to update emails, support payment issues (reports: Payment Activity) with the Rentcafe app  
* Use Maintenance IQ if a resident is inquiring about a work order and it doesn’t appear in the CRM. Just using the dashboard to look up the status of a given order.

## **Facilities & Maintenance**

### **Andy \- Facilities & Maintenance Director**

- Using Maintenance IQ  
- Do weekly trends on how work orders are being managed  
  - Analytics of work orders completed, by whom, by category  
  - Completed by category does not align with completion not by category  
- Use unit turn dashboard to manage make readies  
  - Hitting start automatically creates work orders for cleaning, painting  
  - Use the Make Ready manager board  
  - For every unit turn the team has to call third parties, for example for painting  
- Make Ready Manager dashboard is is a project manager for Unit Turns  
  - Used to close out work orders, but really the team uses the phone app and goes through the work orders they need to complete.  
- Use work order dashboard to track work orders  
  - Current work orders sync properly with Yardi Voyager  
  - Look into why work orders are on-hold  
- Team updates statuses via the app  
- Use the vendor approval chain in Yardi itself \- we don’t tie vendor approvals to each work order.  
- We don’t use Approvals module  
- Categories get skewed when residents get the categories wrong  
  - Team needs to take the initiative to update the categories  
- Voyager and Maintenance IQ are out of sync on completed work orders  
- Only use Voyager for make ready trends to make sure units are turned within the 10 day buffer  
  - We average about 7 units a week fully turned, which is usually less than the number of move outs (at Society)  
  - Using:  
    - Residential Reports \-\> Unit Availability Details  
    - Projected Occupancy for number of move-ins and move-outs  
- We have a google form to compile Move Out inspection information each time someone moves out \-\> we get a google doc file that we use to determine what we bill back to the resident.  
  - Maintenance IQ doesn’t support journey from inspection to charges on the ledger.  
  - Need to be able to see the progress of a make ready at the unit level.  
- All Technicians have a specific role  
  - Some specifically do Unit Turns, others just do Work Orders  
  - In Society they use the Work Order Dashboard to see what is critical  
    - Have to review all the work orders to decide if they are critical  
      - Discretionary on whether the team updates work orders  
    - At Society the team picks up the work orders \-\> they don’t triage them or assign them  
- RX doesn’t have access to Maintenance IQ to understand the status of work orders  
- Use Voyager \-\> VENDORCafe  
  - Invite Vendor (need to know the email of the accounting person at the Vendor)  
  - Then determine the category of Vendor \-\> to determine the level of insurance they need to have  
    - Takes VENDORShield 3-4 days to verify  
  - Insurance company needs to upload the Vendor’s insurance (VENDORShield does not allow vendors to upload themselves)  
  - Can then track in VENDORShield the compliance status of a Vendor  
  - When a Vendor is not compliant but doing work, Andy is notified by the AP team and has to follow up  
  - If a Vendor is not in compliance, VENDORShield won’t allow us to pay them.  
  - The accounting team can override the liability depending on the nature of the work.

### **Orlando \- Facilities & Maintenance Manager**

- In the morning, start in Voyager. Look at pending work orders and make readies.  
  - Team will print the work orders in the morning at 7 individually for each technician  
    - Write on the service request the priority and notes  
- Use whiteboard in office to track cleaning for make readies  
  - Use the whiteboard to track all work  
- To edit service requests  
  - Edit \-\> Resolution \-\> Save \-\> Then add notes  
    - If we have a resolution to the issue, but it is not yet completed  
  - Then select complete when the issue is resolved.  
- Payscan Approver to do the initial approval for jobs completed by third parties \- then Roxana approves.  
  - Next step \-\> Property Manager Review or Reject with notes  
- Maintenance IQ doesn’t even work on his laptop  
- No real process around categorizing or prioritizing work orders  
  - Add the priority and category when a work order is completed  
  - Orlando trains the team on what’s an emergency and not  
    - Important because there is always someone on call \- 1 week for each person  
    - No document   
- No good way to track the status of a work order \- it’s either updated and open or completed and closed.  
  - Appears to be no field for status.  
- Team is not updating the priority and status \- only Orlando  
- When a work order is outstanding for more than a week, he contacts the resident and updates the priority and category and sends an update note.  
- Resolution \-\> Tenant Resolved means the tenant fixed the problem themself. In which case, we close the work order.  
- Uses this google form to complete Move-Out inspections and then manage Unit Turns \-\> [https://docs.google.com/forms/d/e/1FAIpQLSeFOjAr32BoQa8Qq1b7Qt3bJwTFbSy7fYya0kiIK-8jlblbtw/viewform?vc=0\&c=0\&w=1\&flr=0](https://docs.google.com/forms/d/e/1FAIpQLSeFOjAr32BoQa8Qq1b7Qt3bJwTFbSy7fYya0kiIK-8jlblbtw/viewform?vc=0&c=0&w=1&flr=0) 

## **Transitions**

### **Keith / Taylor  \- Transitions**

- Features that the Transitions Team is aware of and touch but don’t get used very much.  
  - Particularly communication templates within Rentcafe Sitemanager  
    - Team produced about 120 templates, but they haven’t really been used much  
      - Including legal documents that have been approved by Stella  
    - “We are missing an opportunity when it comes to communication with residents”  
    - Ideally we will have everyone communicating from the same source  
      - Currently we have many types of welcome letters etc.  
    - We should schedule and automate messages in Yardi eg. for holidays.  
    - Teams are using a variety of systems for mass communication  
- Challenge we have currently is the tracking and management of service contracts and compliance certificates  
  - Yardi has a platform that they’ve released but we don’t use it, we use an Excel sheet  
  - Doing it all manually  
  - Both service contracts and compliance certificates have expiration dates and we should be staying on top of their schedules.  
- Use Yardi for phone tracking numbers within ILSs  
  - We are limited when it comes to the phone tracking system  
  - Also limited in terms of calling out: You can’t call out of Yardi from the main property line  
  - Rentcafe texting functionality doesn’t work well enough so we use Ringcentral at SLO and Textbot at Caoba.   
  - Call tree is entirely messed up.  
- “Not using Yardi enormously, but whenever they pull reports the information is not the data that we need”  
  - Resident directory  
  - To get vehicle report from Yardi you have to pull the transaction report for parking from the general ledger.  
- Team was planning \- but didn’t implement \- to create a single property calendar that combined all events on the property  
  - Appointments  
  - Events  
  - Amenity Reservations  
  - Move ins/Move outs

## **Pricing**

### **Jason \- Director of Residential Revenue**

- If it didn’t happen in Yardi, it didn’t happen.  
- Fundamentally it serves to protect the landlord and the tenant by recording everything.  
- Use Voyager 96% of the time and then Rentcafe to ensure rents and specials are on the websites.  
- Looking predominantly at Unit Statistics  
- Utilize Residential Analytics reports a lot  
  - Projected occupancy: fact-based on recorded move-outs and move-ins in the future.   
  - Projected Occupancy number is number of occupied units  
  - Look at Rent Roll a lot  
    - Market vs actual rent   
  - Look at Lease Expiration report for renewals  
  - Download all of the reports to excel  
  - Aged receivables to work with the finance team on delinquency  
  - Also use the Unit Availability Detail report  
    - Most property managers are asked to print out this report every monday  
    - Property Managers and Leasing Managers work with the Maintenance Team regularly to stay on top of Make Readies and ensure we are turning Not Vacant Rented units asap.  
  - Uses Market Rent Schedule for price changing  
    - Export to excel  
    - Breakdown of market rent by unit type breaking out amenity fees (for higher floors etc) and comparing market rents to actual rents to compare asking to current rent paid by tenants in the building.   
      - Unit Type Rent (not including Amenity Fees, which don’t change) and Total Unit Rent (including amenity fees), Average Unit Rent (market rent including amenity fees), Average Resident Rent (what residents are paying)  
      - When we do a price change we do it at a floorplan level, not an individual unit level, because it messes up the system.  
        - There is a workaround: we override the advertised rent for a given unit.  
  - Uses the BoxScore Summary the most  
    - Particularly for the leasing funnel  
    - Prefers Yardi because it is Live  
  - Unit Amenities report  
    - Charges or discounts (tags) for different features of all units eg. balcony  
    - Summarized in Amenity Listing report  
      - Shows Past, Current, Proposed  
    - As a whole amenity tags are usually no more than a $500 variance  
      - Don’t want amenity tags to exceed a $500 difference between the same unit type  
- Looks at Financial Reports  
  - Often look at Budget Comparison (with PTD)  
    - Consider concessions vs budgeted concessions when setting pricing  
    - Though the Revenue team doesn’t create the budget, they try to guide the team to get as close as possible to their budget goals.  
      - Though they are less accountable than they might be if they were involved in the budgeting process directly.  
- To override rents, uses SiteManager \-\> Floorplans \-\> Find the Unit within its floorplan category \-\> Override Rent  
  - Will override the rent and set it for no matter what term and show on the website.  
- To adjust rent at the floorplan level, got to Setup \-\> Unit Type and adjust  
  - Then Update Proposed Amenities to see all units and amenity tags associated and the adjustments we have made.  
    - To update the Amenity Tags, Jason works with the Yardi team.  
  - Then Update Unit Rent \-\> Check the report  
  - If we have specials on Units, go to Specials tab and edit  
    - Able to edit if specials are for New Move Ins or Renewals or both and Show on Portal to make sure everyone can see the effective rent.   
  - Totally manual process \- have to manually type in all specials and all copy.  
    - Particularly with blanket concessions  
    - Lot of time  
  - Specials are based on start and expiration \-\> delete by setting the expiration date to today  
- Nudge Marketing  
  - Pop-up banners  
  - Click edit and update the HTML source code for the website using HTML code from Asa to edit the text in the websites  
- ILS Syndication  
  - Use the ILS Special override to update text in different ILSs  
  - Manually select all   
  - We will advertise the best special

### **Derek \- Pricing**

- Voyager  
- Pull pending applications from Community manager dashboards to determine what our move-ins are looking like  
- Scheduled lease renewals  
  - Pasting into Excel  
- Occasionally check pending make readies but have low trust in the data  
- Analytics \-\> Operations \-\> Residential  
  - Rent Roll  
  - Rent Roll with Lease Charges  
  - Unit Availability (rarely use)  
  - Resident Activity (high use)  
    - Pull down units that have given notice and what date they gave notice, along with early terminations.  
  - Lease Expiration report  
    - To get Month to month data  
    - Good for expiry curve  
  - Unit Availability Details  
    - For Days Vacant  
  - BoxScore Summary  
    - Used for traffic data  
      - Consider the impact of pricing changes  
  - Concession Burn Off  
    - Used to calculate effective rent  
  - Don’t have to put together any excels for pricing now we have the Sigma tool  
    - Rent Roll  
    - Concession Burn Off  
    - Month to Month  
    - Lease Renewals  
  - Unit Amenities Report  
    - List outs all the amenity tags \-\> used for pricing  
- Financial Reports  
  - 12 Month Income Statement  
  - Cash Flow Statement \- 1 month period for cash flow to make sure each month ties to the last month  
  - Always use the commercial and residential combined codes

## **Property Accounting**

### **Eyal \- Head of Property Accounting**

- We use Yardi for everything  
- Mostly use Yardi for creating the monthly financials  
  - Focused on the P\&L  
    - We have set it up using a specific design for a chart of accounts in Yardi to define how we show our P\&L  
    - We accrue bad debt for tenants that are delinquent for over 60 days  
    - We can create and allocate charge codes to specific accounts within the chart of accounts  
      - Working with the Yardi team to create codes and make sure the mapping is correct  
    - Majority of the P\&L is automatically generated by Yardi  
      - Including all the automated charges like late charges  
    - We manually upload payroll data into Yardi every pay cycle  
      - Done by the Property Controller  
    - Contract Staffing requires us working with the AP team  
      - Evelyn uses VENDORShield to vet the vendors  
        - We have defined different classes of vendors, with different liability requirements based on risk.  
          - All managed in Yardi  
          - Sometimes takes weeks until a vendor is vetted  
          - Constantly discussing vendors with Operations and deciding how much insurance is necessary  
        - When Vendors are set up they are allocated a GL account  
    - Once workflows are complete to approve invoices, an entry is automatically created in the ledger  
      - We only create manual entries when we need to accrue for things manually that relate to a given month (that haven’t been invoiced for yet).  
    - For utilities, Yardi accounts for tenant vs property charges in the P\&L automatically  
    - Interest, taxes  
    - We use a 27.5 year amortization period \-\> set this up in Yardi and recorded automatically  
    - Yardi also records depreciation automatically  
  - There is a Yardi invoice email (one email) for all our properties that automatically assigns invoices to our properties.  
  - We have approval workflows set up in Yardi for different types of vendor  
    - If it’s over $10,000 Eyal has to approve  
    - If a vendor asks why they weren’t paid, we can see in the workflow.  
    - Every time an invoice is submitted it has to be approved  
    - Every workflow has an originator  
      - The vendor or someone onsite that pushes the invoice to Yardi  
      - Finance works with the vendor owner \-\> the person that can speak to the performance of the vendor  
    - Workflows are being checked by many people every couple of days  
      - Using their Workflow Manager Dashboard  
    - Property Manager included in essentially all workflows  
    - We have a separate workflow for capital projects  
  - Also uses the Aged Receivables to get a good understanding of our delinquency by tenant  
    - Also opens the resident ledgers to see why there is a balance due  
      - Particularly monitoring concessions and checking the tenant’s lease  
      - Cross-checking the Assistant PM’s work  
  - Use Receivable Analytics to pull tenant evictions and our debt related to the evictions  
  - Financial Reports \-\> Balance Sheet  
    - Uses this a little bit less because he looks at cash in the bank account  
    - Yardi is the only place we are managing the property’s balance sheet

### **Robert \- Property Controller**

- Overseeing the property’s financial reporting  
  - Approving invoices and building receivables  
  - Maintaining the financial statements  
- Mainly Voyager  
  - Occasionally ClientCentral  
- Mostly working directly in Yardi, not Excel  
  - Just using Excel for visual manipulation  
- Financial Reports \- predominantly reviewing  
  - Income Statement  
  - Budget Comparison  
    - And with PTD  
    - Able to look into invoices to see if they make sense and if we need to reclass or make reclass or make adjustments  
      - Eg. if painting supplies was coded to cleaning supplies  
    - Weekly  
    - Review variance notes  
  - Cash Flow  
  - 12 Month Actual to Budget  
  - Balance Sheet  
  - Aged Receivables report  
  - Budget comparison most important because all others feed off of it  
- Upload budgets into Yardi  
- Create charges for tenants  
  - If Johnny is unsure (residential)  
  - Robert does all charges for commercial   
- Create a batch receipt for incoming payments that we don’t get a receipt for  
  - Mostly specific for commercial tenants  
  - Have to do manually for all commercial tenants  
    - When they pay via ACH  
  - Same thing for Landing  
- Yardi and the bank are not connected directly other than in the Rentcafe Portal  
- We almost never create payables manually  
- Use the Payables section to process payments and cut cheques  
  - Once you commit a cheque you have to process it  
    - Committing is just telling Yardi you are going to process a cheque  
    - Posting a cheque means you’ve paid it manually and are recording it in Yardi  
  - If a Vendor is set up for Yardi Bill Pay, we use Bill Pay. Otherwise we use cheques.  
    - Bill Pay is a backend system that plugs into the Process Payments module  
  - Everything over $3000 has to be signed by two people manually  
- Workflow Manager Dashboard  
  - To approve invoices  
  - Manually make sure it is coded correctly and then approve  
  - Every workflow is different \-\> depending on the type of invoice  
- G/L module is used to create journal entries on the books so it appears in the reports  
  - Reflect an activity in the ledger  
  - Happens often  
  - Eg. bank fee  
  - Reconcile the bank ledger with the GL on a daily basis  
    - Using the Bank Functions \-\> Bank Reconcile function  
    - Tracks the difference between the G/L and the bank statement  
      - Robert enters the bank balance manually in Yardi  
  - Completed bank reconciliation is due at the end of the month  
  - Done for receipts and deposits  
- Every payment takes 3-4 days to appear on the bank account  
  - Does Yardi take custody of the funds when people pay rent or pay an invoice?  
- Once we process payments Yardi sends the money from our bank account to the vendor  
  - How is it doing this?  
- “Think of Yardi as an accounting platform.”  
- Robert does most of the Commercial accounting  
  - When we get a new building Robert has to input all the lease information  
  - In addition to managing the commercial ledger  
    - Tenant billing  
    - Inputting units  
    - Receipts

### **Evelyn \- Property AP / AR**

- FOL Accounting Mento \-\> Reports \-\> Payables \-\> Payable Analytics Aging Report  
  - Gives an outstanding of what we owe every vendor and then she can decide who to pay  
    - Posted, approved invoices that are ready to paid  
  - Try to pay within 30 days of receipt  
  - Try to be as informational as possible  
  - Download to Excel to choose what to pay \-\> highlight what she is going to pay  
- Then go to Payables \-\> Commit Payments  
  - Shows all the invoices that need to be committed (to commit is to take the funds from the account)  
  - Able to search by HD Supply  
  - Each vendor has their own code and each invoice has a code  
  - Manually cross checking from highlighted Excel to the Commit page  
  - Commit Payments screen shows invoices in a somewhat random order that is not inline with the Aging report above, making the process more painful.  
    - In the aging report, invoices are grouped for each Vendor  
- We pay for Full Service PayScan  
  - Yardi scans invoices and automatically adds information from the invoice, including description  
  - If information is missing, Evelyn completes the fields  
  - All invoice is reviewed manually, even if Yardi scans it in  
- Payables \-\> Process Payments  
  - Shows all Committed payments   
  - For tenant refunds we send each property an email to make sure what we see to be paid and ensure it is the right amount.   
    - For instance the property will reach out to Conservice to understand what the resident should be charged for utilities for their month.  
    - Working with the Assistant PM  
  - Exceptions usually mean Vendor insurance has expired  
- Use VendorCafe heavily. VendorCafe includes VendorShield. Every Vendor should be invited through VendorCafe.   
  - We select the category of Vendor (person inviting them), determining the class of insurance  
  - We have a lot of Vendors that are exempt  
    - Particularly if we order things to be delivered from Vendors  
    - Eg. HD Supply  
  - If we are hiring a company to do work for a category we don’t work we can set up a new category.  
  - Have to look through the email thread to see who invited the vendor.  
  - VendorShield will reach out to all the applicable insurance companies to get their insurance details  
    - Have to wait for the insurance companies to respond  
    - Takes 2-3 days to do the verification  
  - Great service. In other property management companies, AP teams are tasked with verifying insurance themselves.  
  - Currently we can pay up to $2999 in ACH  
    - Vendors set up their details in VendorCafe  
      - Yardi send the funds once payments are processed  
  - Anything over $3000 needs double, wet signatures (Controller, Eyal)  
    - AP doesn’t sign the checks because it is a conflict of interest as they are cutting the checks  
- Dashboards \-\> Invoice Register Dashboard  
  - Vendors can upload invoices directly to VendorCafe or email them to our invoices email [FOL-invoices@yardi.com](mailto:FOL-invoices@yardi.com)  
  - For each invoice, the AP team is the first to interact with them, adding notes, setting Expense Type (to determine the approval workflow) and set the GL code for the invoice.  
  - Within the Invoice Register Dashboard you can see all the approvals in the workflow.  
  - When an invoice takes a building over-budget for their GL account, invoices are sent to the Controller and Eyal for approval.  
  - When an invoice is approved it ends up in the Aging Report  
- Dashboard \-\> PO Dashboard  
  - To see open purchase orders: asking for approval to spend some amount of money for an item.  
  - We don’t work with too many purchase orders. Mostly we use them for CapEx.  
  - We could do purchase orders for everything we buy.  
- AP is at the start and the end of the process  
- Use the Check Registers report to check everything we have paid via check.  
- Team uses Yardi to produce reports for Controllers and Eyal on a weekly basis  
  - Aging Report  
  - Purchase Orders Report  
  - Essentially a gentle nudge to approve to get vendors paid

## **Physical / CapEx**

### **Ayda \- Head of CapEx Projects**

- Ayda manages all Capital Improvement projects  
- We manage our budget through an Google spreadsheet for each property  
- When we are ready to begin the projects, we begin requesting Purchase Orders  
- We connect the spreadsheet with Yardi using the index of items in the spreadsheet as GL codes  
  - Each project has a GL code  
- In Yardi, Ayda approves purchase orders submitted against a budget and approving the invoices that are booked against the purchase orders.  
  - Roles \-\> Payscan Approver \-\> Workflow Dashboard  
  - Purchase order include a description of the work, the amount, quantity, etc.   
  - Then cross checks the details with the invoice  
  - We use comments in the google spreadsheet to track progress towards a budget line item  
  - If everything looks good, approve the purchase order  
  - When the vendor completes the work, they submit an invoice to be paid.  
    - Invoice has to be within 7% of the purchase order to be allowed to be paid.  
- Vetted vendors can submit invoices directly into the system and if we don’t have a purchase order we have to back input them.  
- Also uses Yardi to register Vendors through VendorCafe.  
- Uses Yardi to search for old purchase orders, or get reports on a POs  
  - Using the Purchase Order Dashboard  
- Sometimes reach out to the accounting team to get a report on what’s actually been spent for a specific GL code.

## **Data & Analytics**

### **Xuan Mai \- Head of Data & Analytics**

- The mission for the Data & Analytics team is to create and provide better analytics than what Yardi provides out of the box. We’ve done a lot of work to do that.  
- Yardi as a property management system has 8800 tables.  
- If we want to differentiate ourselves from competitors we need better analytics. The path to that while we are using Yardi is quite painful.   
- What Xuan Mai has done is write data pipelines to clean, transform, aggregate, and join and write the resulting datasets to Snowflake, our data warehouse.   
- As a UI frontend to Snowflake we use Sigma, which is the entry point for our data stakeholders and consumers.  
  - Dashboards are viewed every day  
  - Property Health Scorecard is rich in information, manifested in a way that does not appear in Yardi at all.  
- Xuan Mai uses Yardi \-   
- People usually come to the team with a specific ask, or an ambiguous ask.  
  - For example, do we know what the average tenure of resident  
  - In asking questions about the need, they tease out usecases and potential visualizations of the data.  
- Very familiar with the 15 or so core tables in Yardi  
  - When she gets an ask, she’ll initially write some quick Sigma to get a quick intuition into whether or not we can even answer the question and how long the solution might take.  
  - If there are explorations that are easier to do in python, she will start a Jupyter notebook to play around with how she wants to model the data and express it in python in the future.  
    - It’s quite messy to transform a lot of the data.  
    - We are getting to a point where we have an understanding of the data model necessary to produce answers effectively.  
  - After completing the initial exploration, she will go into the Yardi UI and into Yardi Data Model documentation (Voyager 7S Data Dictionary)  
    - Spends a lot of time hunting in this document and hoping for the best. Some tables are well documented, others have no descriptions at all.  
    - Often need to make an educated guess on the meaning of a field. If she has to guess, she will work with the internal Yardi Team, predominantly Llu, to check.  
  - Spent a lot of time understanding pricing data, amenity tags, and unit statuses.   
  - Will often go into the interface and look at different units, comparing what Yardi shows to what she is seeing in the tables after doing initial exploration and engineering.  
- Yardi does not have a master table of all of the Leases.  
  - Tenant table is either a mixed use or misnamed table or the table has evolved over time.  
    - From the tenant table you can surmise what the most recent lease is for a given tenant.  
    - But one of the most common asks from our data stakeholders is a view into historic data.  
      - To serve this ask, because Yardi does not have a true concept of a Lease.  
        - Lease History table is essentially an event table of all the events that may occur on a Lease. One might think that there would be a master table of all the Leases that have ever existed, but there is not. It has to be derived from the Lease History table \-\> events that indicate a unique Lease, for which we create our own unique ID.  
        - The Lease should tell you who, where, when, etc.  
    - Lease table in Snowflake takes all the data in the tenant table, assuming it is the most recent lease for a tenant, and then fill in the historic leases and rents from the lease history table.   
      - The challenge with this is that the Lease History table is accurate from the time that we take over a lease. Therefore when we take over a building that is already occupied, we ingest data from all the current residents, but we might not ingest past resident data, leasing to an incomplete historic view of the building’s performance before we take over.  
- Xuan Mai feels like we have hardly scratched the surface, even if we are doing better from an analytics point of view than other multifamily companies.  
- Only use Voyager, though will sometimes peruse RentCafe Sitemanager to see what is published on the ILSs.   
  - Spends a little time in the reports area.   
  - Occasionally uses the Unit Availability Details report to spot check our data and to understand what our stakeholders are looking at.  
- Because Yardi has so many aspects, there is not one team member to go to about the underlying business rules around all the ways it works. For example, logic around ILS rules.  
  - Specifically, she wants to know when does a unit actually get advertised on an ILS, or how often listings are refreshed to make sure the data we are materializing is timely and accurate and to understand how numbers we see in the tables come to be.  
  - Often the biggest challenge is that we don’t have visibility into how Yardi’s system works. For instance, how they publish to the ILSs.  
- Is Yardi accurate? Do we do testing using Yardi? To what extent?  
  - Yardi is consistent, but not necessarily accurate. There is a big difference between these two things.   
  - Assumptions that you bake into data and information need to be consistent. Because Yardi is the incumbent, it is very consistent, and so people adopt Yardi’s assumptions and believe the data to be accurate.  
- So far the team has largely avoided financial reporting and analytics and so is not using, or planning to use the ledger suite.

## **Engineering**

### **Asa \- Engineering Lead, Website**

- “Yardi is a beast. It has tentacles everywhere.”  
- Within Rentcafe  
  - CRM  
  - CMS/Website  
    - Specify photos to send to ILS for the property  
    - Built our own CMS for the new website  
  - Syndication \- sending our marketing and availability to ILS (1 per day)  
    - Down to the unit level  
  - Marketing Sources  
    - Phone numbers and emails attached to each marketing source that allow us to track to know where leads came from, and who the lead is  
    - Same thing for the website \- when you submit a ‘Contact Us’  
    - Rentcafe provides the analysis of the lead source  
  - Online Leasing  
    - Screening  
    - IDV  
    - Income Verification  
    - Lease Signing (through Bluemoon)  
  - Resident App  
    - Payments  
    - Service Requests  
- Backend  
  - Maintenance IQ  
  - Vendor Shield  
    - Background checks on vendors  
  - Do we use the compliance function  
  - Assurant integrated with Yardi for Renter’s Insurance  
- Asa interacting mostly with Rentcafe CMS/Website, Syndication, and Marketing Sources  
  - Yardi does the syndication \- we set it up with the interface  
- Website  
  - Only leveraging the Rentcafe API, not the Yardi API  
  - Floorplans page  
    - All comes with Rentcafe APIs  
    - Including imagery of the floorplans and apartments they relate to  
  - Contact us page  
  - Scheduler page \- contact us and schedule an appointment  
    - Using the Yardi calendar  
  - Sources API  
    - Need to show the phone number and email that relates to the source the prospect came from (eg. show a particular phone number if the prospect found the flow website from google.)  
      - Refer header in the API request informs the Rentcafe API where the prospect came from.  
      - Need to track the prospect across other pages, storing where they came from  
  - Property API  
    - Office hours  
    - Address  
    - Amenities  
  - Challenges  
    - In Rentcafe there is a description field on the floorplans that doesn’t come back in the API  
      - The workaround is we are not showing a description  
    - When we get the list of floorplans we only get the available floorplans. If a floorplan doesn’t have availability, it doesn’t show up.  
      - There is a configuration in Rentcafe to show floorplans that are not available if we turn on the waitlist functionality.  
        - But if we turn this on the unavailable floorplans also show up in the ILSs through syndication.  
- Yardi has two databases  
  - Yardi database  
    - Dedicated database for every client  
    - We are able to get a backup of the database on a nightly basis  
  - Rentcafe database  
    - A single database for everybody \- multitenant database  
    - Cannot get a backup every day  
    - Can’t even query \- have to access via the API  
- Rentcafe APIs we are using  
  - [https://marketing.rentcafeapi.com/swagger/index.html\#/Reviews/post\_reviews\_getreviews](https://marketing.rentcafeapi.com/swagger/index.html#/Reviews/post_reviews_getreviews)  
  - [https://basic.rentcafeapi.com/swagger/index.html\#/Reviews/post\_reviews\_getreviews](https://basic.rentcafeapi.com/swagger/index.html#/Reviews/post_reviews_getreviews)   
  - ApartmentAvailability  
    - applyOnlineURL  
      - Actual application form to become an applicant  
        - Leads to us having a different user to the user we create in our app  
  - Floorplan  
  - Property  
  - UnitPricingData  
    - Prices based on a lease term  
    - Prices set in Yardi, sent to Rentcafe, but can be overridden in Rentcafe  
  - Appointments (in the Marketing API not the basic API)  
    - To send prospects to the CRM queue  
- Asa: Replacing Yardi is not realistic. But what we should do is replace the CRM.  
  - Complicated part is the syndication  
  - Building the accounting system is extremely complicated

### **Arjuna \- Backend Engineer**

- Yardi is hard to use because modules have been built upon each other without any consistency or refactoring of other modules to align with the new one.   
- Their Soap API is hard to use because we have to parse XML and transform it into something else  
  - This creates a lot of issues  
- APIs we use (all APIs are POSTs, even if they are retrieving information):  
  - GetResidentData  
    - Used to look at resident ledgers to see if they made a payment outside of the FOL App  
    - Able to see the ledger history here for any timeframe  
  - GetUnitInformation  
    - All units in the building  
    - Will be used by the Deepsky backend  
  - GetUserPropertyAccess  
    - List of properties that the Yardi user has access to  
  - GetResidentTransaction\_Login  
    - Gives all unsettled transactions for the user  
    - Can be a charge or a payment  
    - Anything that has not been fully resolved eg. if you have not completed the charge  
      - To show balances  
  - GetResidentTransactions\_Login  
    - All unsettled transactions for all residents in the building  
    - TenantCode in the request is returned as CustomerID in the response  
  - ImportResidentTransactions\_LoginCharge  
    - Creating a charge in Yardi  
    - For example for fees when using a credit card  
  - ImportResidentTransactions\_LoginPayment  
    - Creating a payment in Yardi  
      - Associated with a document number (that we generate as a UUID)  
    - Does not directly relate to a specific charge: we input business rules in Yardi to determine how payments are allocated to outstanding charges on a ledger.  
    - Associated to the ledger by the tcode.  
    - Records the payment on the ledger.  
    - Can also be used for reversals  
      - Identified using the Document Number