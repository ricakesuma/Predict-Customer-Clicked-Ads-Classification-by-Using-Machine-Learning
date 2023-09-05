# Predict Customer Clicked Ads Classification

### Introduction

A company in Indonesia aims to determine the effectiveness of an advertisement they have launched. This is crucial for a company operating in the digital marketing consulting field to gauge the reach of their marketed ads and attract customers to view the ads. The company seeks to extract insights regarding user behavior from the collected data by creating visualizations, developing a relevant machine learning model to meet their needs, and providing recommendations based on the findings.

### Data Overview

| Attribute                | Description                                                                                     |
|--------------------------|-------------------------------------------------------------------------------------------------|
| Daily Time Spent on Site | Amount of time the user spends on the site daily (likely in minutes or hours).                  |
| Age                      | Age of the user.                                                                                |
| Area Income              | Income level in the user's residential area (likely in currency units).                         |
| Daily Internet Usage     | Amount of daily internet consumption by the user (likely in MB or GB).                          |
| Male                     | Binary indicator representing the gender of the user (e.g., 1 for male, 0 for female).           |
| Timestamp                | Date and time of the activity or interaction, possibly indicating when the ad was clicked.      |
| Clicked on Ad            | Binary indicator representing whether the user clicked on the ad (e.g., 1 for clicked, 0 for not clicked). |
| City                     | City where the user resides.                                                                    |
| Province                 | Province or state where the user resides.                                                       |
| Category                 | Category of the ad or product being advertised.                                                 |

### Step-by-Step Analysis
1. **Import Packages**: Importing necessary libraries such as pandas, numpy, matplotlib, and seaborn.
2. **Load Dataset**: Reading the dataset named "Clicked Ads Dataset.csv" containing information related to customer interactions with online ads.
3. **Check Duplicate Rows**: Identifying and printing duplicate rows in the dataset.
4. **Check Missing Values**: Identifying and displaying missing values in different columns.
5. **Convert Timestamp**: Converting the "Timestamp" column to a datetime data type.
6. **Handle Missing Values**: Filling missing values in the "Daily Time Spent on Site" column based on the median of the respective age group.
7. **Modelling**: Use Modelling in Confusion Matrix, and using Random Forest Classifier With and Without Normalization. 

### Interpretation
By understanding customer behavior in clicking on ads, companies can enhance the efficiency of their advertising campaigns. For instance, comprehending demographics allows firms to better target ads towards specific groups more inclined to engage with them. If there's a particular pattern indicating when customers are more likely to click on ads, such as specific times during the day, companies can optimize their ad broadcast times accordingly. Recognizing the relationship between regional income or daily internet usage and the likelihood of ad engagement can assist firms in tailoring their ad messages or special offers, aiming to boost engagement rates. Furthermore, by targeting ads towards customers more likely to engage, companies can reduce costs wasted on disinterested customers and enhance the Return on Investment (ROI) from their advertising campaigns.

### Business Recommendations
1. **Customer Segmentation**: Based on features such as age, income, and daily internet usage, companies should segment their customers and target tailored ads to each segment. This approach ensures that the right message reaches the right audience, increasing the likelihood of engagement.
2. **A/B Testing**: Before launching a full-scale advertising campaign, companies should conduct A/B tests with different ad variations. This helps identify which version of the ad resonates most with the target audience and ensures maximum engagement when the campaign is rolled out widely.
3. **Further Analysis**: Beyond just classification modeling, companies might consider clustering analyses to identify groups of similar customers. By understanding these clusters, companies can adjust their advertising strategies to appeal to specific groups, further improving engagement rates.
4. **Cost Optimization**: With insights into which features influence customer click behavior the most, companies can better allocate their advertising budget. By focusing on those features that are more likely to result in engagement, they can reduce their cost-per-click and achieve a higher return on their advertising spend.
