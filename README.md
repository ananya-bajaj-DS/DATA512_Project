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

For the development of a predictive model for future smoke estimates in Pueblo West, the project employs the DARTS library and uses the exponential smoothing algorithm. This model facilitates the projection of potential smoke impacts over the next 25 years.

**Data Visualization:**

The outcomes of the data analysis are visually conveyed through a variety of time series graphs and histograms. This visual representation offers a comprehensive overview of the wildfire impact on Pueblo West.

**Challenges Faced:**

Anticipated challenges during replication:

**Missing of Gaseous AQI Data in between:** The missingness of Gaseous AQI data for the assigned location posed a notable challenge, impacting the optimization process and necessitating the removal of its calculation from the project.

**Data Unavailability for Specific Years:** The absence of data for the years 1963-1983 prompted a modification to start the program loop from 1987, mitigating the risk of processing data for the unavailable time frame.

**Handling Large Datasets:** Efficiently managing and analyzing extensive wildfire datasets presented a significant challenge, demanding strategic optimization of data processing and analysis to ensure project execution was smooth.

**Data Extraction and Preprocessing:** Extracting and preprocessing the wildfire dataset for relevant information necessitated meticulous handling and processing. Managing the intricacies of data extraction and ensuring the data was appropriately formatted for analysis required careful attention to detail and expertise in data manipulation techniques.

**Visualization 1:**

This histogram illustrates the distribution of wildfires based on their proximity to a specific city. The x-axis denotes distance from the city in miles, divided into 50-mile intervals, while the y-axis represents the count of wildfires.
<img width="662" alt="image" src="https://github.com/ananya-bajaj-DS/DATA512_Project/assets/121599846/f429e387-7d47-427b-ac4a-28438c027712">

**Visualization 2:** This time series graph portrays the total acres burned by wildfires per year within a specified distance from the city. The x-axis represents the years, while the y-axis indicates the total acres burned by wildfires.

<img width="662" alt="image" src="https://github.com/ananya-bajaj-DS/DATA512_Project/assets/121599846/8ec5dc6c-9d20-4ea8-968a-fa814f38f1a5">

**Visualization 3:** This time series chart illustrates the patterns in the projected impact of fire smoke and the corresponding Air Quality Index (AQI) estimates for the city across the years. The horizontal axis denotes the years, while the vertical axis signifies the values of both the fire smoke estimate and the AQI estimate.

# PROJECT STRUCTURE
The project structure includes the main data processing and analysis scripts, as well as the data visualization components. The repository also contains additional documentation and resources related to the project.

# INSTALLATION
To install the required dependencies, use the following command:
pip install -r requirements.txt

# FOLDER STRUCTURE
1. LICENSE
2. README.md

# DATA FILES

# REPRODUCING THE ANALYSIS
To replicate this analysis, adhere to the following instructions:

Clone this repository to your local machine.
Ensure Python is installed with the required libraries.
Within the project directory, create a 'data' folder.
Download the GeoJSON Files.zip from this link, extract the "USGS_Wildland_Fire_Combined_Dataset.json" file, and place it in the 'data' folder.
Execute 'wildfire_analysis.ipynb' to generate analyses such as smoke analysis, AQI analysis, and their comparison.
Examine the results and interpret the findings accordingly.

# LICENSE
This project is licensed under the MIT License - see the LICENSE file for details.










