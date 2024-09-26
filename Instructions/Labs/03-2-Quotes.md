---
lab:
    title: 'Lab 3.2: Build quotes'
---

# Module 3: Manage orders and product catalog with Dynamics 365

## Practice Lab 3.2 – Build quotes

### Scenario
As a sales analyst for the Dynamics 365 Sales implementation at Contoso Coffee, you want to ensure that salespeople will be able to leverage the product catalog enhancements throughout the entire sales lifecycle. To ensure the functionality is working correctly, you will test the process of building a quote from a new opportunity.

Upon successful completion of this lab, you will be able to:
- Create opportunities and add opportunity line items
- Generate a quote from an opportunity

### Exercise 1 – Create a Quote

#### Task 1 – Add Products Line Items
In this task, you will create an Opportunity and add Products Line Items.
1. Go to your Dynamics 365 Sales Hub application.
2. From the left menu, in the Sales group, select Opportunities.
3. Click + New.
4. Enter Interested in Airpot XL Accessories for Topic, and select Jon Doe for Contact.
5. In the record header at the top select the down arrow next to the Owner field, and choose Test Coffee Shop, Inc. for Account and select Save.
6. Select the Products tab.
7. You must select a Price List before you can add Opportunity Products. Select Filter Direct for Price List.
8. Select System Calculated for Revenue.
9. Above the subgrid, click + Add products.
10. From the All products list, find Airpot XL 6 Month Filter, enter 6 for Quantity, select Add.
11. Find AirpotXL pot extender in the list of products, enter 1 for Quantity and select Add.
12. Find Airpot XL Reservoir Extension in the list of products, enter 1 for Quantity and select Add.
13. You will see three products are Added. Select Save to opportunity.
14. Double click on the Airpot XL 6 Month Filter product.
15. Locate the Volume Discount field. You will find that there is no discount for buying one Speaker.
16. Change the Quantity to 15 and click out of the field. The Discount will now kick in and the Volume Discount field will show the discounted value.
17. Select Save & Close.

#### Task 2 – Create Quote
In this task, you will create a Quote from the Opportunity you created in Task 1.
1. If not there already, go to your Dynamics 365 Sales Hub application.
2. If necessary, open the Opportunity you created in the previous task. It will be called Interested in Airpot XL accessories.
3. Select the Quotes tab.
4. Above the subgrid, Click + New Quote.
5. The Quote form will open, and relevant information will be copied from the Opportunity.
6. On the Interested in Airpot XL Accessories Quote page. Examine the Products sub-grid and make sure products and their quantities look as you expected. You can change the quantities and discount the price of each line item.
7. On the Command bar, select Activate Quote.
8. Click Export to PDF located on the command bar and select Print Quote for Customer. Click Download.
9. Open the generated document and see what the Quote looks like.
10. Close the PDF.
11. Close the Export to PDF window.

