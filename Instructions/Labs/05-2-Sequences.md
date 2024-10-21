---
lab:
    title: 'Lab 5.2: Build a sequence'
---

# Module 5: Work with Dynamics 365 Sales Insights and the Sales accelerator 

## Practice Lab 5.2: Build a sequence

### Scenario
Contoso Coffee’s sellers suggest that sales could be improved if organizational "best practices" were easier to follow. After examination, Contoso’s sales managers have determined an ideal sequence of sales events for sellers. They want to enforce best practices by setting up a series of consecutive activities for sellers to follow while qualifying leads. You want to ensure that it is as easy as possible for sellers to follow during their day. You have determined that a sequence is the best way to accomplish this.

Upon successful completion of this lab, you will be able to:

-   Create a segment
-   Create a sequence
-   Define sequence activities
-   Activate and connect sequences to records

## Exercise 1: Create and attach Sequences to records

### Task 1: Enable Sales Accelerator

1.  In the Sales Insights group, select **Global settings.**
2.  In the Sales accelerator sub-group, select the **Sequences** tab.
3.  You will be asked to set up the Workspace to be able to use Sequences. Select the **Setup workspace** button.
4.  Select the **Quick setup** button.
5.  In the Record type and form section, select **+ Add record type**. Select **Opportunities.**
6.  For the default form for each record type, configure as follows:
    -   Leads: Sales Insights
    -   Opportunities: Sales Insights
7.  Select the **Publish** button.
    -   Note: It can take several minutes for your changes to be applied.

### Task 2: Create a Segment

1.  If you have not done so already, change the area to **Sales Insights settings.**
2.  In the Sales Insights group, select **Global settings.**
3.  In the Sales accelerator sub-group, select the **Work Assignment** tab.
4.  Make sure the **Record type** is set to **Leads** and select the **New Segment** button.
5.  In the **Name** field enter the text **Trade Show Leads** and then select the **Next** button.
6.  On the **Segment definition** tab, select the **Add** button.
7.  From the menu that appears, select **Add** row.
8.  Configure the condition as follows:
    1.  **Lead Source** – **Equals** – **Trade Show**
9.  Select **Simulate Results**.

    You should see a segment member simulation screen which will include any leads that meet your criteria.

10. Close the **Segment member simulation** window.
11. Select the **Save** button.
12. Select the **Activate** button.

## Exercise 2: Create and attach Sequences to records

### Task 1: Create new sequence

1.  If you have not done so already, change the area to **Sales Insights settings.**
2.  In the Sales Insights group, select **Global settings.**
3.  In the Sales accelerator sub-group, select the **Sequences** tab.
4.  If necessary, select **Enable** on the notification to enable workflow for sequences to work properly.
5.  On the Sequences tab, select **+ New sequence.**
6.  You have the option to create a sequence from a number of common templates. You can explore the templates available. When you're ready, select **Start from blank.**
7.  Next, you will assign a name, description, and choose the type of table that the sequence will be available for. In the Sequence Name text box, type the sequence name, *Trade Show Follow-up Sequence.*
8.  In the Description text box, enter sequence description: "This is a test sequence for Test Coffee. This sequence will be used for following up with potential customers after trade shows."
9.  In Record type, select **Lead** (if it is not already selected).
10. Click **Next.**

### Task 2: Choose the first activity for seller to take

Choose the first step for your sellers to take. This can be either sending an email, making a phone call or add a task of your own. In our example, we will start with an email.

1.  Underneath the Sequence start tile, select the **+** button to add an action or other element.
2.  Click on **Send an email.**
3.  For Title, enter: *Introduction email.*
4.  For Description, optionally enter a description: *Introduce lead to the sales team.*
5.  If email templates (table specific or global templates) are available in your organization, you can choose an email template. In this case, we will assume that the seller will write their own introduction email.
6.  Select the **X** to close out of the Activity pane.
7.  On the Command Bar for the sequence, select **Save.**

### Task 3: Add additional activities for your seller to take

Add additional activities for your sellers to take in an ordered manner - for example, the seller needs to take the first activity first, then the second and third and so on.

1.  Click on the **+** button.
2.  Choose the next activity for the seller to take, can be either sending an email, making a phone call or add a task of your own. Select **Set wait time** to define a time-interval between activities. In our example we will add a time-interval of 1 hour.
3.  Click Save.
4.  Click on the **+** button.
5.  Select **Phone call.**
6.  In the Title, enter *Follow-up call.* (You can choose to add a description if you would like.)
7.  Select **Save** on the command bar.

### Task 4: Activate the sequence

To make the sequence available for sellers to use, activate the sequence.

1.  Select **Activate** on the command bar.
2.  Select **I understand**, and then **Activate** in the pop-up.
3.  Your sequence will now have a green bar at the top telling you that the sequence was successfully activated.

### Task 5: Connect the sequence to a segment

1.  Make sure you are in the **Sales Insights settings** area.
2.  Using the navigation on the left, select **Sequences**.
3.  Open the **Trade Show follow-up** sequence you created earlier.
4.  Select the **Connected leads** tab.
5.  Select **+ Connect Segments**
6.  Locate and select the **Trade Show Leads** segment you created earlier.
7.  Select **Connect**.

### Task 6: Connect the sequence to record (From Record)

1.  Change the area to the **Sales** area using the bottom left dropdown menu.
2.  Select **Leads** from the site navigation menu.
3.  Select one of the leads you created earlier.
4.  On the command bar, select the **down arrow** next to Sequences. From the menu that appears, select **Connect sequence** from the command bar.
5.  Select the sequence you created earlier and select **Connect.**
6.  A confirmation message appears at the bottom of the page, and the sequence is connected to the selected lead record.
7.  If you are prompted to assign a seller, select the **Assign** button. Now, the seller(s) who have access to the lead record can see the activities connected with it.
8.  Refresh the page - you should see the tasks you created in the **Up next** section.

