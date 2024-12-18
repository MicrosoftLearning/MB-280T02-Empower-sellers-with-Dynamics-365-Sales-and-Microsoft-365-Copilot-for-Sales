---
lab:
    title: 'Capstone'
---

# Capstone: Configure a product catalog for an organization

The applied workshop portion if the MB-280 course is designed to help students apply the skills they have learned throughout the course to a real-world example. The scenario has a variety of different elements included that span across Dynamics 365 Sales, Customer Insights - Journeys, and Customer Insights – Data. 

Based on the scenario provided below, you will create and configure your Dynamics 365 environment to meet the fictional company's business requirements. It is important to note that you don’t necessarily need to solve all the items addressed. Due to the amount of time allotted and what is included, you might only be able to address some of the items – which is okay and by design. 

**Important:** There is not necessarily a right or wrong way to accomplish this. Based on the criteria outlined in the scenario, you should produce and configure a solution based on how you see leveraging the different elements together.

At the end of the day, we will provide each student with 5 to 10 minutes to walk through part or all the solutions they created. 

## Scenario: Contoso Home Security 
Contoso Home Security is a direct-to-consumer home security equipment and monitoring company. Their products include smart doorbells, smart thermostats, security systems, moisture sensors, and more. Since they are direct to consumer, their products are sold either online or in their retail stores across 11 major US cities. Online customers are assigned an account representative. Their role is to follow up with the customer and attempt to provide them with additional products and services. 

In the upcoming exercises, we will explain their detailed business requirements.

## Time management 

You have the entire day (6.5 hours) to complete all aspects of this assignment. Review all the expectations first, then begin to manage your time. Phase 1 is designed to be a small group discussion; however, if you are working solo, take the time to brainstorm on your own to help you with the rest of the assignment. Most of your time should be spent in Phases 2 and 3. Your instructor will let you know when to start Phase 4, but plan for it to take about an hour of your time.

Plan for the following:
- **Phase 1:**  Small group discussion
- **Phase 2:**  Design your solution
- **Phase 3:** Build your solution
- **Phase 4:** Share and compare your solutions

### Phase 1: Small group discussion

Discuss with your small group how to design the solution. Have a brainstorming session about how you might approach the solution to solve the organization’s business requirements.

Consider the following:
1. What does Contoso's data model look like?
2. What configuration changes need to be made?
3. Is there any irrelevant information offered?

### Phase 2: Design your solution
Now you should plan how you will approach the solution. Put pen to paper (or digital, however it works for you) and make your to-do list.

Consider the following:
1. Do you need to create a new solution? Why or why not?
2. Should you edit existing assets or start from scratch?
3. Do you need to update or make a new security role?

### Phase 3: Build your solution
Time to configure your solution.

Consider the following:
1. What applications will you make certain configuration changes in?
2. Does the order in which you make your configuration changes matter? Where will you start?
3. How can I use my knowledge of user experience design to make my configuration changes work best for the users?

### Phase 4: Share and compare your solution
Share your work with your small group. Compare the experience as a customer experience analyst and as a user of their solution.

Consider the following:
1. What did other teams do differently? Did it still meet the business requirement?
2. How would you improve upon your solution?

## The Contoso product catalog
Contoso home security sells a variety of products and services. These are automatically added to deals so pricing can be calculated based the prices of the specific items each customer needs.

Contoso sells the following products:

| Product                            | Product Number | Est. Retail Price |
|------------------------------------|----------------|-------------------|
| A-100 Control Unit                 | A100-CU        | \$2200.00         |
| A-101 Smart Doorbell               | A101-SD        | \$500.00          |
| A-102 Security Sensor              | A102-SS        | \$150.00          |
| A-103 Thermostat                   | A103-T         | \$450.00          |
| A-104 Moisture Sensor              | A104-MS        | \$150.00          |
| A-105 Wired Outdoor Camera         | A105-WOC       | \$750.00          |
| A-106 Solor Outdoor Camera         | A106-SOC       | \$1500.00         |
| A-107 Indoor/Outdoor Camera        | A107-IOC       | \$500.00          |
| A-108 Motion Detectors             | A108-MD        | \$750.00          |
| A-109 Motion Activated Flood Light | A109-MAFL      | \$900.00          |

Contoso has two different ways that they price products. Individuals who purchase from the website or retail store get retail pricing. Corporate organizations receive corporate pricing which is 10% less than retail pricing.

