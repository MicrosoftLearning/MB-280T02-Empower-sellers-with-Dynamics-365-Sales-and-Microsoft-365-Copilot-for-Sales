---
lab:
    title: 'Lab 3.1: Configure the product catalog'
---

# Module 3: Manage orders and product catalog with Dynamics 365

## Practice Lab 3.1 – Manage product catalog

### Scenario
As Contoso Coffee grows, they are looking to standardize their pricing structure and allow for easier creation of quotes, orders, and invoices with more accurate pricing and product details. Contoso Coffee recently released its newest smart coffee machine. As a functional consultant on their Dynamics 365 for Sales implementation, you have been asked to configure the product catalog.

Upon successful completion of this lab, you will be able to:
- Create unit groups
- Define price lists
- Create discount lists
- Define products and product families

### Exercise 1 – Product Catalog

#### Task 1 – Create Unit Group
In this task, you will create unit groups for the speakers.
1. Go to your Dynamics 365 Sales Hub application.
2. Click into the Change area menu (located in lower left side of screen). By default, Sales will be displayed in the bottom of the left menu.
3. From the menu that appears, select **App Settings.**
4. Select **Unit Groups** from the Product Catalog section of the left menu.
5. Click **+ New.**
6. Enter **Filters** for Name, enter **Each** for Primary Unit, and click **OK.**
7. Once the Unit Group opens, select the Related tab and choose **Units.**
8. You will find that you only have the default unit Each now; you will add three more units. Click **+ New Unit.**
9. Enter *Speaker* for Name, *1* for Quantity, select **Each** for Base Unit, and click **Save & Create New** by selecting the **˅** dropdown icon to the right of the Save & Close button.
10. Enter *Pack* for Name, *2* for Quantity, select **Filter** for Base Unit and click **Save & Create New.**
11. Enter *Value Pack* for Name, *2* for Quantity, select **Pack** for Base Unit and click **Save and Close.**
12. You should now have four unit groups in the list.

#### Task 2 – Create Discount List
In this task, you will create a Discount List for people that buy 15 or 20 or more filters. The 15 filters will get a 15% discount and 20 to 50 filters will get a 25% discount.
1. Select **Discount Lists** from the Product Catalog section of the left menu.
2. Click **+ New.**
3. Enter *Quantity Discount* for Name, select **Percentage** for Type, and click **Save.**
4. Click **Related** and choose **Discounts.**
5. Click **+ New Discount.**
6. Make sure Quantity Discount is selected for Discount Type, enter *15* for Begin Quantity, *19* for End Quantity, *15* for Percentage and click **Save.**
7. Click **+ New** again.
8. Select **Quantity Discount** for Discount Type. Then enter *20* for Begin Quantity, *50* for End Quantity, enter *25* for Percentage, and click **Save.**

#### Task 3 – Create Price List
In this task, you will create a price list for the filters.
1. Select **Price Lists** from the Product Catalog section of the left menu.
2. Click **+ New.**
3. Enter *Filter Direct* for Name, select **US Dollar** for Currency, and click **Save & Close.**

#### Task 4 – Create Products
In this task, you will create products.
1. Click on the **App Settings** change area.
2. Select **Sales.**
3. Select **Products** from the Collateral section of the left menu.
4. Click **Add Product.**
5. Enter *Airpot XL 6 month filter* for Name, enter *AXL6MF-1234* for Product ID, select **Filters** for Unit Group, select **Filter** for Default Unit, enter *2* for Decimals Supported, and click **Save.** (You may need to select the blue check mark next to the decimals supported to accept the suggestion.)
6. Select the **Additional Details** tab.
7. Click the **vertical ellipsis** on the top right of the Price List Items section. Click **+ New Price List** Item.
8. Select **Filter Direct** for Price List, select **Quantity Discount** for Discount List, and select **Whole** for Quantity Selling Option.
9. Select the **Pricing Information** tab, enter *25* for Amount and select **Save & Close.**
10. If Auto publish is enabled, skip this step. (Publish will not appear on the command bar.) Otherwise, select **Publish** and **Confirm** to publish the product.
11. In the left menu, select **Products** in the Collateral group.
12. Click **Add Product.**
13. Enter *Airpot XL Reservoir Extension* for Name, enter *AXLRE-4321* for Product ID, select **Default Unit** for Unit Group, select **Primary Unit** for Default Unit, select the blue checkmark next to the 2 for Decimals Supported, and click **Save.**
14. Select the **Additional Details** tab.
15. Click the **vertical ellipsis** on the top right of the Price List Items section. Click **+ New Price List Item.**
16. Select **Filter Direct** for Price List. Select **Whole** for Quantity Selling Option.
17. Select the **Pricing Information** tab, enter *$299* for Amount and select **Save & Close.**
18. If Auto publish is enabled, skip this step. Otherwise, select **Publish** and **Confirm** to publish the Product.
19. Select **Products** from the left menu.
20. Click **Add Product.**
21. Enter *Airpot XL Pot Extender* for Name, enter *AXPLE-7894* for Product ID, select **Default Unit** for Unit Group, select **Primary Unit** for Default Unit, select the blue check mark next to the 2 for Decimals Supported, and click **Save.**
22. Select the **Additional Details** tab.
23. Click the **vertical ellipses** on the top right of the Price List Items section. Click **+ New Price List Item.**
24. Select **Filter Direct** for Price List. Select **Whole** for Quantity Selling Option.
25. Select the **Pricing Information** tab, enter *199* for Amount and select **Save & Close.**
26. If Auto publish is enabled, skip this step. Otherwise, select **Publish** and **Confirm** to publish the Product.
27. From the left menu, select **Products.**
28. The products you created should show up on the All Products, Families & Bundles view. You can switch to this view by selecting the **˅** dropdown icon next to the default view title. You can use the **Filter by keyword box** to search for your prefix to find your products.
