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
2. In the bottom-left corner, select the **Sales** Change area.
3. From the menu that appears, select **App Settings.**
4. In the left navigation, under **Product Catalog** group, select **Unit Groups**.
5. Select **+ New.**
6. Enter the following values and select **OK**:
   - **Name:** *Filters*
   - **Primary Unit:** *Each*
7. Select the **Related** tab, then select **Units**.
8. On the command bar, select **+ New Unit**.

    > [!NOTE]
    > By default, the unit group contains only the **Each** unit.You will add three more units in the following steps
9. Enter the following values, then select the dropdown arrow next to 
   **Save & Close** and select **Save & Create New**:
   - **Name:** *Filter*
   - **Quantity:** *1*
   - **Base Unit:** Each

10. Enter the following values and select **Save & Create New**:
    - **Name:** *Pack`*
    - **Quantity:** *2*
    - **Base Unit:** Filter

11. Enter the following values and select **Save & Close**:
    - **Name:** *Value Pack*
    - **Quantity:** *2*
    - **Base Unit:** Pack

> [!NOTE]
> The unit group now contains four units — **Each**, **Filter**, **Pack**, and **Value Pack**.

#### Task 2 – Create Discount List
In this task, you will create a Discount List for people that buy 15 or 20 or more filters. The 15 filters will get a 15% discount and 20 to 50 filters will get a 25% discount.
1. In the left navigation, under **Product Catalog** group, select **Discount Lists**.
2. Select **+ New.**
3. Enter the following values and select **Save**:
   - **Name:** *Quantity Discount*
   - **Type:** *Percentage*
4. Select the **Related** tab, then select **Discounts**.
5. Select **+ New Discount**.
6. Enter and select the following values, then select **Save**:
   - **Discount Type:** Quantity Discount
   - **Begin Quantity:** *15*
   - **End Quantity:** *19*
   - **Percentage:** *15*
7. Select **+ New**.
8. Enter and select the following values, then select **Save**:
   - **Discount Type:** Quantity Discount
   - **Begin Quantity:** *20*
   - **End Quantity:** *50*
   - **Percentage:** *25*

#### Task 3 – Create Price List
In this task, you will create a price list for the filters.
1. In the left navigation, under **Product Catalog** group, select **Price Lists**.
2. Select **+ New.**
3. Enter and select the following values, then select **Save & Close**:
   - **Name:** *Filter Direct*
   - **Currency:** US Dollar

#### Task 4 – Create Products
In this task, you will create products.
1. In the bottom-left corner, select the **App Settings** Change area.
2. From the menu that appears, select **Sales.**
3. In the left navigation, under **Collateral**, select **Products**.
4. Select **Add Product** 
5. Enter and select the following values, then select **Save**:
   - **Name:** `Airpot XL 6 month filter`
   - **Product ID:** *AXL6MF-1234*
   - **Unit Group:** Filters
   - **Default Unit:** Filter
   - **Decimals Supported:** *2*
    > [!NOTE]
    > If a suggestion appears next to **Decimals Supported**, select the blue checkmark to accept it.

6. Select the **Additional Details** tab.
7. In the **Price List Items** section, select the vertical ellipsis (**⋮**) and select **+ New Price List Item**.
8. Select the following values:
   - **Price List:** Filter Direct
   - **Discount List:** Quantity Discount
   - **Quantity Selling Option:** Whole
9. Select the **Pricing Information** tab, enter *25* for Amount and select **Save & Close**.
10. If Auto publish is enabled, skip this step. (Publish will not appear on the command bar.), otherwise, select **Publish** and **Confirm** to publish the product.
11. In the left navigation, under **Collateral** group, select **Products**.
12. Select **Add Product.**
13. Enter and select the following values, then select **Save**:
    - **Name:** *Airpot XL Reservoir Extension*
    - **Product ID:** *AXLRE-4321*
    - **Unit Group:** Default Unit
    - **Default Unit:** Primary Unit
    - **Decimals Supported:** *2*
14. Select the **Additional Details** tab.
15. In the **Price List Items** section, select the vertical ellipsis (**⋮**) and select **+ New Price List Item**.
16. Select the following values:
    - **Price List:** Filter Direct
    - **Quantity Selling Option:** Whole
17. Select the **Pricing Information** tab, enter *299* for **Amount**, then select **Save & Close**
18. If Auto publish is enabled, skip this step. Otherwise, select **Publish** and **Confirm** to publish the Product.
19. In the left navigation, under **Collateral** group, select **Products**.
20. Select **Add Product.**
21. Enter and select the following values, then select **Save**:
    - **Name:** *Airpot XL Pot Extender*
    - **Product ID:** *AXPLE-7894*
    - **Unit Group:** Default Unit
    - **Default Unit:** Primary Unit
    - **Decimals Supported:** *2*
22. Select the **Additional Details** tab.
23. In the **Price List Items** section, select the vertical ellipsis (**⋮**) and select **+ New Price List Item**.
24. Select the following values:
    - **Price List:** Filter Direct
    - **Quantity Selling Option:** Whole
25. Select the **Pricing Information** tab, enter *199* for **Amount**, then select **Save & Close**.
26. If Auto publish is enabled, skip this step. Otherwise, select **Publish** and **Confirm** to publish the Product.
27. In the left navigation, under **Collateral** group, select **Products**.
> [!NOTE]
>The products you created should show up on the All Products, Families & Bundles view. You can switch to this view by selecting the **˅** dropdown icon next to the default view title. 
