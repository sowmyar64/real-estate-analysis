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





![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/95d8d825-9b4e-4891-905c-6dd90f25ddb3)


The visualization presents the monthly trends for two key metrics in the market analysis data: revenue and occupancy rate.

##### Monthly Trend of Revenue:
- The line plot shows the average revenue generated each month throughout the year.
- Overall, there is a noticeable fluctuation in revenue from month to month, indicating variability in the business's performance.
- Revenue tends to peak during certain months, possibly corresponding to high-demand periods or seasonal fluctuations.

##### Monthly Trend of Occupancy:
- The line plot illustrates the average occupancy rate for each month.
- The occupancy rate also displays variability over time, with fluctuations from month to month.
- Peaks and valleys in the occupancy rate may coincide with seasonal factors, such as holidays, festivals, or vacation seasons, influencing travel patterns and accommodation demand.

In summary, the visualization provides valuable insights into the monthly performance trends of revenue and occupancy rate, enabling businesses to make data-driven decisions to enhance operational efficiency and financial performance.




![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/c5d03407-d079-417d-abfa-ef136bb3c39d)

The visualization shows the average length of stay per month over the analyzed period. The line plot indicates how the average length of stay fluctuates over time, with each point representing the mean length of stay for a specific month. 
Peaks and troughs in the plot indicate fluctuations in average length of stay, offering insights into booking patterns and seasonal trends. Businesses can use this information to optimize strategies related to pricing, marketing, and resource allocation, enhancing the overall guest experience.


![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/52f2464d-3944-4445-a9b7-93b3a650309a)
![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/89944d35-173e-4303-9681-c084fd6445df)


- The scatter plots depict the relationship between nightly rate and two key performance indicators: occupancy rate and revenue. 
- In the first plot, "Nightly Rate vs. Occupancy," each point represents a property, with its position indicating both the nightly rate and the corresponding occupancy rate. The color gradient represents the varying levels of occupancy, with darker shades indicating higher occupancy. 
- Similarly, in the second plot, "Nightly Rate vs. Revenue," the points represent properties, with their position indicating both the nightly rate and the corresponding revenue. The color gradient reflects the revenue generated, with darker shades indicating higher revenue. These visualizations help identify any trends or patterns between nightly rates and occupancy/revenue, aiding in pricing and revenue management strategies.



![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/6880bfd2-4aca-4311-b8fd-95c65eba7c87)


The bar charts display the average revenue and occupancy rate across different cities. 
##### Average Revenue by City:
The heights of the bars represent the average revenue generated by properties in each city. Cities with taller bars have higher average revenue per property. This information is valuable for understanding the financial performance of properties in different cities.

##### Average Occupancy by City: 
The heights of the bars represent the average occupancy rates of properties in each city. Cities with taller bars have higher average occupancy rates, indicating higher demand or better performance in terms of filling available capacity.



![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/f4942121-c81a-4a63-85ef-2cd869fe9081)


The bar chart illustrates the average property prices across different zip codes. 
- Variation in Average Property Prices: The heights of the bars vary, indicating differences in average property prices among different zip codes. Zip codes with taller bars have higher average property prices, while those with shorter bars have lower average prices.
- Identifying High and Low-Priced Areas: By comparing the heights of the bars, we can identify which zip codes tend to have higher or lower average property prices. This information can be valuable for real estate investors, homebuyers, or property developers seeking to target specific market segments or areas with varying price ranges.



![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/c7116492-87a0-4b54-857d-032a7e2a6ec0)


This visualization presents the distribution of various characteristics or features of properties, including the number of bedrooms, bathrooms, living area, home type, and presence of a pool.
##### Number of Bedrooms and Bathrooms:
- The first and second subplots display the distribution of the number of bedrooms and bathrooms, respectively.
- These plots provide insights into the typical configurations of bedrooms and bathrooms in the properties within the dataset. we can observe whether most properties have a specific number of bedrooms or bathrooms, which can be crucial information for homebuyers or renters.
##### Living Area:
- The third subplot illustrates the distribution of the living area (in square feet) of the properties.
- It helps in understanding the range and spread of living area sizes among the properties.
- Peaks in the distribution can indicate common sizes or preferences in living area dimensions.

##### Home Type:
- The fourth subplot shows the distribution of property types (e.g., single-family, apartment, condo) represented in the dataset.
- It provides insights into the diversity of property types and their respective proportions within the dataset.

##### Presence of a Pool:
- The fifth subplot presents the distribution of properties based on the presence or absence of a pool.
- It helps in understanding the prevalence of properties with pools and their relative frequency compared to those without pools.


![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/c35e02e1-86d6-4e0f-a51e-83a356460d4b)


This visualization displays the number of properties with a pool for each unique zip code in the dataset.
- Each bar represents a unique zip code, and the height of the bar indicates the count of properties with a pool in that specific zip code.
- By observing the heights of the bars, we can identify which zip codes have a higher concentration of properties with pools.
- This visualization allows us to identify geographic areas or zip codes where properties with pools are more prevalent, which can be valuable information for potential buyers or investors interested in such amenities.

![image](https://github.com/sowmyar64/real-estate-analysis/assets/43263218/e6ac8d78-9c57-4334-bfa5-9d10bcf635d3)


This visualization depicts the distribution of property status categorized by postal code.
- Each bar represents a unique Zipcode, and the height of the bar indicates the count of properties within that postal code.
- The bars are further divided into segments of different colors, representing different statuses of the properties.
- Zip codes with taller bars in specific status segments indicate a higher concentration of properties with that particular status.
- This visualization enables stakeholders to understand the distribution of property statuses geographically, identifying areas with a higher number of properties for sale, sold, or new construction, among other statuses.
- It provides valuable information for real estate professionals, investors, and buyers to assess market conditions and make informed decisions based on the status of properties within different postal code areas.




# Conclusion
The analysis of Airbnb data sheds light on key factors influencing property investment decisions and revenue optimization. Geographic insights highlight popular rental areas and seasonal revenue trends, aiding pricing strategies. Property features like pools and hot tubs are prevalent, reflecting market preferences. Location-based analysis identifies high-demand areas, guiding investment decisions. Moreover, examining property characteristics by postal zone reveals varied occupancy rates and pricing dynamics.Additionally,the examination of property characteristics in each postal zone suggests that Joshua Tree (92252) and Yucca Valley (92284) exhibit the highest average occupancy, while the Big Bear zone commands higher prices and offers more amenities, contributing to its superior profitability.Overall, understanding these trends enables property owners and investors to make informed decisions and maximize returns.
