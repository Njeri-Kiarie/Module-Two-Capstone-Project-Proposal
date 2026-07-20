# Module-Two-Capstone-Project-Proposal

# Kenya Flood Humanitarian Response Dashboard

## Project Overview
During heavy rainfall seasons, Kenya experiences severe localized flooding that displaces thousands of families. Efficient crisis response requires disaster response agencies to quickly see where human displacement intersects with insufficient relief funds. This project builds a disaster response dashboard by pulling raw disaster data using **Power Query** and build a budget planning tool in **Excel** and create an interactive visual map in **Tableau** to help leaders send aid where it is needed most.

## Problem Statement
When Flood disasters strike, humanitarian organizations struggle with fragmented data. Disaster management agencies frequently log displacement numbers, damage metrics and financial aid disbursments across non-related files. Without a centralized and data-driven framework:
* **Misallocation occurs:** Some heavily impacted counties may suffer from resource shortages while other regions recieve funding in surplus.
* **Slow Response Time:** Decision makers cannot easily see which highly flooded areas are running out of money.
* **Hidden Costs:** Government and non+profit stakeholders lack an automated system to forecast the exact budget needed to support displaced families based on new field reports.

## Key Research Questions
To provide actionable insights for disaster response teams, this project answers the following core questions:
1. **Geospatial Risk:** Which counties in Kenya exhibit the highest priority emergency levels based on human displacement and Structural damage?
2. **Aid Equity:** What is the current aid-per-capita (fund per displaced person) distribution across affected regions and where do the sharpest resource disparities exist?
3. **Financial Liabilities:** What is the exact monetory funding gap(deficit or surplus) per county to buy basic emergency supply kits for families?
4. **Smart Reallocation of funds:** How can we use a dashboard to quickly identify areas with extra money and move those resources to underfunded hotspots?

## Data Source.
* https://data.humdata.org/group/ken

## Methodology
The project follows the following steps to process the data:
* **Phase One:** Data Gathering and Cleaning (Excel Power Query)
i. Download the raw, official flood tracking data in csv from reliable data source.
ii. Open the data in Excel using Power Query.
iii. Clean the data - Remove unnecessary columns, filter rows to only show Kenyan counties, fix any mispelled county names and replace empty or blanks with '0'.
* **Phase Two:** Budget Modeling and Gap Analysis (Excel Formulas)
Use standard Excel formulas to calculate metrics and risk categories like:
i. Required Emergency Budget.
ii. Funding shortage or deficit.
iii. Resource status labelling using 'IF' to categorize funding as either 'Underfunded' or 'Fully Funded/Surplus'.
iv. Priority level label: Labelling dispaced persons as either 'CRITICAL (Priority 1)', 'SEVERE (Priority 2)' or 'STABLE (Priority 3)'.

* **Phase Three:** Spatial Visual Analytics (Tableau)
i. Connect Tableau directly to the finalized, clean Excel workbook.
ii. Build KPI cards (Total Displaced, Total Shortages).
iii. Create an interactive Filled map of Kenya to color code the counties based on priority levels.
iv. Build Bar chart to show counties with the biggest money shortages.
v. Enable dashboard interactivity whereby clicking on a specific county instantly filters the KPI metrics and resource charts across the entire dashboard.
