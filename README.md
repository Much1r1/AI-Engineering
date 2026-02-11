# AI-Engineer-Roadmap
# Phase 1: Car Rental Financial Data Analysis 🚗📊

## Project Overview
This project marks the first milestone in my **AI Engineer Roadmap**. The goal was to practice foundational data handling skills using Python and Pandas, focusing on a real-world dataset involving vehicle financial transactions.

## Dataset Description
The dataset represents the financial ledger of a vehicle rental company. It tracks:
* **Transactions:** Rental income, vehicle purchases, and miscellaneous costs.
* **Assets:** Unique vehicles identified by license plates (1,393 unique values).
* **Descriptions:** Detailed logs of the specific car models involved (e.g., FIAT ARGO, DUSTER).

## Key Objectives
1.  **Data Loading:** Efficiently importing large CSV files into a Pandas DataFrame.
2.  **Data Cleaning:** Identifying missing values and ensuring numerical consistency.
3.  **Exploratory Analysis:** Aggregating data to understand revenue vs. expenditure.

## Initial Insights
* **Transaction Mix:** Approximately 90% of the ledger entries are 'Rental' transactions, while 'Purchases' represent high-value capital outflows.
* **Data Integrity:** The dataset contains negative values (expenditures) and positive values (revenue), requiring careful handling during aggregation to avoid misleading sums.

## Potential AI Use Cases
Later in this roadmap, this data could be used to build:
* **Predictive Maintenance:** Forecasting when a vehicle might need service based on rental frequency.
* **Revenue Forecasting:** Predicting monthly income based on seasonal rental patterns.
* **ROI Analysis:** Calculating the "break-even" point for newly purchased vehicles.

---
### Technical Stack
* **Environment:** Google Colab
* **Language:** Python 3.x
* **Library:** Pandas

## Feature Engineering for App Integration
To prepare the data for a mobile UI, I implemented a feature engineering pipeline that:
* **Extracted Brands:** Parsed raw strings to identify manufacturers.
* **Categorized Fleet:** Developed a logic-based classifier to group vehicles into 'Economy', 'SUV', and 'Premium' tiers.
* **Engine Mapping:** Isolated engine displacement values to allow for user-side filtering by performance/efficiency.
