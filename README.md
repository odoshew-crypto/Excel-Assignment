### Data Cleaning and Preparation Notes

This document summarizes the data cleaning and preparation steps performed on the transactional dataset containing 632 entries.

### 1. Duplicate Handling

Duplicate Criteria:

Duplicates were identified based on the OrderID column, which serves as a unique identifier for each transaction.

Action Taken: 1 duplicate row was removed from the dataset.

### 2. Assumptions

The following assumptions were made during data cleaning and analysis:

Currency: All prices and costs are assumed to be in KES (Kenyan Shillings).

OrderID: Treated as a unique identifier for each transaction.

Missing Values Handling:

City- filled as "Unknown"

Channel- filled as "Unknown Channel"

Salesperson- filled as "Unassigned"

### 3. New Columns Introduced

IsCorrectUnitPrice

Purpose: To flag suspicious unit prices.

Method: Calculated using a custom function that checks for anomalies in the UnitPrice column.

Clean Required Date

Purpose: Standardized and cleaned the RequiredDate column for further analysis.
