# Portfolio Project 1: SQL and Power BI, AdventureWorks

I took the AdventureWorks dataset, a sample sales database from a fictional bike manufacturer covering products, customers, and transactions, and turned it into a full end to end analytics project. Cleaned the data with SQL, built a three page interactive dashboard in Power BI, and exported a static PDF version.

## Build Process

I wrote SQL queries to clean four data tables, keeping only the columns needed for the dashboard and exporting each one as a CSV. From there I imported the four CSVs plus an Excel worksheet into Power BI and linked them together in the Model tab.

![Data model](https://user-images.githubusercontent.com/122973220/213426036-5aa569b0-9f8d-4b82-bbb2-2d242e2c7e09.jpg)

Next I used Power Query to rename columns, fix data types, and shape everything into a format ready for visualization. Then I built the three page dashboard and exported a PDF copy.

## Page 1: Sales Overview

![Sales overview](https://user-images.githubusercontent.com/122973220/213424939-2e4614c7-28f2-4f25-9691-e53f7aa9f368.jpg)

## Page 2: Sales by Customer

![Sales by customer](https://user-images.githubusercontent.com/122973220/213426418-36348415-aa68-42e7-90a2-81b0306cd30f.jpg)

## Page 3: Sales by Product

![Sales by product](https://user-images.githubusercontent.com/122973220/213426517-39db89b9-88e1-4241-9844-bd65cfadb686.jpg)

## Project Files

Three project files here, one SQL script, one Power BI file, one PDF, plus five data files, four CSVs and one Excel worksheet.

The full AdventureWorks Data Warehouse file is 99 MB, over GitHub's 25 MB limit, so it is not included in this repo. Download it directly from Microsoft:

[AdventureWorksDW2019.bak](https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorksDW2019.bak)

The original Microsoft Learn link is also in my SQL script file. This file comes in backup format, so I restored it through SQL Server Management Studio to unlock the full dataset, then ran a script from TechTalkCorner to update several date columns before starting my own analysis:

[Update_AdventureWorksDW_Data.sql](https://github.com/techtalkcorner/SampleDemoFiles/blob/master/Database/AdventureWorks/Update_AdventureWorksDW_Data.sql)

## What Is Next

I am rebuilding this pipeline with Python in addition to SQL and R, with the goal of full automation, pulling data from a database, cleaning it, building the dashboard, exporting it as a PDF, and emailing it to stakeholders with no manual steps beyond periodic checks.
