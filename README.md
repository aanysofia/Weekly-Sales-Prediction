# Weekly-Sales-Prediction

### Goal of the project:
The goal of the project is to predict the weekly sales of Walmart stores.

### Dataset 
The data is obtained from Kaggle competition. (https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting/overview)
Historical sales data for 45 Walmart stores located in different regions in US with the type and size of store was provided. Each store contains a number of departments. In addition, Walmart runs several promotional markdown events throughout the year. These markdowns precede prominent holidays, the four largest of which are the Super Bowl, Labor Day, Thanksgiving, and Christmas. The weeks including these holidays are weighted five times higher in the evaluation than non-holiday weeks. Part of the challenge presented by this competition is modeling the effects of markdowns on these holiday weeks in the absence of complete/ideal historical data.

#### Train data
The historical training data, covers to 2010-02-05 to 2012-11-01. Within this file the following fields are there:
•	Store - the store number
•	Dept - the department number
•	Date - the week
•	Weekly_Sales -  sales for the given department in the given store
•	IsHoliday - whether the week is a special holiday week

#### Test data
This file is identical to train.csv, except we have withheld the weekly sales. You must predict the sales for each triplet of store, department, and date in this file.

#### Features
This file contains additional data related to the store, department, and regional activity for the given dates. It contains the following fields:
•	Store - the store number
•	Date - the week
•	Temperature - average temperature in the region
•	Fuel_Price - cost of fuel in the region
•	MarkDown1-5 - anonymized data related to promotional markdowns that Walmart is running. MarkDown data is only available after Nov 2011, and is not available for all stores all the time. Any missing value is marked with an NA.
•	CPI - the consumer price index
•	Unemployment - the unemployment rate
•	IsHoliday - whether the week is a special holiday week


### Requirements

- pyenv
- python==3.9.4

### Setup

For this purpose, use following commands:

```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```
