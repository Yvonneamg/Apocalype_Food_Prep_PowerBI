# Apocalypse Food Preparation_Power BI Project

## Overview
We are preparing to store food for a predicted apocalypse. We need tlo store food th\at is highly likely not to be perishable within a short period of time. This project utilizes **Power BI** 

The dataset contains information about the stores from which we purchase the products for the apocalypse.

## Key Findings
---
## Business Recommendations
---
## Business Problem
The business is preparing for an apocalypse. It needs to determine the most efficient way way to store up food.

This project seeks to answer the following questions:
1. Which store offers the best price combination in general
2. Which Store offers the best price by product
3.

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