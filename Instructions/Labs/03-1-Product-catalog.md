---
lab:
    title: 'Lab 2: Configure the product catalog'
---

# TW-7003: Optimize sales processes with Dynamics 365 Sales

## Lab 2 – Manage product catalog

### Scenario
As Contoso Coffee grows, they are looking to standardize their pricing structure and allow for easier creation of quotes, orders, and invoices with more accurate pricing and product details. Contoso Coffee recently released its newest smart coffee machine. As a functional consultant on their Dynamics 365 Sales implementation, you have been asked to configure the product catalog.

Upon successful completion of this lab, you will be able to:
- Create unit groups
- Define price lists
- Create discount lists
- Define products and product families

### Exercise 1 – Product Catalog

#### Task 1 – Create Unit Group
In this task, you will create unit groups for a line of coffee machine filters.
1. Go to your Dynamics 365 Sales Hub application.
1. Select **Sales** (default option for the Change Area menu) in the lower-left, then select **App Settings**.

    ![Change Area - App Settings](./Media/change-area-app-settings.png)

1. Under the **Product Catalog** section on the left menu, select **Unit Groups**.
1. Select **+ New** on the top command bar.
1. Enter the following information in **Create Unit Group**:

    - Name: **Filters**
    - Primary Unit: **Each** 

1. Once the Unit Group opens, select the **Related** tab, then select **Units**.

    ![Related tab](./Media/related-tab.png)

    You will find that you only have the default unit **Each** now. You will add three more units. 

1. Select **+ New Unit** at the top of the **Unit Group Units Associated View** section.
1. Enter the following information in **Quick Create: Unit**:

    - Name: **Filter**
    - Quantity: **1** 
    - Base Unit: **Each**

1. Select the **˅** dropdown icon to the right of the **Save and Close** button, then select **Save & Create New**.

1. Enter the following information:

    - Name: **Pack**
    - Quantity: **2** 
    - Base Unit: **Filter**

1. Select the **˅** dropdown icon, then select **Save & Create New**.

1. Enter the following information:

    - Name: **Value Pack**
    - Quantity: **2** 
    - Base Unit: **Pack**

1. Select **Save and Close**.

    You will now see the four unit groups in the list.

#### Task 2 – Create Discount List
In this task, you will create a Discount List for people that buy 15 or 20 or more filters. The 15 filters will get a 15% discount and 20 to 50 filters will get a 25% discount.

1. Under the **Product Catalog** section on the left menu, select **Discount Lists**.
1. Select **+ New** on the top command bar.
1. Use the following information for the **New Discount List**:

    - Name: **Quantity Discount**
    - Type: **Percentage** 

1. Select **Save** on the command bar.
1. Select the **Related** tab, then select **Discounts**.
1. Select **+ New Discount** at the top of the **Discount Associated View** section.

1. Enter the following information for the **New Discount List**:

    - Discount Type: **Quantity Discount**
    - Begin Quantity: **15** 
    - End Quantity: **19**
    - Percentage: **15**

1. Select **Save**.
1. Select **+ New** again.
1. Enter the following information:

    - Discount Type: **Quantity Discount**
    - Begin Quantity: **20** 
    - End Quantity: **50**
    - Percentage: **25**

1. Select **Save**.

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
