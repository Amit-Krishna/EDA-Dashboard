# Accident Data Analysis (NYC Motor Vehicle Collisions)

## Project Overview

This project performs Exploratory Data Analysis (EDA) on motor vehicle collision data from New York City using Microsoft Excel. The primary goal is to derive actionable insights from historical crash data, identify key patterns, risk factors, and create an interactive dashboard using Excel's Pivot Table and Pivot Chart features to aid in safety analysis and decision-making.

## Project Details

*   **Project Name:** Accident Data Analysis
*   **Project Period:** January - April 2025 (Project Semester)
*   **Submitted By:** Amit Krishna
    *   Registration No: 12326830
*   **Program & Section:** B-Tech, KM005
*   **Course Code:** INT 217
*   **Under the Guidance of:** Ms. Baljinder Kaur (ID: 27952)
*   **Institution:** Lovely School of Computer Science and Engineering, Lovely Professional University, Phagwara

## Data Source

The dataset analyzed is sourced from the NYC Open Data portal and contains detailed records of motor vehicle collisions reported by the New York Police Department (NYPD).

*   **Source:** NYC Open Data Portal
*   **Dataset Link:** [Motor Vehicle Collisions - Crashes](https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes)

The dataset includes fields such as crash date, time, location details, number of persons and pedestrians injured or killed, contributing factors, and vehicle types involved.

## Data Preparation & Preprocessing

The raw dataset underwent the following preprocessing steps in Excel:

1.  **Missing Values:**
    *   Numeric missing values were filled using the mean of the respective column.
    *   Categorical missing values were filled using the mode of the respective column.
    *   No rows were deleted during this process.
2.  **Date Formatting:** The `CRASH DATE` column was formatted appropriately using Excel functions.
3.  **Feature Engineering (New Columns Created):**
    *   `CRASH_YEAR_MONTH`: Extracted from `CRASH DATE`.
    *   `CRASH_HOUR`: Extracted from `CRASH TIME`.
    *   `TOTAL_INJURED`: Sum of `PERSONS INJURED` and `PEDESTRIANS INJURED`.
    *   `TOTAL_KILLED`: Sum of `PERSONS KILLED` and `PEDESTRIANS KILLED`.
    *   `CRASH_SEVERITY`: Categorical label ("Severe" if `TOTAL_INJURED` > 0 or `TOTAL_KILLED` > 0, otherwise "Non-Severe").
    *   `DAY_TYPE`: Categorical label ("Weekday" or "Weekend") based on the `CRASH DATE`.
    *   `MONTHS`: Abbreviated month name extracted from `CRASH DATE`.

## Analysis & Key Findings

The analysis aimed to answer specific questions about the accident data using Excel Pivot Tables and Pivot Charts. Key findings include:

*   **Accident Severity:** Approximately two-thirds of the analyzed accidents were classified as "Non-Severe".
*   **High-Risk Locations:** Belt Parkway was identified as a location with a notably high frequency of crashes.
*   **Contributing Factors:** "Distraction" was the most frequently cited contributing factor in accidents.
*   **Vehicle Involvement:** Sedans and Station Wagons were the vehicle types most commonly involved in collisions.
*   **Casualty & Fatality Rates Over Time:** The analysis revealed seasonal trends and specific periods with spikes in total injuries and fatalities, such as peaks observed around March-May and an increasing trend towards year-end (Nov-Dec).
*   **Factor-Severity Correlation:** While 'Distraction' is the most frequent cause, factors like 'Failure to Yield Right-of-Way' showed a higher proportion of severe outcomes relative to their frequency compared to 'Distraction'.
*   **Weekday vs. Weekend Trends:** More accidents, injuries, and fatalities were recorded during weekdays compared to weekends.

Visualizations used to present these findings include Donut Pie Charts, Pie Charts, Bar Charts, Column Charts, Combo Line Charts, Stacked Column Charts, and Clustered Column Charts, all created within Excel.

## Technology

*   Microsoft Excel (for Data Preprocessing, Analysis, Pivot Tables, Pivot Charts, and Dashboard Creation)

## Dashboard / Analysis Showcase

An interactive dashboard was created in Excel to allow dynamic filtering and exploration of the analysis findings.

*   **Link to Showcase:** [https://tinyurl.com/DashBoardEDA](https://tinyurl.com/DashBoardEDA)
    *(Note: This link likely leads to a presentation, video, or post showcasing the dashboard and analysis results.)*

## Conclusion

The project successfully performed EDA on NYC crash data using Excel, identifying significant risk factors such as specific locations, contributing factors (like distraction), involved vehicle types, and temporal patterns. The creation of an interactive dashboard enhances the ability to explore these insights dynamically.

## Future Scope

Potential extensions and improvements for this project include:

1.  **Clustering Analysis:** Applying clustering techniques to group geographically proximate areas based on risk profiles (frequency, severity, factors) to better identify high-risk zones algorithmically.
2.  **Real-time Data Integration:** Developing a system or utilizing tools that can integrate real-time or near-real-time crash data for up-to-date analysis and potential alerting on emerging hotspots.
3.  **Advanced Visualization Tools:** Migrating the analysis and dashboard creation to more powerful Business Intelligence tools like Power BI for enhanced interactivity, data modeling, and visualization capabilities.
4.  **External Data Integration:** Incorporating external datasets such as weather conditions, traffic flow data, and road infrastructure details to understand their influence on accident frequency and severity.

## References

1.  NYC Open Data - Motor Vehicle Collisions, data.cityofnewyork.us
2.  Microsoft Excel Official Documentation, support.microsoft.com
3.  Lovely Professional University Project Guidelines
