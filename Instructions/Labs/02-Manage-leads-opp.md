---
lab:
  title: 'Lab 2.1: Manage leads and opportunities'
  description: In this task, you will create three leads, one without company information and two with company information.
  duration: 30 minutes
  level: 200
  islab: true
---

# Module 2: Manage leads and opportunities with Dynamics 365 Sales

## Practice Lab 2.1 – Manage leads and opportunities

### Scenario
Contoso Coffee is looking to use Dynamics 365 Sales to formalize their sales process as well as address a backlog of untouched leads imported by the marketing team from trade shows and campaigns. As a sales analyst at Contoso Coffee, you have been asked to assess and update lead records to ensure that the executive team is working from an accurate pipeline report in the upcoming leadership meeting.

Upon successful completion of this lab, you will be able to:
- Create and update lead records
- Qualify and disqualify leads
- Reactivate lead records

This lab will take approximately **30** minutes to complete.

### Exercise 1 – Manage customers

#### Task 1 – Creating Leads
In this task, you will create three leads, one without company information and two with company information.
1. Go to your Dynamics 365 Sales Hub application. Ensure you are in the Sales area, using the bottom left dropdown menu.
2. In the left navigation, under **Sales**, select **Leads**.
3. On the command bar, select **Read Only Grid** to change the type of view.
4. On the command bar, select **+ New**.
5. Enter the following values:
   - **Topic:** *Coffee Machine Lead Without Company*
   - **First Name:** *Jane*
   - **Last Name:** *Doe*
6. In the **Job Title** field, enter `Cafeteria Manager`. If a suggestion appears, you can accept it instead.
7. Select **Save**, then on the command bar, select **+ New**.
8. Enter the following values:
   - **Topic:** *Coffee Machine Lead with Company*
   - **First Name:** *Jon*
   - **Last Name:** *Doe*
   - **Company:** *Doe Inc.*
9. Select **Save**, then on the command bar, select **+ New**.
10. Enter the following values:
    - **Topic:** *Another Coffee Machine Lead*
    - **First Name:** *Jack*
    - **Last Name:** *Rogers*
    - **Company:** *Test Coffee Shop, Inc.*

11. Select **Save**.
### Exercise 2 – Lead Qualifications
In this exercise, you will qualify/disqualify leads and see what records will be created when a lead goes through the qualification process.

#### Task 1 – Qualify Coffee Machine Lead Without Company Information
1. Go to your Sales Hub application.
2. In the left navigation, under **Sales**, select **Leads**.
3. On the command bar, select **Read Only Grid** to change the type of view.
4. Locate and select **Coffee Machine Lead Without Company**.
5. On the command bar, select **Qualify** to convert the lead into a new opportunity record.
    > [!NOTE] 
    > If the new opportunity does not open automatically, select **Opportunities** in the left navigation to view all open opportunities, then open the **Coffee Machine Lead without Company** opportunity.
6. In the **Contact** field, notice that **Jane Doe** is now a Contact 
   record in the application.
7. In the header of the opportunity record, locate the **Account** 
   field and notice that it is empty.
9. Select **Save.**

#### Task 2 – Qualify Coffee Machine Lead with Company
1. Go to your Sales Hub application.
2. In the left navigation, under **Sales**, select **Leads**.
3. Locate and open **Coffee Machine Lead with Company** record.
4. On the command bar, select **Qualify** to convert the lead into a 
   new opportunity record.
   > [!NOTE]
   > You are automatically taken to the newly created opportunity record. If the opportunity does not open automatically, select **Opportunities** in the left navigation, then open the **Coffee Machine Lead with Company** opportunity.
5. In the **Contact** field, notice that **Jon Doe** is now a Contact record in the application.
6. In the header of the opportunity record, locate the **Account** field and notice that **Doe Inc.** is now an Account record.

#### Task 3 – Disqualify a Lead
1. If necessary, go to your Sales Hub application.
2. In the left navigation, under **Sales**, select **Leads**.
3. Locate and open **Another Coffee Machine Lead** record.
4. On the command bar, select the vertical ellipsis (**⋮**), then 
   select **Disqualify**.
5. From the menu that appears, select **No Longer Interested.**
> [!NOTE]
> Notice that the lead is disqualified, the status changes to **No Longer Interested**, and the record becomes read-only.


#### Task 4 – Reactivate A Lead
1. If necessary, go to your Sales Hub application.
2. In the left navigation, under **Sales**, select **Leads**.
3. Select the view selector next to **My Open Leads** and change the 
   view to **Closed Leads**.
   > [!NOTE]
   > The lead you disqualified is no longer visible in the **My Open Leads** view.
4. Locate and open the **Another Coffee Machine Lead** record.
5. On the command bar, select **Reactivate Lead**.
   > [!NOTE]
   > The lead is reactivated, the status changes back to **New**, and the record becomes editable.

### Exercise 3 – Work with Opportunities
In this exercise, you will walk through the process of working an opportunity through the sales process.

#### Task 1 – Manage the Coffee Machine Lead with Company
1. If necessary, go to your Sales Hub application.
2. In the left navigation, under **Sales**, select **Opportunities**.
3. Locate and open the **Coffee Machine Lead with Company** opportunity.
4. In the **Opportunity information** section, enter the following values:
   - **Budget Amount:** *$17,000*
   - **Purchase Timeframe:** *This Quarter*
   - **Purchase Process:** *Committee*
   - **Description:** *Looking to upgrade their current coffee machines at multiple*
5. Expand the record header and enter the following values:
   - **Est. Close Date:** Enter tomorrow's date.
   - **Est. Revenue:** *$16,500*
6. On the **Timeline** control, select **+** to add a timeline record.
7. From the menu that appears, select **Phone call.**
8. Enter the following values:
   - **Subject:** *Initial Call to Jon*
   - **Due:** Select today's date at 4:30 PM
9. Select **Save and Close**.
10. On the **Lead to Opportunity** business process flow, select the 
    **Develop** stage and enter the following values:
   - Customer Need: *Looking to upgrade their coffee machines at multiple locations.*
   - Proposed Solution: *Recommending multiple AirPot Duo Machines.*
   - Identify Stakeholders: Completed
   - Identify Competitors: Completed
11. Select **Next Stage**.
12. On the **Propose** stage, set all the fields to **Completed.**
13. Select **Next Stage**.
14. Select anywhere outside of the business process stage to close it.
15. In the **Timeline** section, locate the **Initial Call to Jon** phone call activity and select the **Open record** icon to open it.
16. On the command bar, select **Mark Complete**.
17. On the **Lead to Opportunity** business process flow, select the **Close** stage.
18. Mark all the items in the Close stage as **Completed.**
19. Select **Finish**.
20. On the Command bar at the top, select **Close as won**.
21. On the **Close opportunity** dialog, select the **OK**.

Congratulations, you have successfully created and managed Leads and Opportunities in Dynamics 365 Sales.
