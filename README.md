# SALES-DASHBOARD
## Problem Statement:

To uncover hidden sales insights and trends for the sales team, enabling better decision-making, and to automate the extraction of these insights, reducing the time otherwise spent gathering this information..

**Stakeholders Involved :**

- Marketing 
- Customer Service Team
- Data & Analytics Team (Outsource)
- IT

## End Result:

An automated sales dashboard and customer dashboard providing quick & latest sales insights in order to support data driven decision making.

**Success Criteria :**

1. Dashboards uncovering sales order insights and customer engagement with latest data available.
2. Sales team able to take better decisions and prove 10% cost saving of total spend.
3. Sales analyst stop data gathering manually in order to save 20% of their business time and reinvest it value added activity.

**Data Collection:**

From data warehouses data is being collected through online analytic processing system.

## Sales Dashboard Requirement

To present overview of the sales metrics and trends in order to analyze year on year sales performance and understand sales trends.

**KPI :**

Display a summary of total sales, profits and quantity for the current year and the previous year.

**Sales Trends:**

Present the data of each KPI on a monthly basis for both the current year and previous year. 

Identify months with highest and lowest sales and make them easy to recognize.

**Product subcategory Comparison:**

Compare sales performance by different product subcategories for the current year and the previous year .

Include a comparison of sales with profit.

**Weekly Trends for Sales and Profit :**

Present weekly sales and profits data for the current year.

Display the average weekly values.

Highlight weeks that are above and below the average to draw attention to sales and profit performance.

## Customer Dashboard Requirements

Show the distribution of customers based on the number of orders they have placed to provide insights into customer behaviour and engagement.

Present top 10 customer who have generated the highest profit for the company.

Show additional information like rank , number of orders current sales etc.

### Dynamic Interactive Requirements :

Dashboard should allow to check historical data with a button to select any particular year.

Ability to navigate between to dashboards easily.

Interactive graphs , enabling users to filter data using the charts on basis of regions , place , product category etc.

# Steps Involved

## TASK 1 : Extracting Data From MySQL

- Perform some analysis on data in SQL then hook the data to Tableau public .
- We will choose connection live when frequency of data is high (daily ) but if frequency is less then choose extract. We have choose Extract connection.

## TASK 2 : Data Transforming in Tableau or preprocessing

- join all the tables ( customer , date , order , product) to Transaction table (fact dimensions).
- removed  2 transaction which are from Newyork and London
- change currency transaction in USD.
- change sales amount range from 1 and above . To get rid of 0 and negative number.
- other important things like checking datatypes.

## TASK 3: Creating charts

To represent total sales, profits and quantity for the current year and the previous year. we will make bans charts.

1. KPI for Total Sales: Representing Total Sales , Percentage change wrt previous month. Showing trend on Sparkline chart with Max and Min values for every Year.
2. KPI for Total quantity: Representing Total Quantity , Percentage change wrt previous month. Showing trend on Sparkline chart with Max and Min values for every Year.
3. KPI for Total Profits: Representing Total Profits , Percentage change wrt previous month. Showing trend on Sparkline chart with Max and Min values for every Year.
4. Represent each of the KPI with proper formatting , color , size etc.

## TASK 4: Creating a chart to compare different subcategories

1. Bar under bar chart created to show CY sales and PY sales for each sub category.
2. Profit chart created alongside .
3. Proper formatting and coloring done.
4. worked on tooltip to show proper numbers.

## TASK 5: Creating a Weekly trend line for profit and sales in current year.

1. created line graph for both current year sales and current year profits .
2. created a reference line to show above and below average marks on profits and sales .
3. done proper formatting , give suitable colors to distinguish above and below average.
4. worked on the tooltip to show proper numbers.

## TASK 6 : Creating Dashboard

1. Creating a vertical container for Filters.
2. Creating a horizontal container for all other charts and KPI.
3. Adding Titles to Dashboard and navigating buttons for switching to Sales and Customer Dashboards.
4. Format the whole dashboard . 
5. Assigning colors to all containers .
6. Making legends for all the year and codings.
7. Making the Dashboard Dynamic by attaching filters to all .
