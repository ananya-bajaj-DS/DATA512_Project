# DATA512_Project
# Wildfire Impact Analysis in Pueblo West City

The objective of this undertaking is to assess the consequences of wildfires in Pueblo West City, with a specific emphasis on gauging the smoke effects spanning the past six decades. The examination encompasses tasks such as extracting and filtering data, estimating smoke levels, and establishing correlations with Air Quality Index (AQI) data. Furthermore, a predictive model has been crafted to anticipate forthcoming smoke estimates.

# Introduction
With increasing frequency, summers in the western United States have become synonymous with wildfires, resulting in widespread smoke that affects various facets of society. This initiative centers on the analysis of the wildfire impact on Pueblo West, seeking to offer insights into the historical and anticipated levels of smoke exposure in the city.

# Common Analysis
The course project encompasses a thorough examination of the repercussions of wildfires on a designated city in the United States. The primary objective is to equip policymakers and civic institutions with valuable insights, enabling them to formulate well-informed strategies for mitigating potential future impacts stemming from wildfires. The project unfolds in four segments, with Part 1 serving as the foundational analysis that sets the groundwork for subsequent tasks.

Part 1 initiates with data acquisition, utilizing the Combined wildland fire datasets for the United States and certain territories, spanning from the 1800s to the present, as the basis for the analysis. This section of the project entails the generation of annual estimates for wildfire smoke impacts on the specified city over the past 60 years (1963-2023). Additionally, the analysis involves a comparative examination, aligning the created smoke estimates with the Air Quality Index (AQI) data from the US Environmental Protection Agency (EPA) to validate the accuracy of the estimations.

Furthermore, a predictive model is crafted to forecast smoke estimates for the city over the next 25 years, emphasizing the importance of conveying appropriate levels of uncertainty inherent in the predictions. The subsequent phase, Step 2 of the project, focuses on visualizing the analysis through a variety of time series graphs. These visual representations include a histogram detailing the frequency of fires occurring at 50-mile intervals from the city, a time series graph illustrating the annual total acres burned for fires within a specific distance from the city, and another time series graph showcasing the fire smoke estimate for the city in conjunction with the corresponding AQI estimate.

# Data Sources
The focal dataset for the common analysis research question is the USGS_Wildland_Fire_Combined_Dataset.json, accessible at the Combined wildland fire datasets for the United States and certain territories, spanning from the 1800s to the present (combined wildland fire polygons). This dataset has been compiled and consolidated by the US Geological Survey and is adequately documented. The fire polygons within the dataset are accessible in both ArcGIS and GeoJSON formats. Each participant has been allocated a specific US city as the focal point for their individual analysis, and the assigned city can be identified in the Google spreadsheet provided.

source: https://www.sciencebase.gov/catalog/item/61aa537dd34eb622f699df81

The below sample codes were referenced for the following tasks and have been provided under the Creative Commons CC-BY license:

Sample notebook for Geodetic Distance Computation
Sample code for accessing the US EPA Air Quality System API
Sample code for GeoJSON reader
Link: https://drive.google.com/drive/folders/1OJktGAx86hvMtirCUkGnS292r-FpPvLo

# Project parts

**Data Extraction:**

The dataset utilized in this analysis is the Combined Wildland Fire Datasets for the United States and certain territories, spanning from the 1800s to the present (combined wildland fire polygons). This dataset has been curated and compiled by the US Geological Survey. The extraction and processing of data are carried out using Python modules and diverse data processing techniques.

**Data Filtering and Preprocessing:**

The phase of data filtering and preprocessing involves the selection of fire perimeters within a 1250-mile radius of Pueblo West. This targeted approach enables the extraction of pertinent fire data for subsequent analysis.

**Smoke Estimation Process:**

The smoke estimation process entails the calculation and normalization of the smoke impact associated with each fire event, utilizing predefined parameters. The resulting estimated smoke impacts undergo further processing and correlation with the available Air Quality Index (AQI) data.

**Correlation Analysis:**

Correlation analysis delves into exploring the relationship between the estimated smoke impacts and the Air Quality Index data. This exploration provides valuable insights into the correlation between fire smoke and air quality in Pueblo West.

**Predictive Model:**

For the development of a predictive model for future smoke estimates in Pueblo West, the project employs the X library. This model facilitates the projection of potential smoke impacts over the next 25 years.

**Data Visualization:**

The outcomes of the data analysis are visually conveyed through a variety of time series graphs and histograms. This visual representation offers a comprehensive overview of the wildfire impact on Pueblo West.

**Challenges Faced:**

Anticipated challenges during replication:

**Missing of Gaseous AQI Data in between:** The missingness of Gaseous AQI data for the assigned location posed a notable challenge, impacting the optimization process and necessitating the removal of its calculation from the project.

**Data Unavailability for Specific Years:** The absence of data for the years 1963-1983 prompted a modification to start the program loop from 1987, mitigating the risk of processing data for the unavailable time frame.

**Handling Large Datasets:** Efficiently managing and analyzing extensive wildfire datasets presented a significant challenge, demanding strategic optimization of data processing and analysis to ensure project execution was smooth.
Data Extraction and Preprocessing: Extracting and preprocessing the wildfire dataset for relevant information necessitated meticulous handling and processing. Managing the intricacies of data extraction and ensuring the data was appropriately formatted for analysis required careful attention to detail and expertise in data manipulation techniques.

Visualization 1:

This histogram illustrates the distribution of wildfires based on their proximity to a specific city. The x-axis denotes distance from the city in miles, divided into 50-mile intervals, while the y-axis represents the count of wildfires.










