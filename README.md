# Ridership Intelligence Portal - Excel Dashboard

This repository contains the source files and documentation for the "Ridership Intelligence Portal," an interactive dashboard built entirely in Microsoft Excel to analyze public transportation data.



## Key Insights & Features

This dashboard provides a comprehensive overview of the transit system's performance, highlighting several key findings:

*   **Fleet Utilization Analysis:** A significant operational imbalance was identified: while **24%** of buses are **Over Utilized** (risking poor passenger experience), **22%** are **Under Utilized** (impacting cost efficiency).
*   **Peak Time Identification:** The analysis pinpointed the **9:00 AM - 12:00 PM** window as the busiest 3-hour block, challenging traditional assumptions about peak travel times.
*   **Weekly Ridership Patterns:** Sunday, Monday, and Tuesday are powerhouse days, accounting for nearly half (**49.4%**) of all weekly passengers. This insight is crucial for resource and staff scheduling.
*   **AM/PM Split:** The data clearly shows that **64.6%** of all riders travel in the PM, indicating a strong demand for evening and night services.
*   **Interactive Slicers:** The dashboard includes slicers for dynamic filtering by route, rider demographics, and date, allowing for deeper, user-driven analysis.

## Tech Stack

*   **Microsoft Excel:** The primary tool for dashboard creation and visualization.
*   **Power Query (Get & Transform Data):** Used for the ETL (Extract, Transform, Load) process to clean, shape, and load the raw CSV data.
*   **Power Pivot:** Used to create a relational data model, connecting the different data sources.
*   **DAX (Data Analysis Expressions):** Used to write formulas and create calculated measures for advanced KPIs like utilization categories and revenue calculations.



## Data Source

The analysis is based on four separate CSV files.

*   `Facttable_ridership.csv`: The main fact table containing transactional ridership records, including `BusID`, `Date`, `Time`, and `NumberOfRiders`.
*   `Dim_buses.csv`: A dimension table with details for each bus, including `BusID` and `Capacity`.
*   `Dim_routes.csv`: A dimension table containing information about each route, such as `RouteName`, `TripFee`, and locations.
*   `Dim_demographics.csv`: A dimension table with anonymized demographic data for each rider, including `RiderID`, `Age`, and `Occupation`.

