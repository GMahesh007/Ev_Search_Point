# EV Search Point

## Overview
This project, **EV Search Point**, is a personal side project aimed at gaining familiarity with spatial data analysis tools such as GeoPandas, PySal, PostgreSQL, and PostGIS. Additionally, the project explores the distribution and density of EV charging stations across Ontario, Canada, to uncover meaningful spatial patterns.

## Motivation
The initial motivation was personal curiosity about the quantity and geographical spread of EV stations across Canada. Upon analyzing the data, it became evident that Ontario and Quebec lead in EV station deployment. Ontario was chosen for deeper analysis due to a better familiarity with its cities and towns.

## Methodology
Spatial data analysis was conducted to:
- Identify patterns in the distribution of EV stations.
- Determine cold and hot spots using spatial auto-correlation:
  - **Hot spot:** A region with a high number of EV stations surrounded by other high-density regions.
  - **Cold spot:** A region with a low number of EV stations surrounded by other low-density regions.
- The number of EV stations in each census area was used as the primary spatial attribute for this analysis.

## Feature Engineering
To enhance the dataset, two new attributes were incorporated:
- **Median Income**
- **Population per Census Area**

These attributes were chosen because income and population often correlate with EV ownership and, consequently, EV station distribution. A clustering technique was applied to group regions based on these features and compare results with spatial analysis.

## Key Findings
- **Cold Spots:** Found in northern census areas, except for those along the TransCanada Highway.
- **Hot Spots:** Concentrated around Toronto and its neighboring census areas.
- **Potential Insights for Service Providers:**
  - High-income, high-population areas with few stations indicate potential locations for new charging stations.
  - High-income, low-population areas with few stations suggest a market for home charging solutions.

## Future Enhancements
Further research could include additional factors influencing EV station distribution, such as:
- Commute time
- Gender demographics
- Age distribution
- Occupation types
- Political views

## Tools & Technologies Used
- **GeoPandas**: Spatial data manipulation
- **PySal**: Spatial statistics and clustering
- **PostgreSQL & PostGIS**: Storing and querying spatial data

## Conclusion
This project provided valuable insights into EV station distribution in Ontario and demonstrated the power of spatial data analysis in infrastructure planning. A deeper study could assist policymakers and service providers in optimizing EV station placement for better accessibility and efficiency.
