
## Exercise 1: Configure email, SharePoint, and OneDrive integration
### Task 1: Configure Email Integration
1. In a web browser, navigate to *An external link was removed to protect your privacy.*.
2. From the site navigation on the left side of the screen, select **Environments**.
3. Select the **Sales Trial** environment to open it.
4. Locate and select **Settings** from the commands listed at the top.
5. Select the email heading to expand it and select **Mailboxes**.
6. Open the Mailbox record for **MOD Administrator**.
7. Verify that **MOD Administrator Mailbox** is set as follows:
   - **Server Profile**: Microsoft Exchange Online
   - **Incoming Email**: Server-Side Synchronization or Email Router
   - **Outgoing Email**: Server-Side Synchronization or Email Router
   - **Appointments, Contacts, and Tasks**: Server-Side Synchronization
8. Click **Approve Email**. (Note: You must approve the mailbox before you can send and receive email)
9. You will be asked if you want to approve the primary email, select **OK**.
10. Click **Test & Enable Mailbox**.
11. On the test and enable pop-up screen, make sure that if this mailbox was previously configured to sync with another organization, checking this option will switch it to sync with this organization.
12. Select **OK** (Wait for all the tests to complete before moving to the next step). This can run in the background as you move on to more tasks.

### Task 2: Enable Server-Based SharePoint Integration
In this task, you will enable server-based SharePoint integration for your Dynamics 365 organization.
1. In a web browser, navigate to *An external link was removed to protect your privacy.*.
2. From the site navigation on the left side of the screen, select **Environments**.
3. Open the **Sales Trial** environment that you have been working in to open it.
4. Locate and select **Settings** from the commands listed at the top.
5. Under the Integration heading, select **Document management settings**.
6. You should see an option to **Enable Server-Based SharePoint Integration**. (If it is not there, SharePoint integration has already been enabled and you can skip to step eleven.)
   - If SharePoint Integration is not configured, select **Enable Server-Based SharePoint Integration**.
7. In the enable Server-Based SharePoint Integration screen, click the **Next** button.
8. Select **Online** for the deployment type, click the **Next** button.
9. Enter the URL of the SharePoint site you want to use. (Example: `https://”Orgname”.sharepoint.com`), click the **Next** button. (Hint: You will be able to find the org name in your current browser tab. It will be before `.crm.dynamics.com`.)
10. After the site has been validated, click the **Finish** button.
11. Click **Document Management Settings**.
12. Select any entities that you want document management to be enabled for, such as Leads, Accounts, Opportunities, and click **Next**.
    - **IMPORTANT**: If you are planning on configuring email engagement in Sales insights, select the Email Entity.
13. In the SharePoint site URL field, enter the URL of the SharePoint site you used in the previous task.
14. Click the **Next** button.
15. Click the **Finish** button to complete the setup.

### Task 3: Setup OneDrive for Business Integration
In this task, you will set up OneNote integration for your Dynamics CRM organization. (As of the publication of this course, Document Management settings were not available from within the Power Platform Admin center. You will need to configure OneDrive for business integration from the classic Dynamics 365 Settings area.)
1. If necessary, navigate to **Settings** > **Document Management**.
2. Click on the **Enable OneDrive for Business** icon.
3. Select the **Enable OneDrive for Business** checkbox and click **OK**.
4. After the screen refreshes, click the **OneDrive for Business Folder Settings**.
5. Accept the default folder name, or enter a name of your choice, and click **OK**.

## Exercise 2: Configure Teams and Copilot 
### Task 1: Configure Teams Integration
1. If necessary, open the Sales Hub app.
2. Using the navigation on the left, select the **Sales** area (Bottom Left).
3. From the menu that appears, select **App Settings**.
4. Under the General Settings group, select **Chat and Collaboration**.
5. Set **Turn on the linking of Dynamics 365 records to Microsoft Teams channels** to **Yes**.
6. Set **Turn on Enhanced Microsoft Teams Integration** to **Yes**. (You may need to select your MOD Administrator account. If asked for permissions, select **Accept**.)
7. Under **Turn on Microsoft Teams chats inside Dynamics 365**, select **Turn on for all Dynamics 365 Apps**.
8. Select the **Save** button.  
   **IMPORTANT**: It can take several minutes for the changes to be saved.

### Task 2: Configure Copilot
1. Make sure that you are in the **App Settings** area.
2. Under the General Settings group, select **Copilot**.
3. Select the checkbox next to **Try our newest preview features before they’re rolled out to everyone** to enable it.
4. Under **Copilot features**, change the **All Dynamics 365 Sales Apps** as follows:
   - **Chat**: On
   - **Email (Preview)**: On
5. Select the **Save** button.
