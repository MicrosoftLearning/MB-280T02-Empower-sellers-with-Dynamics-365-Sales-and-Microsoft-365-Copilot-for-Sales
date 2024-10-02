---
lab:
    title: 'Lab 7.1: Customize a business process flow'
---

# Module 7: Enhance seller productivity by extending Dynamics 365 Sales

## Practice Lab 7.1: Customize a business process flow

## Scenario

Contoso Coffee is looking to formalize their sales process to
increase revenue and the give leadership stronger forecasting abilities. In this lab, you will create a business process flow to guide the
sales process experience for users.

## Exercise 1 – Customize Business Process Flow
### Task 1 – Create Business Process Flow

In this task, you will create a new Business Process Flow from the Opportunity
Sales Process and then test the new BPF.

1.  Navigate to <https://make.powerapps.com>.

2.  Ensure that you are in the **Sales Trial** environment. 

3.  Select **Solutions** and click on the **Default Solution**.

4.  Locate the **Search** box in the top left corner of the page. Search for *Processes* and select it.

6.  Now, we will find the **Lead to Opportunity Sales Process** in the list of processes. (You can now use the search box in the upper right corner to search.) When you find it, select it.

8.  A new tab will open the BPF editor. (Keep the old tab with the Solution open.) In the menu above the business process flow, click **Deactivate**.

9.  Confirm deactivation.

10. Click **Save As**. Return to the other tab with the Processes view. (If you have a pop-up saying you are currently editing a Process, click **Done.**)

11. In the list of Processes, you will now have a new process will be named **Opportunity Sales Process (Copy)**. Select the name of the process to open the editor.

12. Expand the dropdown next to the name of the process. Change the Process Name to *Opportunity Sales Process V2*.

13. Click **Save**.

14. Drag **Condition** from the **Components** tab and place it between the
    **Qualify** and **Develop** stages.

15. Select the **Condition**, go to the **Properties** tab, and enter **Check
    Budget** for **Display Name**.

16. Under **Rules,** select **Budget Amount** for **Field**.

17. Select **Is Greater than or Equals to** for **Operator**.

18. Select **Value** for **Type**.

19. Enter **1,000,000** for **Value** and click **Apply**.

20. Click **Save**.

21. A new stage has now been added between the Check Budget condition and the Develop stage. Select the new stage.

22. Select the **Properties** tab.

23. Enter **Confirm interest** for **Display Name**. Select **Apply.**

24. Click the **Details** button of the **Confirm interest** stage.

25. Select the **New Step** inside the **Confirm interest** stage.

26. In the **Properties** tab, open the dropdown for **Data Field.** Select **Confirm interest**. The Step Name will update automatically.

27. Check the **Required** check box and click **Apply**.

28. Click **Save**.

29. Click **Activate**.

30. Confirm the activation.

31. Close the Business process Flow editor.

33. Click **Done**.

### Task 2 – Add Business Process Flow

In this task, you will remove the old business process flow from your Sales Hub
application and add the V2 business process flow.

3.  Select **Apps**.

4.  Select the **Sales Trial** application and click **Edit**.

5.  The application designer will open. Select **Automation.**

6.  Select the **Opportunity Sales Process V2** business process flow from the pane on the left. 

7.  Select **Save**.

8.  Select **Publish**.

9.  Select **Back.**

### Task 3 – Test Business Process Flow

1.  Select **Play** next to the Sales Trial app. The Sales Trial app will launch.

2. Select **Leads** and create a new lead (you can use any name or information you would like). Enter $800,000 for Budget Amount.

12. The Business Process Flow should have 4 stages, **Qualify**, **Develop**,
    **Propose**, and **Close**. The Confirm Interest stage will not be part of the
    process if the Budget Amount is less than $1,000,000.

13. Change the **Budget Amount** to 1,200,000.

14. The Business Process Flow should have 5 stages, **Qualify**, **Confirm Interest**, **Develop**, **Propose**, and **Close**.

15. Click on the **Qualify** Stage.

16. Click **Next Stage**.

17. The process should move to the **Confirm Interest** stage. Click **Next Stage**.

18. The process should not move to the next stage until the **Confirm Interest**
    step is marked complete.

19. Check the **Mark Complete** checkbox and click **Next Stage**.

20. The process should now move to the **Develop** stage.
