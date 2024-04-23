# Tessa's Coffee Sales

<img width="798" alt="pic14" src="https://github.com/edbeato/coffee_sales/assets/163080154/7edf519d-7423-448f-ae63-ba38be4d6239">

## Summary

I combined and cleaned Tessa's Coffee sales data to include all the customer, product, and order information. I then analyzed it by using pivot tables to discover trends and patterns in the sales. I finalized the project by creating an interactive dashboard that clearly dispalys the data.

[Dashboard: Tessa's Coffee Sales](https://github.com/edbeato/tessas_coffee_sales/blob/829372fc740886c620f642fe6389b69dbd0bb2e1/Sales%20Dashboard.xlsx)

[Raw Data: Tessa's Coffee Sales](https://github.com/edbeato/tessas_coffee_sales/blob/19b894fc9a04b08e9de3c76cdb73fda7918a7351/Raw%20Data.xlsx)

## Scenario

## About the Company

Tessa's Coffee is a small online company that sells coffee beans to individuals across the United States, United Kingdom, and Ireland. They sell arabica, robusta, excelsa, and liberica coffee beans with a roast type of light, medium, or dark. Customers can buy packages of different sizes ranging from 0.2 kg to 2.5 kg. 

## Guiding Questions 

Could I combine scenario, about the company, and guiding questions all under scenario.

## Combining the Data

The [raw data](https://github.com/edbeato/tessas_coffee_sales/blob/19b894fc9a04b08e9de3c76cdb73fda7918a7351/Raw%20Data.xlsx) began with three separate sheets: orders, customers, and products. To prepare the sales data for analysis, I decided to bring all the relevant information from the customers and produts sheets into the orders sheet. This meant creating the following columns in the order sheet:

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
- Tessa's company sells packages in kilograms so I added that to the size column.
- Tessa's company is an american company so I made sure that unit prices and sales were in USD.

4.) With the company being international, I wanted to make sure that the dates were clearly understood by all parties. To ensure this I changed the month from a numerical value to an abbreviation. 

## Analyzing the Data

There were three categories of the data that I wanted to highlight: (I did this by creating pivot tables to and compaing different variables)

1.) Total sales over time

2.) Sales broken down by country

3.) Customers who've spent the most money

These three categories give us a good pciture of the sales for the company, but I also created filters for order date, roast type, size, and loyalty card so that we could see how each of these factors affects the sales. 

## Conclusions
