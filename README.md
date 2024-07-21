# Cyclistic bike-share Analysis

### Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Interactive Excel Dashboard](#interactive-excel-dashboard)
- [Key Features of the Dashboard](#key-features-of-the-dashboard)
- [Analysis](#analysis)
- [Recommendations](#recommendations)

### Project Overview

- Cyclistic is a bike-share program that features more than 5,800 bicycles and 600 docking stations. There are two types of memberships. Customers who purchase annual memberships are Cyclistic members, and customers who purchase anything else are Cyclistic casuals.
- The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, my team needs to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, my team should design a new marketing strategy to convert casual riders into annual members.
- This project is mainly based on Excel.

### Data Sources

- [The original data.](https://1drv.ms/f/c/1c14129f07a236b3/EnDMZWSGyK5MmhGCLFtdzc4BhbyHUVj5mAYlc0klYgUVXQ)
- [Cleaned, edited, and enhanced source in the power query.](https://1drv.ms/f/c/1c14129f07a236b3/EnDMZWSGyK5MmhGCLFtdzc4BhbyHUVj5mAYlc0klYgUVXQ)

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
1. Download the Excel File: [Bike-share dashboard.xlsx](https://1drv.ms/f/c/1c14129f07a236b3/EnDMZWSGyK5MmhGCLFtdzc4BhbyHUVj5mAYlc0klYgUVXQ)
2. Open the Excel File using Microsoft Excel.
2. Navigate to the Dashboard Sheet


![Dashboard](https://github.com/user-attachments/assets/915d1cd3-76cd-432a-b00f-efa8e55b5bd2)

### Key Features of the Dashboard

- **Interactive Charts**:
  - Slicers are used to filter data by different categories. In the bar chart and the line chart slicers are used to analyze bikers' behaviors based on membership type. Another slicer is used in the pie chart to filter data based on months.

- **Trend Analysis**:
  - Heatmap shows riders' density throughout months. During the months of June, July, and August numbers of bikers increase noticeably.
  - The bar chart shows the number of riders on each day of the week for each membership type. Casual members tend to bike more than usual on Saturdays and Sundays.
  - The line chart shows when each membership type tends to bike in days' hours. There is an obvious increase in 8 a.m. and 5 p.m. for members.
  - The pie chart shows the percentage of each membership for every month.
 
### Analysis

- After August, the percentage of members numbers started to increase after continuously decreasing from the beginning of the year. This can be interpreted in **two** possible ways. Firstly, since the realization that both memberships were more active between June to August, which is spring, we can assume that bikers became more willing to purchase a member membership after enjoying biking in spring. Secondly, it is not the percentage of members numbers that has increased, but rather the percentage of casual memberships number that has decreased, again, because spring was starting to end, which, in my opinion, sounds more convenient and sentimental.
- Building on the previous point, and since mere intuition can't play a role in making analytical insight, I conducted further investigation trying to figure out if anything specific took place to increase members' percentage. Usually, I would head to the marketing department and make an acquisition about any marketing strategy that might've taken place, if so, I would analyze it using A/B testing and figure out if it might be effective for further usage.
- From analyzing two facts, that, clearly, more members tend to bike at 8 a.m. and at 5 p.m., and casuals tend to bike more on Saturdays and Sundays -the weekends-, it becomes obvious that, usually, members use bikes for commuting, and casuals use bikes for leisure, hobby, or sports.
- I analyzed trends in the numbers and the percentages of each membership over months to notice if there is any sudden increase of subscriptions of a membership against a sudden drop in the other membership, that might indicate that the increase of subscriptions is due to members conversion from membership to another rather than new memberships, to conduct further analysis. To have a general idea I used a scatter plot to see if any point is far from the supposed correlation line. I also used `=CORREL` function, it was `0.92`; the positive correlation is strong. No significant increase and decrease has been spotted. After calculating the mean, standard deviation, and monthly change of each membership -using the formula `monthly change = (current month percentage - previous month percentage ) / previous month percentage`- I found a data point from the percentages of differences that has a z-score of 2.17 in casual membership, which is considered high, but the corresponding data point from the member membership has a z-score of 1.17; nothing significant.
 
  ![Per  of Diff](https://github.com/user-attachments/assets/441c596b-bff0-407b-a7a7-373ed832751f)


### Recommendations

Based On the analysis, I recommend the following actions:

- Include an extra membership, either a monthly membership or a seasonal membership, to allow some casual members to bike seasonally.
- Build a system that collects data about the exact number of new members, converted members, and canceled members.
- Collect more data about characteristics of each memberships users.
- Use social media to influence the audience about the beneficiality and importance of biking.
