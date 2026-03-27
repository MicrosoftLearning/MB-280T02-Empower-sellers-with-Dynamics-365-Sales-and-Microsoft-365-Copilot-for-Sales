---
lab:
  title: 'Lab 3.1: Configure the product catalog'
  description: In this task, you will create a price list for the filters.
  duration: 30 minutes
  level: 100
  islab: true
---

# Module 3: Manage orders and product catalog with Dynamics 365

## Practice Lab 3.1 – Manage product catalog

### Scenario
As Contoso Coffee grows, they are looking to standardize their pricing structure and allow for easier creation of quotes, orders, and invoices with more accurate pricing and product details. Contoso Coffee recently released its newest smart coffee machine. As a functional consultant on their Dynamics 365 Sales implementation, you have been asked to configure the product catalog.

Upon successful completion of this lab, you will be able to:
- Create unit groups
- Define price lists
- Create discount lists
- Define products and product families

This lab will take approximately **30** minutes to complete.

### Exercise 1 – Product Catalog

#### Task 1 – Create Unit Group
In this task, you will create unit groups for a line of coffee machine filters.
1. Go to your Dynamics 365 Sales Hub application.
2. In the bottom-left corner, select the **Sales** area switcher.
3. From the menu that appears, select **App Settings.**
4. In the left navigation, under **Product Catalog** group, select **Unit Groups**.
5. Select **+ New.**
6. Enter the following values and select **OK**:
   - **Name:** `Filters`
   - **Primary Unit:** `Each`
7. Select the **Related** tab, then select **Units**.
8. On the command bar, select **+ New Unit**.

    > [!NOTE]
    > By default, the unit group contains only the **Each** unit.You will add three more units in the following steps
9. Enter the following values, then select the dropdown arrow next to 
   **Save & Close** and select **Save & Create New**:
   - **Name:** `Filter`
   - **Quantity:** `1`
   - **Base Unit:** `Each`

10. Enter the following values and select **Save & Create New**:
    - **Name:** `Pack`
    - **Quantity:** `2`
    - **Base Unit:** `Filter`

11. Enter the following values and select **Save & Close**:
    - **Name:** `Value Pack`
    - **Quantity:** `2`
    - **Base Unit:** `Pack`

> [!NOTE]
> The unit group now contains four units — **Each**, **Filter**, **Pack**, and **Value Pack**.

#### Task 2 – Create Discount List
In this task, you will create a Discount List for people that buy 15 or 20 or more filters. The 15 filters will get a 15% discount and 20 to 50 filters will get a 25% discount.
1. In the left navigation, under **Product Catalog** group, select **Discount Lists**.
2. Select **+ New.**
3. Enter the following values and select **Save**:
   - **Name:** `Quantity Discount`
   - **Type:** `Percentage`
4. Select the **Related** tab, then select **Discounts**.
5. Select **+ New Discount**.
6. Enter the following values and select **Save**:
   - **Discount Type:** `Quantity Discount`
   - **Begin Quantity:** `15`
   - **End Quantity:** `19`
   - **Percentage:** `15`
7. Select **+ New**.
8. Enter the following values and select **Save**:
   - **Discount Type:** `Quantity Discount`
   - **Begin Quantity:** `20`
   - **End Quantity:** `50`
   - **Percentage:** `25`

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
28. The products you created should show up on the All Products, Families & Bundles view. You can switch to this view by selecting the **˅** dropdown icon next to the default view title. 
