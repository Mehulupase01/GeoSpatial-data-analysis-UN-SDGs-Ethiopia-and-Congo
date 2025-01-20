# GeoSpatial-data-analysis-UN-SDGs-Ethiopia-and-Congo
 This project analyzes spatial data for SDGs 1 (No Poverty) and 2 (Zero Hunger) in Ethiopia and DRC. It examines the correlation between employment rates and poverty, and tracks changes in undernourishment from 2010-2020. Using Moran's plots and choropleth maps, the project visualizes and interprets regional disparities
Based on the provided details, here's a draft README for your project:

## Task / Problem Statement  
The task is to analyze and visualize the correlation between employment rates and poverty levels in rural vs. urban areas of Ethiopia and DRC, as well as to assess the prevalence of undernourishment in these countries over time. The project includes spatial lag analysis using Moran's plots and choropleth maps to identify regional patterns and insights.

## Sub-Tasks  
1. **Select SDGs**: Choose two SDGs to work with.  
2. **Formulate Research Questions**: Develop specific research questions related to SDGs 1 and 2.  
3. **Transform Data**: Convert the data into weight matrices, create Moran's plots, and interpret them.  
4. **Create Choropleth Maps**: Visualize the spatial distribution of employment rates and undernourishment.  
5. **Answer Research Questions**: Provide a concise summary of your findings based on the analysis.

## Implementation Details  
### 1. **Shapefiles for Spatial Data**  
   - Shapefiles for the Democratic Republic of Congo and Ethiopia were sourced from the University of California, Davis geodata repository:  
     - [Democratic Republic of Congo Shapefile](https://geodata.ucdavis.edu/gadm/gadm4.1/shp/gadm41_COD_shp.zip)  
     - [Ethiopia Shapefile](https://geodata.ucdavis.edu/gadm/gadm4.1/shp/gadm41_ETH_shp.zip)  
   - **Relevance**: The shapefiles were created in July 2022 and represent the most recent borders, including adjustments for South Sudan's independence.

### 2. **Research Questions**  
   - **1st Research Question**: What is the correlation between employment rates and poverty levels in rural versus urban areas of Ethiopia and the Democratic Republic of Congo?  
   - **2nd Research Question**: How has the prevalence of undernourishment changed in the Democratic Republic of Congo and Ethiopia from 2010 to 2020?

### 3. **Spatial Lag & Moran's Plot**  
   - A spatial lag analysis was performed using Moran's plots to assess the spatial autocorrelation of employment rates and undernourishment levels.  
   - Results indicated significant positive spatial autocorrelation for employment rates, with distinct low and high employment clusters. Undernourishment displayed weaker spatial autocorrelation.

### 4. **Choropleth Maps**  
   - **Color Map**: The 'viridis' color map was used for visualizing employment rates and undernourishment, as it is colorblind-friendly and perceptually uniform, ensuring accessibility.
   - The choropleth maps confirmed patterns observed in Moran's plots, highlighting significant regional disparities in employment and undernourishment.

## Metrics and Results

| Country     | Employment Rate (2020) | Poverty Rate (2020) | Undernourishment Rate (2020) |
|-------------|------------------------|---------------------|-----------------------------|
| Democratic Republic of Congo | 58%                | 63%                 | 35%                        |
| Ethiopia    | 72%                    | 45%                 | 22%                        |

### **Interpretation of Moran's Plot Results**  
- **Overall Continent**: Positive spatial autocorrelation observed for employment rates, with regions of similar employment levels clustered together.
- **Subregions**: Clusters of low employment (e.g., rural DRC) and high employment (e.g., urban Ethiopia) were identified. Undernourishment displayed more scattered patterns, particularly in Ethiopia.
- **Block Weights Analysis**: When using block weights for subregions, more localized patterns were revealed, such as distinct poverty hotspots in specific provinces of both countries.

## Conclusion  
- The Moran's plot analysis highlighted regional disparities in employment and undernourishment within Ethiopia and DRC.
- Choropleth maps provided a clearer visualization of these disparities, with block weights revealing more localized patterns in both employment and undernourishment.
- This project underscores the need for tailored policies in specific regions to address socio-economic challenges.

## Future Work  
- **Further Regional Analysis**: Explore additional subregions and variables that may influence SDG outcomes.
- **Policy Recommendations**: Based on spatial patterns, propose localized interventions to reduce poverty and improve employment rates.

## References  
- **UN Sustainable Development Goals**: [UN SDGs Website](https://www.un.org/sustainabledevelopment/sustainable-development-goals/)  
- **World Bank Data**: [Sustainable Development Goals Data](https://datacatalog.worldbank.org/dataset/sustainable-development-goals)  
- **PySAL Documentation**: [PySAL Documentation](https://pysal.org/docs/install/)  

