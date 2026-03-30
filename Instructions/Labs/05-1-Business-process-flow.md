---
lab:
  title: 'Lab 5.1: Customize a business process flow'
  description: In this task, you will create a new Business Process Flow from the Opportunity Sales Process and then test the new BPF.
  duration: 45 minutes
  level: 100
  islab: true
---

# Module 5: Work with Dynamics 365 Sales Insights and the Sales accelerator 

## Practice Lab 5.1: Customize a business process flow

## Scenario

Contoso Coffee is looking to add a few extra steps to their tried-and-true Sales Business Process. Although sellers have been successful following this framework in the past, they are reporting that a few new suggestions would help nurture leads and land high-value contracts.

Sellers would like to add the following steps to their business process:

-   For high-value potential customers with a budget over \$1,000,000, have the sales lead reach out personally to confirm interest before moving into qualification.
-   In the develop stage, ensure that sellers are tracking existing customer pain points to help identify potential areas for add-on sales that may have been previously missed.

In this lab, we will customize the business process flow to meet our sellers' requests.

This lab will take approximately **45** minutes to complete.

## Exercise 1 – Customize Business Process Flow

### Task 1 – Create Business Process Flow

In this task, you will create a new Business Process Flow from the Opportunity Sales Process and then test the new BPF.

1.  Navigate to `https://make.powerapps.com`
2.  Ensure that you are in the **Sales Trial** environment.
3.  Select **Solutions.**
4.  On the command bar at the top, select **+ New solution**.
5.  In the **Display name** field, enter **Contoso**.
6.  Select **+ New publisher**.
7.  Configure the new publisher as follows.
    1.  **Display Name:** Contoso
    2.  **Name:** Contoso
    3.  **Prefix:** contoso
    4.  **Choice value prefix:** 10000
8.  Select **Save**.
9.  Under Publisher, select the new **Contoso** publisher that you just created.
10. Select **Create**.
11. On the **Command bar** select **Add** existing.
12. From the menu that appears, select **Automation** \> **Process**.
13. In the search box, enter `Sales Process` and select it from the results.
14. Select the **Add** button.
15. Select the **Sales Process** to open it.
16. A new tab opens the BPF editor. Keep the previous tab with the Solutions list open.
17. From the **Components** tab, drag **Condition** and place it between the **Qualify** and **Develop** stages.
    > [!NOTE]
    > This condition checks the customer's budget and identifies 
    > high-value customers with budgets over $1,000,000.
18. Select the **Condition**, go to the **Properties** tab, and enter **Check Budget** for **Display Name**.
19. Under **Rules,** select **Budget Amount** for **Field**.
20. Select **Is Greater than or Equals to** for **Operator**.
21. Select **Value** for **Type**.
22. Enter **1,000,000** for **Value** and select **Apply**.
23. From the **Components** pane, drag a new **Stage** and place it to the right of the **Condition**.
24. Select the **Properties** tab.
25. Enter **Confirm interest** for **Display Name**. Select **Apply.**
26. Click the **Details** button of the **Confirm interest** stage.
27. Select the **Data Step \#1 New Step** inside the **Confirm interest** stage.
28. In the **Properties** tab, open the dropdown for **Data Field.** Select **Confirm interest**. 
    > [!NOTE]
    > The **Step Name** updates automatically.
29. Leave the **Required** checkbox unchecked, then select **Apply**.
30. Next, we will add a new step to ask for customer pain points in the Develop stage, as requested by our sellers. Select the **Develop** stage and expand **Details.**
31. From the Components pane, drag a **Data Step** below Data Step \#4.
32. In the Data Field drop down, select **Customer Pain Points.**
    > [!NOTE]
    > This step appears as a suggested step in the **Develop** stage 
    > to identify customer pain points. This field is not marked as 
    > required.
33. Select **Apply.**
34. Select **Validate** to ensure that the changes you made are valid and that the BPF will work as expected.
35. If there are no issues, select **Update.**
36. Close the tab with the Business process flow editor.
37. Back on your previous tab, select **Done**.
38. In the top menu, select **Publish all customizations.** 
     > [!NOTE]
     > You may need to delete the "opportunity" search in the text box in the upper right to be able to see this button.
39. Wait for your customizations to **publish**.

### Task 2 – Test Business Process Flow

1.  Return to the Sales Hub app.
2.  In the left navigation, select **Opportunities**, then select **+ New** to create a new oppportunity.
3.  In the **Topic** field, enter `Interested in new machines`.
4.  In the **Contact** field, select an existing contact.
5.  Open the **Qualify** stage of the Sales Process business process flow and enter *\$800,000* for Estimated Budget.
    > [!NOTE] 
    >The Business Process Flow includes 4 stages: **Qualify**, **Develop**, **Propose**, and **Close**. The Confirm Interest stage will not be part of the process if the Budget Amount is less than \$1,000,000.
6.  Change the **Estimated budget amount** to *\$1,200,000.*
7.  Confirm that the business process flow now shows five stages: **Qualify**, **Confirm Interest**, **Develop**, **Propose**, and **Close**.
8.  **Save** The Opportunity.
9.  In the **Qualify** stage flyout, select **Next Stage** to advance to the **Confirm Interest** stage.
10.  **Save** The Opportunity.
11. In the **Confirm Interest** stage, for the **Confirmed Interest** field, select **No**, then select **Yes** to confirm.
12. Select the **Next Stage** button to move to the **Develop** stage.
13. Confirm that the Customer Pain Points field appears at the bottom of the Develop stage.
14. Enter *Current machines cannot handle customer volume* in the Customer Pain Points field.
15. Select **Next stage**.
16. Select **Save** to save the record.

