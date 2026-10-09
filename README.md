# Real Estate Data Analysis

## Project Overview

This project analyzes real estate listing and sold transaction data from CRMLS, the California Regional Multiple Listing Service. The goal is to clean, aggregate, and analyze MLS data to better understand housing market trends, property sales activity, pricing behavior, and market performance across different locations and property types.

The project uses Python and Pandas for data aggregation, cleaning, validation, and exploratory data analysis. The final cleaned datasets can be used for further analysis, reporting, and dashboard development.

## Objectives

The main objectives of this project are to:

- Combine monthly MLS listing and sold transaction files into two unified datasets from January 2024 to May 2026, filtering residential properties

- Prepare analysis-ready datasets and improve data quality by handling missing values, duplicate records, invalid dates, inconsistent values, and potential outliers.

- Analyze completed sales transactions to understand California housing market trends in sales volume, home prices, price per square foot, Days on Market (DOM), and sale-to-list price ratios.

- Evaluate geographic market differences by comparing pricing, market speed, and competitiveness across California counties.

- Examine property characteristics such as property subtype, bedrooms, property age, and living area to determine how they are associated with price and market performance.

- Analyze current housing inventory using listing data, with an emphasis on Active listings, to understand asking prices, inventory levels, and how long properties remain on the market.

- Explore external market factors, including mortgage rates, and their relationship with transaction volume and market speed.

- Develop interactive Tableau dashboards that summarize key market trends and allow users to compare housing market conditions across time, location, and property characteristics.


## Data Source
The dataset originates from CRMLS, the California Regional Multiple Listing Service. CRMLS is one of the largest MLS systems in the United States and covers much of Southern California.

A Multiple Listing Service, or MLS, is a private cooperative database operated by a regional association of real estate brokers. Real estate agents use the MLS to share listing information with one another. It works like a centralized marketplace for properties. There is no single national MLS; instead, each region has its own MLS system, such as CRMLS in Southern California, NWMLS in the Pacific Northwest, and MRED in the Chicago area.

Consumer-facing platforms such as Zillow and Redfin often receive listing information from MLS feeds through licensed agreements. This means that many public real estate listings originally come from MLS data. Working directly with CRMLS data provides access to information closer to the original source.

**Metadata**: https://trestle-documentation.corelogic.com/metadata/resources/Property/ 


## Listings vs. Sold Data

This project keeps listing data and sold data separate because they represent different parts of the real estate market.

The listings dataset includes properties that were listed on the market, regardless of final outcome. These records may include active, pending, expired, withdrawn, or closed listings. This dataset is useful for analyzing market supply and listing activity.

The sold dataset includes only properties that completed a transaction. These records contain final sale information such as ClosePrice and CloseDate. This dataset is useful for analyzing price trends, sales volume, and closed transaction behavior.


## Important Notes

The row counts may vary slightly depending on when the data was pulled from the MLS API because MLS data is continuously updated. Small differences in row counts are expected as long as the extraction process is working correctly and the results are reasonably consistent.

Some monthly files may contain slightly different columns. During aggregation, inconsistent metadata columns are reviewed and standardized before final analysis.
