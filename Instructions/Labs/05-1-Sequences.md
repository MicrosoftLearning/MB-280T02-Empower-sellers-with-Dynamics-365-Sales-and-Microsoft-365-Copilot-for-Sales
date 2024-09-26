---
lab:
    title: 'Lab 5.1: Build a sequence'
---

# Module 5: Work with Dynamics 365 Sales Insights and the Sales accelerator 

## Practice Lab 5.1: Build a sequence

### Scenario
Contoso Coffee’s sellers suggest that sales could be improved if organizational "best practices" were easier to follow. After examination, Contoso’s sales managers have determined an ideal sequence of sales events for sellers. They want to enforce best practices by setting up a series of consecutive activities for sellers to follow while qualifying leads. You want to ensure that it is as easy as possible for sellers to follow during their day. You have determined that a sequence is the best way to accomplish this.

Upon successful completion of this lab, you will be able to:
- Create a sequence
- Define sequence activities
- Activate and connect sequences to records

### Task 1: Enable Sales Accelerator
1. Change the area to Sales Insights settings using the bottom left ˅ drop-down menu icon.
2. In the Sales Insights group, select Global settings.
3. In the Sales accelerator sub-group, select the Sequences tab.
4. You will be asked to set up Workspace to be able to use Sequences. Select the Setup workspace button.
5. Select the Quick setup button.
6. In the Record type and form section, select + Add record type. Select Opportunities.
7. For the default form for each record type, configure as follows:
   - Leads: Sales Insights
   - Opportunities: Sales Insights
8. Select the Publish button.
   - Note: It can take several minutes for your changes to be applied.

### Task 2: Create new sequence
1. If you have not done so already, change the area to Sales Insights settings using the bottom left ˅ drop-down menu icon.
2. In the Sales Insights group, select Global settings.
3. In the Sales accelerator sub-group, select the Sequences tab.
4. If necessary, select Enable on the notification to enable workflow for sequences to work properly.
5. On the Sequences tab, select + New sequence.
6. You have the option to create a sequence from a number of common templates. You can explore the templates available. When you're ready, select Start from blank.

### Task 3: Create basic information about the sequence
Next, you will assign a name, description, and choose the type of table that the sequence will be available for.
1. In the Sequence Name text box, type the sequence name, Sequence.
2. In the Description text box, enter sequence description: "This is a test sequence for Test Coffee."
3. In Record type, select Lead (if it is not already selected).
4. Click Next.

### Task 4: Choose the first activity for seller to take
Choose the first step for your sellers to take. This can be either sending an email, making a phone call or add a task of your own. In our example, we will start with an email.
1. Underneath the Sequence start tile, select the + button to add an action or other element.
2. Click on Send an email.
3. For Title, enter: Introduction email.
4. For Description optionally, enter a description: Introduce lead to the sales team.
5. If email templates, table specific or global templates, are available in your organization, you can choose an email template. In this case, we will assume that the seller will write their own introduction email.
6. Select the X to close out of the Activity pane.
7. On the Command Bar for the sequence, select the Save.

### Task 5: Add additional activities for your seller to take
Add additional activities for your sellers to take in an ordered manner, i.e. seller needs to take the first activity first, then the second and third and so on. To persist changes, after adding an activity, click on the Save button.
1. Click on the + button.
2. Choose the next activity for the seller to take, can be either sending an email, making a phone call or add a task of your own. Select Set wait time to define a time-interval between activities. In our example we will add a time-interval of 1 hour.
3. Click Save.
4. Click on the + button.
5. Select Phone call.
6. In the Title, enter Follow-up call. (You can choose to add a description if you would like)
7. Select Save on the command bar.

### Task 6: Activate the sequence
To make the sequence available for sellers to use, activate the sequence.
1. Select Activate on the command bar.
2. Select I understand, and then Activate in the pop-up.
3. Your sequence will now have a green bar at the top telling you that the sequence was successfully activated.

### Task 7: Connect the sequence to records
1. Change the area using the bottom left dropdown menu, select the Sales area.
2. Select Leads from the site navigation menu.
3. Open the Another Coffee Machine Lead you created earlier in the course. If you do not have that lead, you can select one randomly.
4. On the command bar, select the down arrow next to Sequences. From the menu that appears, select Connect sequence from the command bar. The list of available sequences includes sequences created by you and other users for the Lead table.
5. Select the Lead Sequence you created earlier and select Connect.
6. A confirmation message appears at the bottom of the page, and the sequence is connected to the selected lead record.
7. If you are prompted to assign to a seller, select the Assign button. Now, the seller(s) who have access to the lead record can see the activities connected with it.
```

Feel free to copy and paste this markdown content wherever you need it! If you have any other requests or need further assistance, just let me know.
