# ENGO645_FINAL_PROJECT

## Documentation Overview

STUDY OF THE SPATIAL RELATIONSHIP BETWEEN FOOD SOURCES AND HEALTH OUTCOMES IN THE US.
*This Jupyter Notebook is designed to analyze county-level health and socioeconomic data. It includes processes for data loading, cleaning, merging, EDA visualization, Hotspot Analysis using Getis Ord GI, and in-depth modelling with Spatial Autocorrelation Regression to provide insights that might inform public health decisions.

**Data Sources** : Health Outcomes - https://nccd.cdc.gov/DHDSPAtlas/Default.aspx

**Food Sources** - https://www.ers.usda.gov/data-products/food-environment-atlas/documentation/

**County Boundaries** - https://www.arcgis.com/home/item.html?id=f16090f6d3da48ec8f144a0771c8fec4

**NB: You might need to download the County boundary from the link above. File was to big to push into the repository**

## Dependencies

To run this notebook effectively, ensure the following Python libraries are installed:

**Pandas** : Used for data manipulation and analysis.
**GeoPandas**: Utilized for handling geographic data.
**Matplotlib and Seaborn**: For plotting and visualizing data.
**NumPy**: Provides support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.
**SciPy**: Used for scientific and technical computing.
**scikit-learn**: For implementing machine learning algorithms.
**Pysal**: A library for spatial data analysis.

## Detailed Documentation

### Data Loading
Data is loaded from various sources, primarily Excel, CSV, and shapefile files, into pandas DataFrames and Geodataframes.

Example libraries used: Pandas and Geopandas

### Data Preprocessing
Initial data exploration includes checking for missing values and duplicate rows.
Relevant columns are selected and renamed for clarity and ease of analysis.
Data types are checked and converted as necessary to ensure compatibility for analysis.
Example functions: DataFrame.isnull(), DataFrame.duplicated(), DataFrame.drop(), DataFrame.rename()

### Data Merging
Multiple datasets are merged based on common identifiers (e.g., county IDs) to consolidate information into a single DataFrame for analysis.
Example methods: pandas.merge()

### Data Analysis
Descriptive statistics are computed to understand the distribution and central tendencies of the data.
Inferential statistics may be applied to draw conclusions or make predictions based on data samples.
Example functions: DataFrame.describe(), DataFrame.mean(), DataFrame.std()

### Data Visualization
- Visualizations are created to illustrate data trends, distributions, and relationships between variables.
- Plots such as histograms, scatter plots, and bar charts are used.
- libraries: matplotlib.pyplot, seaborn
- Spatial Data Analysis
- GeoPandas is used to handle spatial data, including transformations and operations such as projecting data to different coordinate reference systems.
- Spatial relationships and patterns are analyzed, often using visual mapping techniques.
- Example methods: GeoDataFrame.to_crs(), GeoDataFrame.plot()

**Conclusions**
Insights are derived from the analyses, highlighting key findings such as health disparities, trends over time, and the impact of socioeconomic factors on health outcomes.

**NB: Some EDA-related visualizations and dataframe adjustments were made while doing the actual datamining tasks to further examine and confirm the datasets used. Hence, some sections of the script may seem intermixed.**
