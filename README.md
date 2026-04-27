# Amazon vs eBay: Financial Performance and Stock Return Comparison

**Author:** Your Name  
**Student ID:** Your ID
**Module:** ACC102

## 1. Problem & User
This project compares Amazon and eBay using accounting data and stock return data. The aim is to examine differences in firm size, profitability, and annual stock return, and to explore whether higher ROA is associated with stronger stock performance.

The main users are business students, beginner investors, and anyone interested in a simple firm-level comparison using WRDS data.

## 2. Data
The data comes from **WRDS** and includes:
- **Compustat Fundamentals Annual** for accounting data
- **CRSP Monthly Stock File** for stock returns
- **CCM Link Table** for matching Compustat and CRSP identifiers

Main variables used:
- `sale`(sales)
- `at`(total assets)
- `ni` (net income)
- `ret` (monthly stock return)

Constructed variables:
- `roa = ni / at`
- `annual_return` from compounded monthly returns

Sample firms:
- Amazon (AMZN)
- eBay (EBAY)

Access date:
- [Replace with actual access date]

## 3. Methods
The analysis follows these steps:
1. Download accounting and stock return data from WRDS
2. Match Compustat and CRSP data using the CCM link table
3. Clean the data and keep valid observations
4. Calculate ROA and annual stock return
5. Compare the two firms using summary statistics and visualizations
6. Examine the relationship between ROA and annual return using correlation and regression

## 4. Key Findings
- Amazon is larger than eBay in terms of sales and assets
- The two firms show different profitability patterns
- Their annual stock return performance also differs over time
- ROA appears related to stock return, but the relationship is not fully explained by accounting data alone

## 5. How to Run
1. Clone this repository
2. Install required packages:
   ```bash
   pip install -r requirements.txt
