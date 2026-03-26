---
lab:
  title: 'Lab 1.1: Configure supporting applications'
  description: In this lab, we will turn on and configure the features that will help our CRM organization meet these sellers' requirements.
  duration: 30 minutes
  level: 100
  islab: true
---

# Module 1: Configure Dynamics 365 Sales

## Practice Lab 1.1: Configure supporting applications

## Scenario

Contoso Coffee sellers report that although Dynamics 365 Sales is very helpful in increasing seller productivity, the application feels very siloed in relation to their daily flow of work. They have the following requirements for their IT department:

-   Sellers would like to track and manage sales-related email correspondence in CRM.
-   Sellers would like to store documents related to sales (like product knowledge articles, customer research, and market trend reports) in CRM. They want to be able to access, share, and manage these documents directly from the Sales app.
-   Sellers would like to collaborate with other departments like inventory, order fulfillment, and marketing as they pursue their sales opportunities. They would like these other departments to be able to collaborate on a customer record within a Teams chat or channel.
-   Sellers have heard a lot about the Copilot features within Dynamics 365 Sales, including record summarization, catching up on changes to records, preparing for meetings, and composing correspondence. They want to ensure that Copilot features are turned on in their environment so they can start leveraging AI within the app to enhance their productivity.

In this lab, we will turn on and configure the features that will help our CRM organization meet these sellers' requirements.

This lab will take approximately **30** minutes to complete.

## Exercise 1: Configure email, SharePoint, and OneDrive integration

### Task 1: Configure Email Integration

1.  In a web browser, navigate to `https://admin.powerplatform.microsoft.com/`
2.  In the left navigation, select **Manage**, then select **Environments**.
3.  Select the **Sales Trial** environment to open it.
4.  Locate and select **Settings** from the commands listed at the top.
5.  Select the email heading to expand it and select **Mailboxes**.
6.  Open the Mailbox record for **MOD Administrator**.
7.  Configure the **MOD Administrator Mailbox** as follows:
    -   **Server Profile**: Microsoft Exchange Online
    -   **Incoming Email**: Server-Side Synchronization 
    -   **Outgoing Email**: Server-Side Synchronization 
    -   **Appointments, Contacts, and Tasks**: Server-Side Synchronization
8. Select **Save**, then select **Approve Email**.

   > **Note:** You must approve the mailbox before you can send and receive email.
9.  You will be asked if you want to approve the primary email. Select **OK**.
10. Click **Test & Enable Mailbox**.
11. On the test and enable pop-up screen, make sure that if this mailbox was previously configured to sync with another organization, checking this option will switch it to sync with this organization.
12. Select **OK**.

**IMPORTANT:** Do not navigate away from this page while the tests complete. If you would like to work on Task 2 while the tests complete, you can open a new tab or browser.

## Task 2: Enable Server-Based SharePoint Integration

In this task, you will enable server-based SharePoint integration for your Dynamics 365 organization.

1.  In a web browser, navigate to `https://admin.powerplatform.microsoft.com/`
2.  In the left navigation, select **Environments**.
3.  Open the **Sales Trial** environment.
4.  In the top command bar, select **Settings**.
5.  Under **Integration**, open **Document management settings**.
6.  If the **Configure server-based SharePoint integration** option is 
   available, select it and continue to the next step. If the option is 
   not visible, SharePoint integration is already enabled — skip to 
   step 13.
7.  On the **Configure Server-based SharePoint integration** page, select **Next**.
8.  Select **Online** as the site location, then select **Next**.
9.  Enter the URL of your SharePoint site (Example: https://m365x<XXXXXXXX>.sharepoint.com), then select **Next**.
    > [!NOTE]
    > To find your SharePoint URL, select the **App Launcher** icon (Looks like a 3 x 3 square) in the upper-left corner of the screen, hold **Ctrl** and then select **SharePoint**.

10. After the site is validated, select **Next**.
11. Select **Next**.
12. Review the summary and select **Done**.
13. Select **Document management settings**.
14. Select any entities that you want document management to be enabled for, such as **Lead**, **Account**, **Opportunity**, then select **Next**.
    
    > [!IMPORTANT]
    > If you plan to configure email engagement in Sales insights, ensure you also select the **Email** Entity.
15. In the SharePoint site URL field, enter the URL of the SharePoint site you used in step 9 and validate the URL.
16. Select **Next**.
17. Select **Next**.
18. Review the **Document library creation status**, then select **Finish**.
19. Select **Close**.

### Task 3: Setup OneDrive for Business Integration

In this task, you will set up OneDrie integration for your Dynamics CRM organization. (As of the publication of this course, Document Management settings were not available from within the Power Platform Admin center. You will need to configure OneDrive for business integration from the classic Dynamics 365 Settings area.)

1.  In a web browser, navigate to `https://admin.powerplatform.microsoft.com/`
2.  From the site navigation on the left side of the screen, select **Environments**.
3.  Open the **Sales Trial** environment that you have been working in to open it.
4.  Locate and select **Settings** from the commands listed at the top.
5.  Under the Integration heading, select **Document management settings**.
6.  Click on the **Enable OneDrive for Business** icon.
7.  Select the **Enable OneDrive for Business** checkbox and click **OK**.
8.  After the screen refreshes, click the **OneDrive for Business Folder Settings**.
9.  Accept the default folder name, or enter a name of your choice, and click **OK**.

## Exercise 2: Configure Teams and Copilot

### Task 1: Configure Teams Integration

1.  If necessary, open the Sales Hub app.
2.  Using the navigation on the left, select the **Sales** area (Bottom Left).
3.  From the menu that appears, select **App Settings**.
4.  Under the General Settings group, select **Chat and Collaboration**.
5.  Set **Turn on the linking of Dynamics 365 records to Microsoft Teams channels** to **Yes**.
6.  Set **Turn on Enhanced Microsoft Teams Integration** to **Yes**. (You may need to select your MOD Administrator account. If asked for permissions, select **Accept**.)
7.  Under **Turn on Microsoft Teams chats inside Dynamics 365**, select **Turn on for all Dynamics 365 Apps**.
8.  Select the **Save** button.  
    **IMPORTANT**: It can take several minutes for the changes to be saved.

### Task 2: Configure Copilot

1.  Make sure that you are in the **App Settings** area.
2.  Under the General Settings group, select **Copilot**.
3.  Select the checkbox next to **Try our newest preview features before they’re rolled out to everyone** to enable it.
4.  Under **Copilot features**, change the **All Dynamics 365 Sales Apps** as follows:
    -   **Chat**: On
    -   **Email (Preview)**: On
5.  Select the **Save** button.

