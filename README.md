# real-estate-analysis
# Airbnb market analysis and real estate sales
# 1. Introduction
## Project Overview
The Airbnb Analysis project focuses on analyzing Airbnb data from the travel industry and property management domain. By leveraging various data analysis and visualization tools, we aim to extract valuable insights into pricing dynamics, availability patterns, and location-based trends in Airbnb listings.
# Objectives
The primary objectives of this project include:

1) Ensure data quality and consistency by addressing missing values, outliers, and duplicates.
2) Standardize data formats and rectify inconsistencies in column names or values.
3) Validate and clean geographic coordinates, zip codes, and other location-based data to maintain data integrity.
4) Utilize EDA techniques to grasp data distributions, trends, and interrelationships.
5) Summarize and visualize key features using descriptive statistics, histograms, scatter plot and heat map
6) Identify correlations between variables and uncover potential patterns or anomalies.
7) Analyzing geographic trends analysis to identify spatial clusters, hotspots, or patterns in Airbnb listings or amenities distribution.
8) Visualization process utilizes various tools and libraries, such as matplotlib, Seaborn, Plotly, to generate static and interactive visualizations like plots and charts.

# About Dataset

This dataset, titled 'Airbnb Market Analysis and Real Estate Sales Data (2019),' comprises a comprehensive collection of information pertaining to the Airbnb rental market and property sales in two distinct areas within California: Big Bear and Joshua Tree, along with their associated zip codes (92314, 92315, 92284, and 92252). The dataset provides monthly aggregated data, allowing for an in-depth analysis of rental and real estate market trends in these regions. It includes the following files:

## Datasets:
### Market Analysis:
This file contains listing-level information from 2019, aggregated on a monthly basis. It encompasses various metrics, such as unique property codes (unified_id), generated revenue, availability (openness), occupancy ratios, nightly rates, lead times, and average length of stay for reservations made each month. Additionally, it provides insights into property amenities.

### Amenities:
This file indicates whether a listing has specific amenities, denoting their presence with a value of 1 or their absence with a value of 0. Notably, it identifies the availability of a pool or hot tub in each listing.

### Geolocation:
This file contains latitude and longitude coordinates for each listing, enabling precise spatial analysis and visualization.

### Sales Properties:
This dataset provides information concerning properties available for sale within the study areas. In the Joshua Tree region (zip codes 92284 and 92252), there are two separate files—one presenting the overall information about sales properties and the other focusing on properties with pools.

This dataset is a valuable resource for researchers and analysts interested in gaining insights into the real estate and Airbnb rental markets in California, particularly within the specified regions.


# 2. Methodology
### Data Collection 
Gather relevant datasets from sources such as Airbnb listings, geolocation data, and market analysis reports.

### Data Cleaning
Identify and address missing values, outliers, and inconsistencies in the datasets to ensure data integrity and accuracy.

### Exploratory Data Analysis (EDA) 
Explore the datasets to understand distributions, trends, and relationships between variables using descriptive statistics and data visualization techniques.

### Geographic Analysis
Analyze geographic trends such as property density, proximity to attractions, and location-based insights to gain a deeper understanding of the market.


