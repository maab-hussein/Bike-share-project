# Cyclistic bike-share Analysis

### Project Overview

- Cyclistic is a bike-share program that features more than 5,800 bicycles and 600 docking stations. There are two types of memberships. Customers who purchase annual memberships are Cyclistic members, and customers who purchase anything else are Cyclistic casuals.
- The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, my team needs to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, my team should design a new marketing strategy to convert casual riders into annual members.
- This project is mainly based on Excel.

### Data Sources

- [The original data.](https://1drv.ms/f/c/1c14129f07a236b3/EnDMZWSGyK5MmhGCLFtdzc4BhbyHUVj5mAYlc0klYgUVXQ)
- [Cleaned, edited and enhanced source in the power query.](https://1drv.ms/f/c/1c14129f07a236b3/EnDMZWSGyK5MmhGCLFtdzc4BhbyHUVj5mAYlc0klYgUVXQ)

### Data Cleaning and Preparation
- **Data Importing and Loading:**
  - Used Excel’s “Get & Transform” (Power Query) feature to load and transform over 5.5 millions of rows.
- **Removing Duplicates:**
  - Checked for duplicates by using the **Remove Duplicates** button in the data tools.
- **Data Transformation:**
  - Converted data types and standardized formats using Excel functions.
- **Handling Inconsistencies:**
  - Using `=SIGN` function and filters, I realized there were negative values in "duration" column, so I had to remove them while in real life I will have more ways to detect the reason behind these inconsistencies and handle them in better ways.
 
### Exploratory Data Analysis

EDA involved finding trends and insights to answer these questions:

- How do annual members and casual riders use Cyclistic bikes differently?
- Why would casual riders buy Cyclistic annual memberships?
- How can Cyclistic use digital media to influence casual riders to become members?

Additionally, I conducted initial data exploration using Excel features like PivotTables, filters, and conditional formatting to identify data patterns and anomalies. I calculated mean, median, mode, standard deviation, and simple statistics to measure the central tendency and scattering of the data.



### Interactive Excel Dashboard

An interactive Excel dashboard was created to visualize key insights from the analysis.

## Steps to Access the Dashboard
1. **Download the Excel File**: [Bike-share dashboard.xlsx](https://1drv.ms/f/c/1c14129f07a236b3/EnDMZWSGyK5MmhGCLFtdzc4BhbyHUVj5mAYlc0klYgUVXQ)
2. **Open the Excel File using Microsoft Excel.**
2. **Navigate to the Dashboard Sheet**

### The Dashboard

![Dashboard](https://github.com/user-attachments/assets/8bceca2e-e249-4cce-8b8c-a2a5ff71fba4)

### Key Features of the Dashboard

- **Interactive Charts**:
  - A slicers are used to filter data by different categories. In the bar chart and the line chart slicers were used to analyze bikers' behaviors based on membership type.
  - Another slicer was used to filter data based on months.

- **Summary Statistics**:
  - Key metrics such as churn rate, average tenure, and monthly charges are displayed prominently.

- **Trend Analysis**:
  - Heatmap shows riders' density throughout months. During the months of June, July and August numbers of bikers increase noticeably.
  - The bar chart shows the number of riders during each day of the week for each membership type. Casual members tend to bike more on Saturdays and Sundays.
  - The line chart shows when each membership type tends to bike in days' hours. There is an obvious increase in 5 a.m and 5 p.m for members.
  - The pie chart shows the percentage of each membership for every month. It shows that the percentage of members is already increasing.
