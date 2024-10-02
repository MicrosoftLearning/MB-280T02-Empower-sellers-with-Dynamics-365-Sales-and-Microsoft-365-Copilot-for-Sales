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

8.  A new tab will open the BPF editor. (Keep the old tab with the Solution open.) We will now make some edits to the BPF that we have been seeing on the Lead form throughout the course.

14. Drag **Condition** from the **Components** tab and place it between the
    **Qualify** and **Develop** stages.

15. Select the **Condition**, go to the **Properties** tab, and enter **Check
    Budget** for **Display Name**.

16. Under **Rules,** select **Budget Amount** for **Field**.

17. Select **Is Greater than or Equals to** for **Operator**.

18. Select **Value** for **Type**.

19. Enter **1,000,000** for **Value** and click **Apply**.

20. Now we need to add a new stage to complete the condition. From the Components pane, add a new Stage to the right of the Condition.

24. Select the **Properties** tab.

25. Enter **Confirm interest** for **Display Name**. Select **Apply.**

26. Click the **Details** button of the **Confirm interest** stage.

27. Select the **New Step** inside the **Confirm interest** stage.

28. In the **Properties** tab, open the dropdown for **Data Field.** Select **Confirm interest**. The Step Name will update automatically.

29. Check the **Required** check box and click **Apply**.

30. Next, we will add a new step to a stage. Select the **Develop** stage and expand **Details.**

31. From the Components pane, drag a **Data Step** below Data Step #4.

32. In the Data Field drop down, select **Customer Pain Points.** It will now be a suggested step in the Develop stage to identify the customer pain points. We will not mark this field as required.

33. Select **Apply.**

34. Click **Validate** to ensure that the changes you made are valid.

35. Click **Update.**

37. Close the Business process flow editor.

38. Click **Done** in the pop-up in the Default Solution area. In the top menu, select **Publish all customizations.** (You may need to delete the "opportunity" search in the text box in the upper right to be able to see this button.)

39. Wait for your customizations to publish.

### Task 2 – Test Business Process Flow

1.  Return to the Sales Hub app.

2. Navigate to the **Leads** section and click **+New** to create a new lead. You can enter any information you like in the Contact section of the form.

4. Open the **Qualify** stage of the Lead to Opportunity Sales Process business process flow. the Enter $800,000 for Budget Amount.

12. The Business Process Flow should have 4 stages, **Qualify**, **Develop**,
    **Propose**, and **Close**. The Confirm Interest stage will not be part of the
    process if the Budget Amount is less than $1,000,000.

13. Change the **Budget Amount** to 1,200,000.

14. The Business Process Flow should have 5 stages, **Qualify**, **Confirm Interest**, **Develop**, **Propose**, and **Close**. Move from the Qualify stage to the next stage.

17. The process should move to the **Confirm Interest** stage. Confirm interest by selecting **Yes.**

18. **Save** and **Qualify** your Lead record.

20. You will be taken to a new Opportunity record created from your Lead record, and the business process flow should now move to the **Develop** stage.

21. **Save** the record. Any new Lead and Opportunity records will now use your new version of the business process flow.

22. Confirm that the Customer Pain Points field appears at the bottom of the Develop stage.

23. Enter *Current machines cannot handle customer volume* in the Customer Pain Points field.

24. Select **Next stage**.

25. **Save** the record. Any new or existing Lead and Opportunity records will now use your new version of the Lead to Opportunity Business Process.
