# The Impact of Inflation on GDP and Unemployment Rates

A data analysis project exploring the relationship between inflation, GDP growth, and unemployment rates across the world, Africa, and Egypt, using historical data from 1960 to 2024.

## 📊 Project Overview
This project analyzes how changes in inflation influence economic growth and employment levels over more than six decades of global data. The analysis moves through three levels of depth — **Global**, **Africa**, and **Egypt** — combining SQL, statistical testing, web scraping, and visualization to uncover patterns in how these three economic indicators move together.

## 📁 Data Sources
- **Inflation Dataset** — Annual inflation rates for all countries (1960–2024), including average inflation and inflation level classification
- **GDP Dataset** — Annual GDP growth rates and GDP levels by country (1960–2024)
- **Unemployment Dataset** — Unemployment rates by country, sex, and age category (1960–2024)
- **Additional Data**:
  - Historical USD/EGP exchange rates (scraped from financial websites)
  - Egypt's imports and exports over time (World Bank / financial reports)
  - African population, birth rate, and death rate data (scraped from Wikipedia)

## 🔍 Methodology
1. **Data Cleaning & Preprocessing** — Handled missing values (scikit-learn), reshaped yearly columns into a time-series format, merged datasets on country and year
2. **Feature Engineering** — Added derived columns (e.g., average inflation, inflation level classification)
3. **Database Creation** — Loaded cleaned tables into a SQLite database and queried with SQL (`ipython-sql`)
4. **Exploratory Data Analysis** — Distribution and comparison of indicators across countries and continents
5. **Statistical Testing** — Correlation and chi-square tests to examine relationships between inflation, GDP, and unemployment
6. **Regional Deep-Dives** — Focused analysis on Africa and Egypt specifically, including currency and trade data
7. **Web Scraping** — Pulled supplementary population and economic data from Wikipedia using BeautifulSoup

## 🌍 Analysis Structure
- **Global Analysis** — Worldwide trends in inflation, GDP, and unemployment (1960–2024), top/bottom 10 country comparisons, outlier-adjusted trends
- **Africa Analysis** — Regional inflation/GDP/unemployment trends, population vs. world population projections, birth rate vs. inflation
- **Egypt Analysis** — EGP/USD exchange rate vs. inflation, imports vs. exports vs. inflation, unemployment by gender, GDP over time

## 📈 Key Findings
- A **moderate correlation** exists between inflation, GDP, and unemployment at the global level, though country-specific dynamics matter
- **Venezuela** recorded the highest inflation in the dataset's history
- Global GDP growth trended upward overall, with a notable dip in **2019**
- **Unemployment is consistently highest among women**, both globally and in Africa/Egypt specifically
- Egypt shows a **strong relationship** between the Egyptian pound's value and inflation
- Egypt's **imports consistently exceed exports** across the analyzed period

## 🛠️ Built With
- **Python** — pandas, numpy, matplotlib, seaborn
- **SQL** — SQLite, ipython-sql
- **Statistics** — scipy (correlation, chi-square testing)
- **Web Scraping** — BeautifulSoup, requests
- **Machine Learning utilities** — scikit-learn (missing value imputation)
- **Additional APIs** — yfinance, pandas-datareader (World Bank data)
- **Geospatial** — geopandas

## 📌 Notes
This was completed as a graduation project, using publicly available economic datasets for educational and portfolio purposes.

---
**Author:** Ahmed Essam Ahmed  
Financial, Cost & Data Analyst | Python, SQL & Data Analytics
