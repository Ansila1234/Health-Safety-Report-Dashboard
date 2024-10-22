# Health & Safety Report Analysis


## Overview
This project provides an analysis of health and safety incidents reported across multiple business units and sites using Power BI for visualization. The goal is to identify trends in workplace injuries, near misses, vehicle-related accidents, and overall incidents to recommend safety measures that can improve workplace conditions and reduce risks.

## Problem Statement

The company faces various health and safety challenges across multiple business units and sites. There is a need to analyze the reported incidents, injuries, and near-miss cases to understand trends, identify the most frequent issues, and propose data-driven solutions to reduce future occurrences.

### Key Objectives:

+ Analyze incidents by business unit and site.
+ Identify the most frequent types of injuries.
+ Track month-on-month (MoM) trends for incidents, lost hours, and vehicle accidents.
+ Present actionable insights for decision-makers to reduce health and safety risks.


## Data Description
The dataset includes health and safety data from various business units and sites for the year 2023. Key columns in the dataset include:

+ Incidents by Site: Number of incidents reported at various company sites.
+ Incidents by Business Unit: Breakdown of incidents across Transport, Production, Maintenance, and Site Activity.
+ Injuries: Analysis of injuries by type (finger, ankle, arm, etc.).
+ Near Misses: Number of near misses reported by month.
+ Vehicle Incidents: Incidents involving vehicles.
+ Lost Hours: Hours lost due to incidents.
+ Time Period: Data for the year 2023, with month-by-month comparisons.

## Tools and Technologies
+ Data Storage: CSV/Excel files containing raw data.
+ Data Processing: SQL for extracting and manipulating data.
+ Visualization: Power BI for building interactive dashboards and charts.


## Exploratory Data Analysis (EDA)
We performed an initial EDA to better understand the data:

+ Incidents by Site: Kirton, Hams Hall, and Kings Dyke reported the highest number of incidents in July 2023​[Health & Safety report](https://github.com/Ansila1234/Health-Safety-Report-Dashboard/blob/main/Health%20%26%20Safety%20report.pbix).
+ Business Unit Insights: Transport had the most incidents, followed by Maintenance and Production​[Health & Safety report](https://github.com/Ansila1234/Health-Safety-Report-Dashboard/blob/main/Health%20%26%20Safety%20report.pbix).
+ Injury Trends: Finger injuries were the most frequent, followed by ankle and foot injuries​[Health & Safety report](https://github.com/Ansila1234/Health-Safety-Report-Dashboard/blob/main/Health%20%26%20Safety%20report.pbix)

## Findings and Insights
+ Incident Hotspots: Kirton and Hams Hall consistently report the highest number of incidents. These locations should be prioritized for safety reviews​(Health & Safety report).
+ Most Vulnerable Business Units: Transport and Maintenance are particularly vulnerable, accounting for the majority of incidents.
+ Increase in Injuries: The number of injuries, particularly finger and ankle injuries, increased by 60% in July 2023 compared to previous months​(Health & Safety report).
+ Vehicle Incidents: Although vehicle incidents slightly decreased MoM (-3%), the overall numbers remain high and are a concern​(Health & Safety report).


## SQL Queries and Analysis
The project includes various SQL scripts used to analyze the dataset:

+ Incidents by Site: Breakdown of the number of incidents reported at different company sites.

SELECT Site, COUNT(IncidentID) AS TotalIncidents

FROM Incidents

GROUP BY Site

ORDER BY TotalIncidents DESC;

+ Injuries by Type: Analysis of the most frequent types of injuries.

SELECT InjuryType, COUNT(InjuryID) AS TotalInjuries

FROM Injuries

GROUP BY InjuryType

ORDER BY TotalInjuries DESC;

+ Business Unit Analysis: Number of incidents reported in each business unit.

SELECT BusinessUnit, COUNT(IncidentID) AS TotalIncidents

FROM Incidents

GROUP BY BusinessUnit

ORDER BY TotalIncidents DESC;

## Visualization
An interactive Power BI Dashboard was created to visualize key insights:

+ Incidents by Site: A bar chart visualizing which sites have the most incidents​(Health & Safety report).
+ Incidents by Business Unit: Stacked column charts showing incident trends across business units.
+ Injury Trends: Line graphs displaying the number of injuries by type over time.
+ Vehicle Incidents: Analysis of vehicle-related incidents​[Health & Safety report](https://github.com/Ansila1234/Health-Safety-Report-Dashboard/blob/main/Health%20%26%20Safety%20report.pbix).

## Key Findings
Based on the analysis, we identified several critical insights:

+ Incident Hotspots: Kirton and Hams Hall consistently report the highest number of incidents. These locations should be prioritized for safety reviews​.
+ Most Vulnerable Business Units: Transport and Maintenance are particularly vulnerable, accounting for the majority of incidents.
+ Increase in Injuries: The number of injuries, particularly finger and ankle injuries, increased by 60% in July 2023 compared to previous months​.
+ Vehicle Incidents: Although vehicle incidents slightly decreased MoM (-3%), the overall numbers remain high and are a concern​.

## Recommendations
Based on the findings, the following actions are recommended:

+ Enhanced Safety Training: Target high-risk sites like Kirton and Hams Hall for enhanced safety programs.
+ Focus on Transport: Implement stricter safety measures for the Transport unit, which reports the most incidents.
+ Injury Prevention: Focus on preventing finger and ankle injuries through improved equipment and safety protocols.
+ Vehicle Safety: Strengthen vehicle safety training and protocols to reduce incidents.

## Conclusion
The Health & Safety Report Analysis provides actionable insights that can be used to improve workplace safety, reduce incidents, and enhance productivity. By leveraging SQL and Power BI, the data is presented in an accessible format for decision-makers to take data-driven action.


## License
This project is licensed under the MIT License. Feel free to use and modify the code as needed.

By following this structure, you ensure that the repository is clear, easy to navigate, and provides comprehensive documentation for others to understand and replicate the analysis.











