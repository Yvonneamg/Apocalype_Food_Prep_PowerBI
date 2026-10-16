# Apocalypse Food Preparation_Power BI Project

## Overview
We are preparing to store food for a predicted apocalypse. We need to store food that is highly likely not to be perishable within a short period of time. 

We are also analysing the sales of a particular store for the apocalypse.

This project utilizes **Power BI** 

The datasets contains information about the stores from which we purchase the products for the apocalypse as well as information on sales for a single store.

## Key Findings
1. Costco is the cheapest store in general at **210** compared to the other 2 stores.
2. For **Rice** Target has the best price, 2 dollars cheaper than Costco, however, Costco offers the best prices for **Dried Beans** and **Bottled Water**. All stores have similar prices for **Canned Vegetables** so it is insignificant where we buy.
---
## Business Recommendations
- We should buy rice from **Target** and the rest of the items from **Costco** provided it is not logistically expensive to go to target then back to Costco.
---
## Business Problem
The business is preparing for an apocalypse. It needs to determine the most efficient way way to store up food and the other business is trying to understand its sales patterns for the apocalypse.

This project seeks to answer the following questions:
1. Which store offers the best price combination in general
2. Which Store offers the best price by product
3. What is our total revenue, production cost and gross profit
4. Which is our top selling product by products sold and profit per product
5. Who is our top customer
6. Which is the highest selling day of the week during the 3 months.

---

## The Datasets

The initital raw dataset is obtained from [GitHub](https://github.com/AlexTheAnalyst/Power-BI/blob/main/Apocolypse%20Food%20Prep.xlsx)

The dataset with pivot table is obtained from [GitHub](https://github.com/AlexTheAnalyst/Power-BI/blob/main/Apocolypse%20Food%20Prep%20-%20Power%20Query%20Editor%20Tutorial.xlsx)

The dataset with information on different related sheets is obtained from [GitHub](https://github.com/AlexTheAnalyst/Power-BI/blob/main/Apocolypse%20Food%20Prep%20-%20Relationship%20Tutorial.xlsx). It contains three sheets with stores information, sales information and customers information.

The initital raw dataset contains **48** rows and **4** columns namely **stores** , the **product** names, the **price** and **date** of purchase. 

The dataset with pivot table  contains three sheets, **Purchase Tracker**, **Pivot Table** and **Purchase Overview**



---
## Analysis Approach

## Loading the data to Power BI and transformations using Power Query

The analysis is done on ** PowerBI** while utilizing *Power Query** for cleaning up the dataset.

To determine the top store by sales and top store by product sales I load initial raw dataset to PowerBI and use Power Query to perform the following transformations;

- Rename columns for clarity
- Transform columns to correct data types
- load the dataset back to Power BI 
- Create two visuals for the top store by sales and top store by product sales.


The dataset with pivot table  is loaded to Power BI then transformed using Power Query. Key transformations include;

- Deleting top two empty rows
- Promoting first row to header
- Deleting the grand total olumn
- Deleting subtotals by filtering the first column to remove empty rows
- Renaming columns acordingly for better clarity
- Changing data types to match the data ie. the date to be dates, text to be text and fixed decimal numbers to  be decimal numbers
- Unpivoting date columns
- The data is then loaded to PowerBI for visualizations

---


## Building Relationships

The dataset is loaded to power BI and a simple transformation is applied to check data correctness. It is then loaded to Power BI.

In the model view, I create relationships between the tables. I link **Cust ID** with **Customer ID** and **product ID** with **Product ID** in the respective tables. 

I ensure that the cross filter is set to **Both** instead of **single** to ensure accuracy in calculated measures.

I then set the correct relationships to be active and now the dataset is ready for visualization.

---

