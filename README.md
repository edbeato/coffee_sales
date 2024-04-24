# Tessa's Coffee Sales

<img width="798" alt="pic14" src="https://github.com/edbeato/coffee_sales/assets/163080154/7edf519d-7423-448f-ae63-ba38be4d6239">

## Summary

I combined and cleaned Tessa's Coffee sales data to include all the customer, product, and order information. I then analyzed it by using pivot tables to discover trends and patterns in the sales. I finalized the project by creating an interactive dashboard that clearly dispalys the data.

[Dashboard: Tessa's Coffee Sales](https://github.com/edbeato/tessas_coffee_sales/blob/829372fc740886c620f642fe6389b69dbd0bb2e1/Sales%20Dashboard.xlsx)

[Raw Data: Tessa's Coffee Sales](https://github.com/edbeato/tessas_coffee_sales/blob/19b894fc9a04b08e9de3c76cdb73fda7918a7351/Raw%20Data.xlsx)

## Scenario

Tessa's Coffee is a small online company that sells coffee beans to individuals across the United States, United Kingdom, and Ireland. They sell arabica, robusta, excelsa, and liberica coffee beans with a roast type of light, medium, or dark. Customers can buy packages of different sizes ranging from 0.2 kg to 2.5 kg. 

**I have been tasked with creating a dashboard that will highlight all of their sales from 2019 - 2022.**

## Combining the Data

The [raw data](https://github.com/edbeato/tessas_coffee_sales/blob/19b894fc9a04b08e9de3c76cdb73fda7918a7351/Raw%20Data.xlsx) was stored in an excel file with 1001 entries organized in three separate sheets: orders, customers, and products. To prepare the sales data for analysis, I decided to bring all the relevant information from the customers and produts sheets into the orders sheet. This meant creating the following columns in the order sheet:

- customer name
- email
- country
- coffee type
- roast type
- size
- unit price
- loyalty card

I was able to do this using the **XLOOKUP, INDEX and MATCH** functions.

## Cleaning the Data

Once I had all of the key data from the sheets in one place, I needed to make sure that I created the columns needed to analyze the sales data. I also formatted it so that it was easily understood by anyone looking through the data. 

1.) I created a sales column by multiplying the quantity of the order by the unit price. 

2.) The coffee type was initially populated with abbreviations. Having the full name of the coffee type would be more clear so I created a new column called *coffee type name* using the **IF** function.

3.) Since the company does international business, I wanted to make sure that the all of the units were clear.
- The size column initially had only a numeric value in it. Tessa's Coffee sells packages in kilograms so I added that to the column.
- The unit price and sales column initially only had a numeric value. Tessa's Coffee is an american company so I made sure that unit prices and sales were in USD.

4.) With the company being international, I wanted to make sure that the dates were clearly understood by all parties. To ensure this I changed the month from a numerical value to an abbreviation. 

## Creating the Dashboard

There were three categories of the data that I wanted to highlight:

**1.) Total sales over time**

I selected order data into the rows and grouped them by years and months. I put coffee type names into columns and sales as my values. Now that all of the data was in the pivot chart I inserted my line graph.

After this I created an order date timeline so that you could easily filter the data based on whatever months you wanted to look at. This is quickly done by inserting a timeline under the *Pivot Chart Analyze* tab. 

I also added slicers so that you could filter the data by size, roast type name, and loyalty card. This was done by inserting slicers under the *Pivot Chart Analyze* tab.

**2.) Sales broken down by country**

I created a bar chart using the countries as my rows and sales as my values.

**3.) Customers who've spent the most money**

I created another bar chart using the customer name as my rows and sales as my values. Tessa's Coffee has had many different customers over the years, so rather than displaying all of them, I decided to only display the top 5.

These three charts, along with the filters added, give us a great overview of the sales for Tessa's Coffee from 2019 - 2022. 