![image](https://github.com/sowmyar64/Real-estate/assets/43263218/8435af88-7c8c-45ce-adc9-f050e3ddf25c)

The visualization "Distribution of Data Points by Month" illustrates the spread of data across different months in the geolocation dataset. Each bar represents the count of data points corresponding to a specific month. The height of the bars indicates the frequency of data points recorded in each month. By observing the distribution, we can identify any noticeable seasonal trends or patterns in the data. we may observe higher counts during certain months, indicating periods of increased activity or data collection.
### Visualization
Create informative and visually appealing plots, charts, maps to communicate insights effectively to stakeholders.




![image](https://github.com/sowmyar64/Real-estate/assets/43263218/5771546c-c3eb-47ae-866c-2020b9139e8f)

The scatter plot "Geographical Distribution of Data Points" displays the spatial distribution of data points based on latitude and longitude coordinates. It provides insights into the geographic coverage of the dataset, highlighting concentrations or clusters of data points in specific regions. 




![image](https://github.com/sowmyar64/Real-estate/assets/43263218/103835af-b682-400f-b773-4cca0b58c862)

The bar plot "Top 5 Most Common Street Names (Excluding Unspecified)" illustrates the frequency of occurrence of the top 5 street names in the dataset, excluding instances where the street name is not specified. It provides insights into the most prevalent street names within the dataset, helping to identify common naming patterns or frequently encountered locations. This visualization aids in understanding the distribution of properties across different street names and their relative popularity.




![image](https://github.com/sowmyar64/Real-estate/assets/43263218/bf6ab0c3-a8ed-40f1-9f4b-2f34ecd0114a)

The bar plot "Top 5 Least Common Street Names (Excluding Unspecified)" displays the frequency of occurrence of the least common street names in the dataset, excluding instances where the street name is not specified. It highlights street names with the lowest frequency within the dataset, offering insights into less commonly encountered locations or unique naming conventions. This visualization aids in identifying outliers or rare occurrences among street names, which may have implications for property distribution or geographic analysis.




![image](https://github.com/sowmyar64/Real-estate/assets/43263218/23642e79-d59c-4457-bfee-2a5a8417a89d)

The visualization above illustrates the distribution of hot tubs and pools among the properties in the dataset.

In the first subplot, "Distribution of Hot Tubs," the bar plot shows the count of properties with and without hot tubs. The blue bars represent the presence or absence of hot tubs, with "Absent" indicating properties without hot tubs and "Present" indicating properties with hot tubs. From this plot, it's evident that there are more properties without hot tubs compared to those with hot tubs.

In the second subplot, "Distribution of Pools," the bar plot displays the count of properties with and without pools. Similarly, the green bars represent the presence or absence of pools, with "Absent" indicating properties without pools and "Present" indicating properties with pools. Here, it's noticeable that the majority of properties do not have pools, as indicated by the higher count of "Absent" compared to "Present."

which could be useful for potential renters or buyers interested in such amenities.




![image](https://github.com/sowmyar64/Real-estate/assets/43263218/6dc07c8e-8037-4981-bbf5-92dec80afb48)

The visualization above depicts the quarterly trends of hot tub and pool presence among properties over different years.

In the left subplot, "Quarterly Trend of Hot Tub Presence," the bar plot shows the total count of hot tubs across different quarters. Each bar represents a quarter, and the height of the bars indicates the total number of hot tubs present in properties during that quarter. The bars are color-coded by year, allowing for a comparison of hot tub trends across different years.
Similarly, the right subplot, illustrates the total count of pools across quarters, with bars representing each quarter and color distinguishing between different years.
which could inform decisions related to property management, rental pricing, or marketing strategies.






![image](https://github.com/sowmyar64/Real-estate/assets/43263218/041f1105-030b-4fa0-895c-089c78d41b8a)

The heatmap visualization above represents the correlation between the presence of hot tubs and pools in properties.
##### In this heatmap:
The cell at the intersection of 'hot_tub' and 'pool' displays the correlation coefficient, which quantifies the relationship between the presence of hot tubs and pools.
Annotating the heatmap with correlation values provides a quick overview of the strength and direction of the correlation.
The colormap ('coolwarm') visually represents the correlation values, with cool colors (blue) indicating negative correlations, warm colors (red) indicating positive correlations, and shades of white representing values close to zero.
##### Interpretation:
A positive correlation coefficient closer to 1 suggests that the presence of hot tubs and pools tends to co-occur, meaning properties with hot tubs are more likely to have pools as well.
A negative correlation coefficient closer to -1 would indicate the opposite scenario, where the presence of one feature is associated with the absence of the other.
A correlation coefficient close to 0 implies no significant linear relationship between the presence of hot tubs and pools.





![image](https://github.com/sowmyar64/Real-estate/assets/43263218/e896959c-390c-4edf-abff-cd1d6d71720d)

The visualization above depicts the monthly trends of revenue and occupancy rates based on the market analysis data.

##### Monthly Trend of Revenue:
- The line plot shows the average revenue generated each month over the analyzed period.
- The x-axis represents the months, while the y-axis represents the average revenue.
- The blue line illustrates the fluctuation in revenue over time.
###### Interpretation: 
Observing the trend helps in identifying seasonal patterns or trends in revenue generation. spikes or dips in revenue can indicate peak or off-peak seasons, respectively. Additionally, steady growth or decline in revenue over time can provide insights into the overall performance of the market.

##### Monthly Trend of Occupancy:
- The line plot shows the average occupancy rate each month.
- The x-axis represents the months, while the y-axis represents the average occupancy rate.
- The green line represents the trend in occupancy rates across different months.
###### Interpretation: 
Analyzing the occupancy trend helps in understanding demand patterns throughout the year. High occupancy rates suggest strong demand, while low occupancy rates may indicate periods of lower demand. Identifying peaks and troughs in occupancy can inform property management decisions, pricing strategies, and marketing efforts.




![image](https://github.com/sowmyar64/Real-estate/assets/43263218/f5c321ef-eabb-4e76-b8ac-4db5aa54f939)


The visualization above presents the average revenue and occupancy rates across different cities based on the market analysis data.

##### Average Revenue by City:
- The left subplot illustrates the average revenue generated in each city.
- Cities are represented on the x-axis, while the average revenue is depicted on the y-axis.
- Each bar represents the average revenue for a specific city, with the height indicating the revenue value.
###### Interpretation:
This plot allows for a comparison of revenue generation across different cities. Cities with taller bars have higher average revenue, indicating stronger financial performance. Understanding revenue disparities among cities can guide investment decisions, marketing strategies, and resource allocation.

##### Average Occupancy by City:
- The right subplot displays the average occupancy rates for each city.
- Cities are shown on the x-axis, while the average occupancy rate is displayed on the y-axis.
- Each bar represents the average occupancy rate for a specific city, with the height indicating the occupancy percentage.
###### Interpretation: 
This plot facilitates the comparison of occupancy rates across different cities. Higher bars indicate cities with higher average occupancy rates, suggesting strong demand for accommodations. Identifying cities with consistently high occupancy rates can help in prioritizing investment opportunities and optimizing pricing strategies to maximize revenue.


![image](https://github.com/sowmyar64/Real-estate/assets/43263218/00c67ba2-8a8e-4566-bc83-19e602853405)

The visualization above presents the average revenue and occupancy rates across the top 10 zip codes based on the market analysis data.

##### Average Revenue by Zipcode (Top 10):
- The left subplot illustrates the average revenue generated in the top 10 zip codes.
- Zipcodes are represented on the x-axis, while the average revenue is depicted on the y-axis.
- Each bar represents the average revenue for a specific zipcode, with the height indicating the revenue value.
###### Interpretation: 
This plot allows for a comparison of revenue generation among the top-performing zip codes. Zip codes with taller bars have higher average revenue, indicating stronger financial performance. Understanding revenue disparities among zip codes can inform investment decisions, marketing strategies, and resource allocation.

###### Average Occupancy by Zipcode (Top 10):
- The right subplot displays the average occupancy rates for the top 10 zip codes.
- Zipcodes are shown on the x-axis, while the average occupancy rate is displayed on the y-axis.
- Each bar represents the average occupancy rate for a specific zipcode, with the height indicating the occupancy percentag
###### Interpretation: 
This plot facilitates the comparison of occupancy rates among the top-performing zip codes. Higher bars indicate zip codes with higher average occupancy rates, suggesting strong demand for accommodations. Identifying zip codes with consistently high occupancy rates can help prioritize investment opportunities and optimize pricing strategies to maximize revenue.




![image](https://github.com/sowmyar64/Real-estate/assets/43263218/3839b4a1-f687-4bed-b1f2-85c02d727b30)
![image](https://github.com/sowmyar64/Real-estate/assets/43263218/56127a85-3aff-4516-85a6-de518fa883c7)
![image](https://github.com/sowmyar64/Real-estate/assets/43263218/c9fe6d14-678b-4990-a472-b44fb8c11628)

The scatter plots above depict relationships between different variables in the market analysis dataset:

##### Scatter Plot of Revenue vs. Occupancy:
- This plot illustrates the relationship between revenue and occupancy rate.
- Each point on the scatter plot represents a specific listing or property.
- The x-axis represents the occupancy rate, while the y-axis represents revenue.
###### Interpretation:
The scatter plot allows us to observe how changes in occupancy rates correspond to changes in revenue. Clusters of points with higher revenue may indicate properties with consistently high occupancy rates, suggesting a positive correlation between occupancy and revenue.

##### Scatter Plot of Revenue vs. Nightly Rate:
- This plot showcases the relationship between revenue and nightly rate.
- Each point on the scatter plot represents a specific listing or property.
- The x-axis represents the nightly rate, while the y-axis represents revenue.
###### Interpretation:
The scatter plot helps identify how changes in nightly rates affect revenue generation. Clusters of points with higher revenue at lower nightly rates may indicate properties that attract more bookings due to competitive pricing or higher perceived value.

##### Scatter Plot of Occupancy vs. Length of Stay:
- This plot visualizes the relationship between occupancy rate and length of stay.
-Each point on the scatter plot represents a specific listing or property.
- The x-axis represents the length of stay, while the y-axis represents the occupancy rate.
###### Interpretation: 
The scatter plot allows us to examine how the length of stay influences occupancy rates. Properties with longer average stays may exhibit higher occupancy rates, indicating potential opportunities to target guests seeking extended accommodations.

# Conclusion
The analysis of Airbnb data reveals key insights for property owners and investors. Geographic distribution highlights popular rental areas, while revenue and occupancy trends show seasonal variations with a positive correlation. Property features like hot tubs and pools are prevalent, often with a moderate positive correlation between them. Location-based analysis identifies high-demand areas, aiding investment decisions. Market trends uncover seasonal patterns and guide pricing strategies. Overall, these insights optimize revenue and occupancy rates in the Airbnb real estate market.




