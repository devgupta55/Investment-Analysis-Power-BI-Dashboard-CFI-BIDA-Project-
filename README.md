# Investment-Analysis-Power-BI-Dashboard-CFI-BIDA-Project

## 📌 Overview

This project is a Power BI dashboard developed as part of the Business Intelligence & Data Analyst (BIDA) certification program at the Corporate Finance Institute (CFI). It simulates the role of a Business Intelligence Analyst at an investment bank. The dashboard is designed to provide the sales and trading team at CFI Capital Partners with customized market analysis, offering insights into investment portfolios, securities, and exchange data.

## 🎯 Objectives

The primary objectives of this project include:

-   Connecting to and integrating data from multiple sources.
-   Transforming and modeling data for effective analysis.
-   Creating DAX measures to derive key performance indicators (KPIs).
-   Developing interactive and visually appealing report visuals in Power BI.
-   Providing bespoke market analysis to support the sales and trading team.

## 🗂️ Data Sources

The dashboard utilizes data from the following sources:

-   **factActivity:** This table contains activity data for various securities, including `Close`, `Date`, `Price Change`, `Price Range`, `Security_ID`, and `Volume`. The data was consolidated from multiple Excel files, each representing a year of activity (2015-2021).
-   **dimSecurity:** Contains information about the securities, including `Address`, `City`, `Company`, `Country`, `Exchange_ID`, `Industry`, `Security_ID`, `State`, `Ticker Symbol`, and `Weighting`.
-   **dimExchange:** Contains details about the exchanges, such as `Currency`, `Exchange_ID`, `Exchange_Symbol`, `Location`, `Type`, and `Website`.
-   **dimDate:** A date dimension table used for time-based analysis, containing fields like `Date`, `Day`, `Month`, `Month Name`, and `Year`.

***Note: Due to confidentiality reasons, the actual datasets cannot be included in this repository. Screenshots of the data structure are provided below.***

### Data Model

The data model is structured as a star schema, with `factActivity` as the central fact table linked to the dimension tables (`dimDate`, `dimSecurity`, and `dimExchange`). The relationships are one-to-many from the dimension tables to the fact table.<br>
<img src="https://github.com/user-attachments/assets/a2cbd465-d4c3-420f-ae16-eab8edfb2385" width="600">

### Overview of Datasets
<img src="https://github.com/user-attachments/assets/9fe45a25-9a5d-4e79-aae7-5be0ebfd8875" width="600"> 
<img src="https://github.com/user-attachments/assets/d60550d2-88f0-49de-b1cc-0b690746eaba" width="600">


## Tables
**factActivity:**  This table was created by combining data from multiple excel files from 2015 to 2021.<br>
<img src="https://github.com/user-attachments/assets/6e9f1bd7-9c81-42fd-8221-67787f245b69" width="600">

**dimSecurity:**<br>
<img src="https://github.com/user-attachments/assets/773b0959-910c-4d92-af88-02184fb8ea93" width="600">

**dimExchange:**<br>
<img src="https://github.com/user-attachments/assets/df6f19c4-7fb2-4d5d-a4b0-1c02baf39e4e" width="600">

**dimDate:**<br>
<img src="https://github.com/user-attachments/assets/f7fd4d9e-0f52-4a95-878e-2f3f410477f6" width="600">

## ⚙️ Data Transformation and Modeling

-   **Data Consolidation:** The `factActivity` table was created by combining multiple Excel files (2015 Activity.xlsx to 2021 Activity.xlsx), ensuring data consistency and accuracy.
-   **Relationships:** Relationships were established between the fact and dimension tables to facilitate data slicing and dicing.
-   **DAX Measures:** Custom DAX measures were created to calculate key metrics such as Average Daily Volume, Total Portfolio Value, and Price Change.

## <img src="https://github.com/microsoft/PowerBI-Icons/blob/main/SVG/Power-BI.svg" width="24" style="margin-bottom: -10 px"> Power BI Dashboard

The dashboard consists of multiple interactive visuals to provide a comprehensive view of the market data. Key components include:

-   **KPI Cards:** Display key volume metrics including Average Daily Volume (400.89M), Min Daily Volume (124M), Max Daily Volume (1bn), YTD Average Daily Volume (378.51M), YTD Max Daily Volume (859M), and YTD Min Daily Volume (252M).

-   **Total Volume Trend Chart:** A line chart visualizing the total trading volume by date, broken down by exchange (NASDAQ and NYSE) from 2015 to 2021.

-   **Security Count by Exchange:** A bar chart showing the distribution of securities listed on each exchange (NYSE and NASDAQ).

-   **Geographic Heatmap:** A map displaying the distribution of exchanges across different locations (using Pincode and Exchange\_Symbol).

-   **Average Price Range and Change Analysis:** A scatter plot showing the average price range and average price change by company and year (2015-2021).

-   **Total Close Price Trends:** A line chart visualizing the trends in total close price for various ticker symbols over time (2015-2021).

-   **Portfolio Value Over Time:** A streamgraph illustrating the total portfolio value by year and ticker symbol, providing insights into the changing composition of the portfolio.

-   **Security Performance Table:** A table displaying the current price, weighting, and current portfolio value for each ticker symbol.

### Security and Portfolio
<img src="https://github.com/user-attachments/assets/6190458f-3b56-49b0-95ea-45e8b4236eb9" width="600">

### Exchange
<img src="https://github.com/user-attachments/assets/6c0c5c57-0518-4664-8b99-03def6e0135e" width="600">

## 📈 Key Insights

The dashboard provides insights into:

-   Trading volumes by exchange and date.
-   Geographical distribution of trading activity.
-   Performance of individual securities and their contribution to the overall portfolio value.
-   Trends in price changes and trading volumes over time.

## ✅ Conclusion

This Power BI dashboard provides a robust tool for market analysis, enabling the sales and trading team at CFI Capital Partners to make informed decisions based on comprehensive data insights. The project demonstrates the effective use of Power BI for data integration, modeling, and visualization in a financial context, as part of the BIDA certification program at CFI.

