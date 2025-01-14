---
lab:
    title: 'Lab 3: Build quotes'
---

# TW-7003: Optimize sales processes with Dynamics 365 Sales

## Lab 3 – Build quotes

### Scenario
As a sales analyst for the Dynamics 365 Sales implementation at Contoso Coffee, you want to ensure that salespeople will be able to leverage the product catalog enhancements throughout the entire sales lifecycle. To ensure the functionality is working correctly, you will test the process of building a quote from a new opportunity.

Upon successful completion of this lab, you will be able to:
- Create opportunities and add opportunity line items
- Generate a quote from an opportunity

### Exercise 1 – Create a Quote

#### Task 1 – Add Products Line Items
In this task, you will create an Opportunity and add Products Line Items.
1. Go to your Dynamics 365 Sales Hub application.
1. In the left menu, under the **Sales** section, select **Opportunities**.
1. Select **+ New** in the top command bar.
1. Enter in the **Opportunity information** section: 

    - Topic: **Interested in Airpot XL Accessories**
    - Contact: **Jon Doe**

1. In the record header at the top select the **down arrow** next to the Owner field.
1. Enter and select **Doe Inc.** for **Account**.
1. Select **Save** in the command bar.
1. Select the **Products** tab.
1. You must select a Price List before you can add Opportunity Products. Select **Filter Direct** for **Price List**.
1. Select **System Calculated** for **Revenue**.
1. In the same section, down and to the right of that field, select **+ Add products**.

    ![Add products](./Media/add-products.png)

1. From the All products tab, find **Airpot XL 6 Month Filter**, enter *6* for **Quantity**, select **Add**.
1. For **Airpot XL Pot Extender**, leave *1* for **Quantity**, and select **Add**.
1. For **Airpot XL Reservoir Extension**, leave *1* for **Quantity**, and select **Add**.

    You will see three products are added. 
    
1. Select **Save to Opportunity**.
1. Hover over the **Airpot XL 6 Month Filter** product, and select the right arrow to navigate to it.

    ![Navigate to opportunity](./Media/nav-to-opp.png)

1. Locate the **Volume Discount** field and note that there's no discount.
1. Enter *15* for **Quantity**.

    Select outside of the field. The discount will kick in and the Volume Discount field will show a new value.
1. Select **Save & Close** in the command bar.

#### Task 2 – Create Quote
In this task, you will create a Quote from the Opportunity you created in Task 1.
1. If not there already, go to your Dynamics 365 Sales Hub application.
2. If necessary, open the opportunity you created in the previous task. It will be called **Interested in Airpot XL accessories.**
3. Select the **Quotes** tab.
4. Above the subgrid, Click **+ New Quote.**
5. The Quote form will open, and relevant information will be copied from the Opportunity.
6. On the Interested in Airpot XL Accessories Quote page, examine the Products sub-grid and make sure products and their quantities look as you expected. You can change the quantities and discount the price of each line item.
7. On the Command bar, select **Activate Quote.** (Depending on the size of your browser, you may need to select the ellipses to see this option.)
8. Click **Export to PDF** located on the command bar and select **Print Quote for Customer.** Click **Download.**
9. Open the generated document and see what the Quote looks like.
10. Close the PDF.
11. Close the Export to PDF window.

