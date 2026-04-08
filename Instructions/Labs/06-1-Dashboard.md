---
lab:
  title: 'Lab 6.1: Configure a dashboard'
  description: 'Upon successful completion of this lab, you will be able to:'
  duration: 30 minutes
  level: 100
  islab: true
---

# Module 6: Analyze Dynamics 365 Sales data

## Practice Lab 6.1: Configure a dashboard

### Scenario
Contoso Coffee’s sales managers want to monitor their sales team’s success more effectively, especially around closed opportunities. One sales manager has requested a personal dashboard that will provide them with an overview of recently closed opportunities and their sellers' actions against them. Additionally, they would like this dashboard to be their default dashboard when they open the Dashboards section of the application.

Upon successful completion of this lab, you will be able to:
- Create personal dashboards
- Add components to dashboards

This lab will take approximately **30** minutes to complete.

## Exercise 1 - Configure a dashboard 
### Task 1 - Create a dashboard

1. If necessary,go to your Dynamics 365 Sales Hub application.
2. In the bottom-left corner, select **Sales** from the **Change area** menu.
3. In the left navigation, under **My Work** group, select **Dashboards**.
4. Review the **Sales Activity Social Dashboard** that appears by default. 
   Select the dropdown arrow next to the dashboard title to view the other 
   available system dashboards.
5. When you're ready to create your own dashboard, select **+ New**, and then select **Dynamics 365 Dashboard.**
6. Review the available dashboard layouts, then select **2-Column Regular Dashboard** and select **Create**.

### Task 2 - Add components
1. In the **Name** field, enter *Sales Manager Dashboard*.
   > [!NOTE]
   > The dashboard designer opens in a new window and may take a minute to 
   > load. If it does not open, ensure that your browser's pop-up blocker 
   > is disabled.
2. Sales managers need a graphical view of won versus lost revenue from 
   opportunities. To accomplish this, select the **Insert Chart** icon in 
   the upper-left section.
3. Configure the chart with the following details, then select **Add**:
   - **Record Type:** Opportunity
   - **View:** Closed Opportunities
   - **Chart:** Deals Won vs. Deals Lost
4. Verify that the chart appears in the upper-left section.
5. Select the following details for your chart:
   - Record Type: Opportunity
   - View: Closed Opportunities
   - Chart: Deals Won vs. Deals Lost
   - Select **Add.**
6. Your chart will appear in the upper left section.
7. Sales managers need a way to review recently closed opportunities to 
   check in with sellers on lessons learned. The view should include both 
   won and lost opportunities closed in the current fiscal year. To 
   accomplish this, select the **Insert List** icon in the upper-right section.
8. Configure the list with the following details, then select **Add**:
   - **Record Type:** Opportunities
   - **View:** Closed Opportunities in Current Fiscal Year

### Task 3 - Save and edit the dashboard
1. Select **Save** and then **Close**. Your window will close and you will be returned to the Dashboards form, where your new dashboard will be displayed.
2. Select **Set As Default** from the command bar. This dashboard will now be your default dashboard when you navigate to the Dashboards section.
3. Select **Edit** from the top menu. You will return to the dashboard designer in another new window. Add two more components beneath your chart. The components you select should solve the following business requirements requested by sales managers:
   - Sales managers would like to get a sense of how individual sellers are doing based on their closed opportunity revenue. They would like a chart that shows seller names and their total revenue from closed opportunities.
   - Sales managers would like to monitor the day-to-day tasks of the sellers on their team. They would like to see a list that shows their sales teams' activities.
