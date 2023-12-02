# prophet-challenge
# MercadoLibre Analysis Readme

## Introduction
This project investigates the Google search traffic for MercadoLibre and attempts to correlate it with various financial events within the company. Additionally, it explores seasonality in search data, the relationship between search traffic and stock price patterns, and constructs a time series forecasting model using Prophet.

## Steps and Findings

### Step 1: Unusual Patterns in Search Traffic
- We ingested Google search traffic data into a DataFrame, focusing on May 2020, when MercadoLibre released its financial results.
- Visualization indicated unusual patterns corresponding to the financial announcement.
- Total search traffic for May was higher than the median for all months, suggesting increased interest during the financial release.

### Step 2: Seasonal Search Traffic Patterns
- Hourly search data were grouped and visualized, showing peak traffic late in the evening before midnight.
- Weekly trends peaked on Sundays, with the lowest activity on Fridays.
- Yearly analysis revealed the lowest search traffic just after New Year's Day.
- These findings can assist marketing efforts in optimizing ROI.

### Step 3: Search Traffic vs. Stock Price
- Stock price data were plotted and combined with search data, showing a trend consistent with the increased revenue narrative for e-commerce platforms post the early 2020 market shock.
- Analysis of the first half of 2020 showed both time series rising post-March.
- A new DataFrame column, "Lagged Search Trends," showed a weak negative correlation with stock volatility and a weak positive correlation with hourly stock returns, indicating no strong predictable relationship.

### Step 4: Time Series Model with Prophet
- The search data was modeled using Prophet, providing a near-term forecast that suggested a return to typical search levels following a significant spike.
- The time series components indicated:
  - The most popular time of day: late evening before midnight.
  - The busiest day of the week: Sunday.
  - The lowest point for search traffic in the year: just after January 1st.

## Conclusions
The data analysis suggests a correlation between search traffic and significant financial events, such as earnings releases. Seasonal patterns in search behavior were identified, which could inform targeted marketing strategies. While a weak relationship was observed between search traffic and stock volatility and returns, it was not strong enough to serve as a reliable predictive tool. The time series model projected a reversion to typical search interest levels after a peak, which can be crucial for strategic planning.

## Instructions for Replication
- Install required libraries, including pandas, matplotlib, and Prophet.
- Read and preprocess the data as detailed in the steps.
- Use provided code snippets for analysis and model creation.
- Refer to the questions and hints for detailed analysis and interpretation of results.

## Requirements Checklist
- [x] Read search data and slice for May 2020.
- [x] Calculate and compare total search traffic.
- [x] Group and visualize search data for different timeframes.
- [x] Correlate search traffic with stock price patterns.
- [x] Create and interpret a time series model with Prophet.

