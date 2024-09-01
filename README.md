# S-and-P-500_Stock-Market
# 📊 S&P 500 Analysis Project

## Introduction

The S&P 500, or Standard & Poor's 500, is a stock market index tracking the performance of 500 large companies listed on stock exchanges in the United States. This project aims to analyze various aspects of the S&P 500 index, including stock performance, sector analysis, and employment statistics.

## 📂 Datasets

We utilized three datasets for this analysis:
1. **Stocks**: Contains historical stock data for 503 companies.
   - Columns: `date`, `symbol`, `adjclose`, `high`, `low`, `open`, `volume`
   - Rows: 1,830,417
2. **Index**: Contains historical data of the S&P 500 index.
   - Columns: `date`, `S&P500`
   - Rows: 2,517
3. **Companies**: Contains detailed information about the companies listed in the S&P 500.
   - Columns: `exchange`, `symbol`, `shortname`, `longname`, `sector`, `industry`, `currentprice`, `marketcap`, `ebitda`, `revenuegrowth`, `city`, `state`, `country`, `fulltimeemployees`, `longbusinesssummary`, `weight`
   - Rows: 503

## 🎯 Objectives

The objectives of this project include:
- Calculating the Compound Annual Growth Rate (CAGR) of the S&P 500 index and individual companies.
- Identifying companies that outperform the S&P 500 index.
- Highlighting the best investment options based on historical performance.
- Analyzing sectors and industries for growth.
- Determining companies with the highest employment.
- Assessing the market cap and revenue growth of the companies.
- Examining the geographic distribution of companies.

## 🛠️ Methodology

### Data Import

Datasets were imported from Kaggle using the Kaggle library in Python.

### Data Cleaning

#### Handling Null Values

1. **Stocks Dataset**: Removed null values for companies listed after the start date of 2010-01-04.
2. **Companies Dataset**:
   - `Revenuegrowth`: Calculated missing values using the mean percentage change of the `adjclose` column.
   - `Ebitda`: Imputed 29 null values using the median from the financial services sector.
   - `State`: Manually filled 19 null values based on the corresponding city.
   - `Fulltimeemployees`: Filled 4 null values using data from reliable sources.

### Data Visualization

Uploaded the data to Excel using Power Query and made necessary changes. Created pivot tables and visualizations for the index, stocks, and companies. This helped in deriving insights from the visualized data.

### Analysis Steps

1. Calculated the CAGR of the S&P 500 index and individual companies.
2. Filtered stocks listed for more than 10 years.
3. Analyzed sectors and industries for growth.
4. Identified the best investment options based on historical CAGR.
5. Conducted detailed analyses of Tesla, NVIDIA, and Broadcom Inc.
6. Visualized the data in Excel to identify trends and insights.

## 🔍 Observations

### Index Observations

- The CAGR of the S&P 500 index is 10.8%.
- **2021**: Best year with a 1010-point increase.
- **2022**: Significant drop of 922 points.
- **2023**: Market recovered with a 930-point increase.
- **March 2020**: 19% downfall due to the pandemic.
- **June 2020**: 6.3% return as the market recovered.

### Stock Observations

- 469 stocks were listed for more than 10 years.
- **Top Performers**: NVIDIA (49% CAGR), Tesla (40% CAGR), Broadcom Inc. (40% CAGR).
- **Highly Volatile Stock**: Tesla showed significant fluctuations in recent years.

### Companies Analysis

- **Best Performing Sectors**: Based on average CAGR.
- **Max Employment**: Walmart, Amazon, and Accenture are the top employers.
- **Market Cap**: NVIDIA, Microsoft, and Apple have the highest market caps.
- **Revenue Growth**: NVIDIA, Super Micro Computer, and Blackstone lead in revenue growth.
- **Geographic Distribution**: Analyzed companies listed in the S&P 500 by country.
- **Most Expensive Stock**: NVR, Inc.

## 📈 Insights

- The S&P 500 index has shown consistent growth with an average CAGR of 10.8%.
- **Top Investment Options**: NVIDIA and Broadcom Inc. are recommended based on historical performance.
- **Highest Growing Industries**: Rental & Leasing Services, Trucking, Consumer Electronics. Best options with multiple companies include Software - Application and Semiconductor.
- **Top Employers**: Walmart, Amazon, and Accenture.
- **Top Market Cap Companies**: NVIDIA, Microsoft, and Apple.
- **Top Revenue Growth**: NVIDIA, Super Micro Computer, and Blackstone.

## 🚀 Conclusion

This project provides a thorough analysis of the S&P 500 index and the companies within it, offering valuable insights for investment decisions. By understanding growth patterns, sector performance, and employment statistics, more informed choices can be made in the stock market.
