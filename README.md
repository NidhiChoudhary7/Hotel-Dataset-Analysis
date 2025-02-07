# Analyze Hotel Dataset Project

## Overview
This project focuses on analyzing hotel booking data to derive meaningful business insights and recommendations. It covers a complete data science pipeline from business understanding, exploratory data analysis (EDA), data cleaning, modeling, and visualization using Azure and Power BI.

---

## Table of Contents
1. [Objective](#objective)
2. [Business and Problem Understanding](#business-and-problem-understanding)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Data Cleaning and Modeling](#data-cleaning-and-modeling)
5. [Data Orchestration and Azure Pipeline](#data-orchestration-and-azure-pipeline)
6. [Visualization and Insights](#visualization-and-insights)
7. [Conclusion](#conclusion)
8. [Recommendations](#recommendations)

---

## Objective
To derive business insights from hotel booking data and compare the performance of City Hotel and Resort Hotel year-over-year on various Key Performance Indicators (KPIs). This project supports better customer profiling, informed decision-making, and actionable recommendations.

---

## Business and Problem Understanding
### Problem Statement
Analyze guest profiles from the hotel's perspective to understand:
- Booking patterns and channels
- Occupancy trends by market segment, nationality, and stay duration
- Cancellation behaviors
- Room pricing trends across time periods and room types

---

## Exploratory Data Analysis (EDA)
Initial investigation was performed to discover patterns, anomalies, and validate assumptions. Key variables explored include:
- Arrival dates, room types, and average daily rates
- Number of guests by nationality
- Cancellation rates and booking channels

Observations:
- No primary key in the data led to duplicate entries.
- Cancellation booking filters were essential to assess true customer engagement.
- 2% of guests had free or negative stays, potentially due to logging errors.

---

## Data Cleaning and Modeling
**Key Cleaning Steps:**
- Handling undefined country values (488 occurrences)
- Removing true duplicates due to the lack of a unique identifier
- Correcting anomalies in average daily rates

**Modeling Approach:**  
Data cleaning and modeling were orchestrated using Azure services for efficient handling and Power BI for visualization.

---

## Data Orchestration and Azure Pipeline
**Key Components:**
- **Azure Blob Storage:** Stores the raw CSV file containing hotel data.
- **Azure Data Factory:** Pipelines created to copy and transform data from Blob Storage to Azure SQL Database.
- **Azure SQL Database:** The destination for cleaned and processed data.
- **Power BI Dashboard:** Used to visualize and analyze key business metrics.

**Linked Services:** Connected Azure Blob and SQL Database for data flow automation.

---

## Visualization and Insights
### Key Findings:
- **Nationality Distribution:** Most guests come from Portugal, UK, France, Spain, and Germany.
- **Room Pricing Trends:** Room prices peak during the summer (July-August) and dip in winter.
- **Stay Duration:** Most guests stay for 1-3 days, with Resort Hotel guests staying longer than City Hotel guests on average.
- **Booking Channels:** The majority of bookings are done via online travel agents (OTAs).
- **Cancellations:** Room type A has over 35% cancellation rates, significantly higher than other types.

### Visualizations:
- Filtered dashboards by hotels, time periods, and room types
- Charts on cancellation rates, average room prices, and stay durations

---

## Conclusion
- The average room price peaks in July-August due to high seasonal demand.
- Room type A experiences the highest cancellation rates.
- Most guests prefer short stays (1-3 days).
- Online travel agents dominate booking channels, but direct bookings are relatively low.

---

## Recommendations
1. **Cancellation Management:** Investigate reasons for high cancellations in Room type A using CSAT scores.
2. **Incentivize Longer Stays:** Provide offers to City Hotel guests staying longer than 2 days.
3. **Promote Direct Bookings:** Launch loyalty programs to reduce dependency on third-party channels.
4. **Seasonal Hiring:** Prepare for high demand during the summer by hiring temporary staff.

---

## Dashboard Overview
A Power BI dashboard provides comprehensive insights into:
- Booking trends
- Room prices and cancellations
- Customer segmentation by nationality, stay duration, and booking channel

**Thank You!**  
This project aims to provide actionable insights for enhancing operational efficiency, optimizing pricing strategies, and improving customer experience.
