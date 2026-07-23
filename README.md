# Module-Two-Capstone-Project-Proposal

# Kenya Drought Humanitarian Response Dashboard

## Project Overview
Kenya experiences recurring droughts that affect the Arid and Semi-Arid Lands(ASALs) leading to food insecurity, water shortages, livestock losses and increased humanitarian needs. Effective response requires humanitarian organizations and government agencies to quickly identify counties with the greatest need and allocate limited resources efficienttly. This project builds a drought humanitarian response dashboard by integrating publicly available county-level drought impact data using **Excel Power Query**, build a budget planning and funding gap analysis in **Excel** and create an interactive dashboard in **Tableau** to support evidence-based resource allocation across drought-affected counties.

## Problem Statement
Recurring droughts remain one of Kenya's most significant and devastating natural disasters. Although organizations such as the National Drought Management Authority (NDMA) and humanitarian agencies regularly publish drought monitoring reports, the information is often spread across multiple datasets and reports, making it difficult to obtain a comprehensive overview of drought severity and humanitarian needs. Without a centralized and data-driven framework:
* **Insufficient Resource Allocation occurs:** Counties experiencing the highest levels of drought may not receive resources proportional to their needs.
* **Delayed decision making:** Humanitarian agencies face challenges in quickly identifying priority counties that require urgent intervention.
* **Limited Financial Planning:** Government and non-profit stakeholders lack an automated system to forecast an estimate budget needed to provide emergency food assistance and identify deficits or surpluses.
* **Fragmented Data:** A significant amount of time is taken by decision-makers in consolidating information from multiple sources before being able to plan interventions.

## Key Research Questions
To support humanitarian planning and resource allocation, this project seeks to answer the following core questions:
1. **Geographical Vulnerability:** Which counties in Kenya exhibit the highest levels of drought severity?
2. **Humanitarian Need:** Which counties have the largest populations affected by drought and require urgent humanitarian intervention?
3. **Budget Planning:** What is the estimated humanitarian response budget required to support drought-affected populations for each affected county?
4. **Funding Gap Analysis:** Which counties face the largest estimated funding deficits based on projected humanitarian needs?
5. How can an interactive dashboard support resource allocation and humanitarian planning during drought emergencies?

## Data Sources.
The project utilizes publicly available count-level datasets from the following sources:
* Integrated Food Security Phase Classification(IPC) - County-level data on populations requiring humanitarian assistance (IPC Phase 3 and above).
https://www.ipcinfo.org/ipc-country-analysis/en/?country=KEN

## Methodology
The project follows the following steps to process the data:
* **Phase One:** Data Gathering and Cleaning (Excel Power Query)
  * Download county-level drought and humanitarian datasets from official   sources.
  * Open the data in Excel using Power Query.
  * Clean the data - Remove unnecessary columns, Standardize county names, Handle Missing values, Correcting data types.
    
* **Phase Two:** Budget Modeling and Gap Analysis (Excel Formulas).
Use standard Excel formulas to calculate metrics like:
  * Estimated households affected by drought.
  * Estimated humanitarian response budget.
  * Estimated funding gap (deficit or surplus).
  * Budget coverage percentage.
  * Funding status using IF statements to classify counties as Underfunded or Adequately Funded.
  * Priority level using IF statements to classify counties as Critical (Priority 1), High (Priority 2) or Moderate (Priority 3) based on drought severity and proportion of the population requiring humanitarian assistance (IPC Phase 3 and above).

* **Phase Three:** Interactive Spatial Analytics (Tableau)
  * Connect Tableau directly to the finalized, clean Excel workbook.
  * Build KPI cards (Total Population Analyzed, Total Population Requiring Humanitarian Assistance, Total Estimated Affected Households, Total Estimated Humanitarian Response Budget Required, Total Funding Received, Total Estimated Funding Gap, Number of critical and High Priority Counties).
  * Create an interactive Filled map of Kenya to color code the counties based on humanitarian priority levels based on drought-related impacts.
  * Build Bar chart to rank counties by estimated affected population and Financial Gap chart to compare the estimated humanitarian response budget against available funding to identify counties with the largest funding deficits .* Enable dashboard interactivity whereby clicking on a specific county instantly updates the KPI metrics and Visualizations and Include filters for county, humanitarian priority level, and funding status to facilitate interactive analysis.
