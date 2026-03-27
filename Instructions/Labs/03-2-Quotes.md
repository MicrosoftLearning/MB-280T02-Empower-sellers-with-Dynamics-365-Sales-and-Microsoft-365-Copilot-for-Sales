---
lab:
  title: 'Lab 3.2: Build quotes'
  description: As a sales analyst for the Dynamics 365 Sales implementation at Contoso Coffee, you want to ensure that salespeople will be able to leverage the product catalog enhancements throughout the entire sales lifecycle. To ensure the functionality is working correctly, you will test the process of building a quote from a new opportunity.
  duration: 15 minutes
  level: 100
  islab: true
  primarytopics:
    - Dynamics 365
---

# Module 3: Manage orders and product catalog with Dynamics 365

## Practice Lab 3.2 – Build quotes

### Scenario
As a sales analyst for the Dynamics 365 Sales implementation at Contoso Coffee, you want to ensure that salespeople will be able to leverage the product catalog enhancements throughout the entire sales lifecycle. To ensure the functionality is working correctly, you will test the process of building a quote from a new opportunity.

Upon successful completion of this lab, you will be able to:
- Create opportunities and add opportunity line items
- Generate a quote from an opportunity

This lab will take approximately **15** minutes to complete.

### Exercise 1 – Create a Quote

#### Task 1 – Add Products Line Items
In this task, you will create an Opportunity and add Products Line Items.
1. Go to your Dynamics 365 Sales Hub application.
2. In the left navigation, under **Sales** group, select **Opportunities**.
3. Select **+ New.**
4. Enter and select the following values:
   - **Topic:** `Interested in Airpot XL Accessories`
   - **Contact:** Jon Doe
5. In the record header, select the **down arrow** next to the **Owner** field and select **Test Coffee Shop, Inc.** for **Account**, then select **Save**.
  > [!NOTE]
  > If **Test Coffee Shop, Inc.** does not appear in the list, select **+ New** to create a new account, enter `Test Coffee Shop, Inc.` for **Account Name**, and select **Save & Close**.
6. Select the **Products** tab.
7. Select the following values:
   - **Price List:** Filter Direct
   - **Revenue:** System Calculated
8. Above the subgrid, select **+ Add products.**
9. On the **Add products** panel, for each product, update the 
   **Quantity** and select **Add**:
   - **Airpot XL 6 month filter** — Quantity: `6`
   - **Airpot XL Pot Extender** — Quantity: `1`
   - **Airpot XL Reservoir Extension** — Quantity: `1`
10. Select **Save to Opportunity**
11. Double click on the **Airpot XL 6 Month Filter** product.
12. Locate the **Volume Discount** field and notice that no discount is applied.
13. Change **Quantity** to `15` and select outside the field.
    > [!NOTE]
    > The discount is now applied and the **Volume Discount** field shows the discounted value.
14. Select **Save & Close.**

#### Task 2 – Create Quote
In this task, you will create a Quote from the Opportunity you created in Task 1.
1. If necessary, open the **Sales Hub** app and ensure you are in 
   the **Sales** area.
2. Open the **Interested in Airpot XL Accessories** opportunity.
3. Select the **Quotes** tab.
4. Above the subgrid, select **+ New Quote.**
    > [!NOTE]
    > The quote form opens with relevant information copied from 
    > the opportunity.
5. Review the **Products** subgrid and verify that the products and 
   quantities are correct.
    > [!NOTE]
    > You can modify quantities and apply discounts to individual 
    > line items if needed.
6. On the command bar, select **Activate Quote**.
    > [!NOTE]
    > Depending on your browser size, you may need to select the 
    > ellipsis (**⋮**) to find this option.
7. On the command bar, select **Export to PDF**, then select **Print Quote for Customer**.
8. Select **Download** and open the generated document to review 
   the quote.
9. Close the PDF.
10. Close the **Export to PDF** window.

