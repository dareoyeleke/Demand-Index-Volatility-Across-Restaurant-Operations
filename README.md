# 📊 Demand Volatility in the Hospitality Industry
## A Data-Driven Analysis of Operational Risk and Customer Behavior
### 🔍 Project Overview

This project analyzes demand volatility across restaurant operations to identify the structural drivers behind unstable revenue patterns. Rather than focusing on revenue levels alone, the analysis examines how and when volatility occurs, enabling more informed operational and staffing decisions.

Using transactional data, the project evaluates how restaurant type, time patterns, and environmental conditions influence fluctuations in demand.

### How to read this project 

OBJECTIVES ---> KEY QUESTIONS ADDRESSED ---> METHODOLOGY ---> DASHBOARD AND VISUAL OVERVIEW AND INSIGHTS ---> KEY FINDINGS ---> RECOMMENDATIONS ---> LIMITATIONS. 

### LASTLY 
-  Reproducing the project comes last with the 1) Dataset 2) Required tools 3) Methodology 4) CSV's generated 5) Steps to Reproduce

### 🎯 Objectives

-  Quantify demand volatility across restaurant formats

-  Identify temporal drivers (weekday vs weekend effects)

-  Assess the impact of external stressors (weather, promotions, events)

-  Translate analytical findings into operational insights

### Data Set Acquired From 
- 🔗 https://www.kaggle.com/datasets/farukalam/yelp-restaurant-reviews

### 🧠 Key Questions Addressed

-  Which restaurant types experience the highest demand volatility?

-  Do weekends materially increase volatility?

-  Are promotions effective in driving demand?

-  What operational factors contribute most to instability?

-  How does weather (Stressful (Rain) VS Normal weather) influence Demand? 

### 🧪 Methodology
-  Data was imported in csv format and data was cleaned by normalizing dates to a more accesible format, needed columns were also renamed for easier access in regards to less typing

-  RVI (Revenue Volatility Index) was calculated as a Scaler Comparison from Mininmum to Maximum, using the absolute value of the percentage change in revenue as a rolling value over the period of 3 months and 2 where 3 wasn't applicable per location

-  Promotion and risk patterns were segmented into low, medium and high tiers using percentiles and quartiles respectively. Risk explanations are forecasted as a combination of promotion and risk patterns. Risk patterns are based on RVI

-  Weather, restaurant and restaurant statistical spreads are calculated in regard to RVI

-  Time bound Volatility i.e, day of week, weekday vs weekend, was calculated on a day to day basis with absolute values of revenue percent change by the day and adjusted to weekday vs weekend groups as well as compared by restaurant types

## 📊 Dashboard Overview

<img width="1920" height="1079" alt="VOLATILITY SNAP 1" src="https://github.com/user-attachments/assets/39d82ba7-6e98-42fe-aeb7-9fee6e1800a7" />

### 1️⃣ Executive Summary Dashboard

-  High-level overview of volatility across the business.

**Key Takeaways Based on the Average**

-  Average volatility differs meaningfully across restaurant types

-  Weekends show significantly higher volatility than weekdays

-  Across all restaurant types as a whole, demand Volatility is relatively high

### 2️⃣ Volatility by Restaurant Type also According to Dashboard

**Understanding structural demand differences.**

**Insights by Average**
- Cafe's show the highest Volatity

- Kopitiam Locations show the lowest Volatility

- Kopitiam Locations show the most stable average Demand

### 3️⃣ Time-Based Volatility Analysis

<img width="1920" height="1078" alt="VOLATILITY SNAP 2" src="https://github.com/user-attachments/assets/fe12bf68-506f-423d-8b70-86dfa3622052" />


**How demand changes across days and weeks.**

**Insights**

-  With the exception of Fine Dining and Kopitiam locations which show opposing trends, Weekend demand is significantly more volatile

-  Seasonal effects are present but secondary to behavioral patterns

-  Huge change in Volatility for august and then Sharp fall for September signalling end of summer and beginning of school period signalling less family and student traffic

-  Huge Difference in Volatility from End of year Holiday Season and January as Families contribute to demand in December, and then individuals follow trends such as Dry January leading to a High change in Volatility 

### 4️⃣ Volatility Distribution & Risk Profiles
<img width="1920" height="1079" alt="VOLATILITY SNAP 3" src="https://github.com/user-attachments/assets/8f04447e-b36a-4a96-8e45-f623905a2647" />

-  Comparing dispersion and risk across restaurant types.

**Insights**
-  Promotional activity has limited stabilizing impact, as low promotion dominates across promotion segment for all risk factors showing most demand is organic and mostly generally stable with peak period sensitivity and is not strongly driven by promotion sitting at a 0.26 on the RVI. This highly takes into consideration that low promotion dominates across all risk sections.   
  
-  Volatility clusters around behavioral, not promotional, factors

-  Casual Dining and food stalls show the highest skews from the mean i.e Standard deviation(std) from the mean at a 0.19 std on the RVI with Casual dining having a max RVi of 1 as opposed to Food Stalls at 0.91 std i.e  Both aresensitive to experiential demand. Casual Dining locations are the average person's go to, therefore having the most amount of skews in regards to traffic. Holiday periods affect Casual dinings the most as most families especially with kids and older populations cater to casual dining. Food stalls may see sharp increase in demand due to concerts, fairs and then have limited traffic once concentrated visits due to events are over with.

-  Kopitiam exhibit the most stable patterns showing a standard deviation of 0.08 from the mean on the RVI with a 0.32 max. Kopitiam is a niche restaurant format, signalling acquired taste or regulars who seek out specific profiles of coffee. Social media Trends or such can influence attention around Kopitiam and affect volatility. Hence having the least amount of skew from the average. 

-  Cafés and Fine Dining sit in the middle range of skews from the average with 0.15 and 0.16 deviation from the mean respectively, both close to Casual dining and Food stalls, but also Cafe's and Fine Dining stay in the mid range by balancing out with their max on the RVI scale of 0.73 max for Cafe's and 0.79 max for Fine Dining on the RVI. While fine dining exceeds cafe in skew, cafe's have increased presence of regulars, people looking to study, or grab coffee on the way to work and therefore contribute to regular predictable traffic. Fine dining serves the less popular crowds, with more money to spend per visit, or celebrating special occasions, and also in most cases requiring reservations, in a way have controlled traffic. 

5️⃣ Executive Summary & Recommendations

<img width="1920" height="1080" alt="VOLATILITY SNAP4" src="https://github.com/user-attachments/assets/e20c7651-9856-4bf9-8bf5-c88a7c3870b2" />



**Translating data into decisions.**

**Key Findings**

-  Demand volatility is structurally driven, not random

-  Weekends and Holiday Periods amplify volatility across all restaurant types

-  Promotions do not meaningfully stabilize demand

-  Operational design matters more than pricing tactics

**Recommendations**

-  Increase staffing flexibility during peak volatility windows, especially to casual dining locations - We do this by allowing more flexibility in schedule by having more employees on call during weekends shown to have about 33% volatility increase compared to weekdays, and holiday periods during the summer and years end which have about 20% and 40% differences respectivelly to combat unstable traffic and reduce wait times among customers to maintain consistently remarkable  experience among customers 

-  Focus on operational consistency rather than discounting - To do this we need to ensure service, especially commendable service is delivered across the board by every employee, by implimenting extra training to bridge the gap where needed between employees 

-  Monitor high-risk formats with proactive forecasting - Apart from implimenting on call shifts to match unpredictable traffic. Implimenting secret shoppers to evaluate service, encouraging customer reviews on visit days to guage experience by the day and having spot checks by managers on duty will help bridge the gap and take notice of operational factors that lead to inconsistencies in Revenue

### Limitations 

-  Figures such as labor percentages i.e employees on shift per daily and hourly revenue, amd which specific are employees scheduled on specific days, as well as having customers leave reviews on days of visit would help establish correlation that contribute to focusing efforts where needed to improve Operational Conditions.
-  As there were no recorded events, it was impossible to ascertain the effects of events in isolation or combination with other factors on Volatilty, which could potentially be a stressor for volatility change 

<img width="1920" height="1080" alt="VOLATILITY SNAP 5" src="https://github.com/user-attachments/assets/0c8765a9-5755-444a-b808-41c844b4229b" />


**Data Source: Public restaurant transaction dataset**

## Tools Used: Python (Pandas) 🐍, Power BI 📈 📐

### Metrics Created:

-  Average of Revenue Volatility Index Ranges (Highest and Lowest) 

-  Time-based segmentation (weekday/weekend)

-  Restaurant-type segmentation

**Approach: Descriptive analytics with behavioral interpretation**

### 🧩 Key Takeaway

-  Demand volatility is not random — it is driven by structural and behavioral factors.
-  Understanding when and why volatility occurs enables smarter operational planning than reactive pricing strategies.

### 🛠 Tech Stack

-  Python (Pandas, NumPy) 🐍

-  Power BI (DAX, data modeling, dashboards) 📈 📐

-  Excel (validation & QA) 🔢

-  GitHub (version control & documentation)


## ⚙️ How to Reproduce
### Requirements

-  Kaggle Account to access Data set 

-  Data set access Link [https://www.kaggle.com/datasets/farukalam/yelp-restaurant-reviews] exported as zip file and loaded into Jupyter Notebook as csv

-  Jupyter Notebook
  
-  Power Bi To run CSV files

## Steps

-  Kaggle Account is needed to access and download source file [https://www.kaggle.com/datasets/farukalam/yelp-restaurant-reviews]

-  Data set access Link [https://www.kaggle.com/datasets/farukalam/yelp-restaurant-reviews] exported as zip file and loaded into Jupyter Notebook as csv. 

-  Access Python Script -Restaurant_Demand_Index_Volatility.ipynb- at 🔗 [https://github.com/dareoyeleke/Demand-Index-Volatility-Across-Restaurant-Operations/blob/main/Restaurant_Demand_Index_Volatility.ipynb]

-  Refer to Methodology at the top of page to follow steps taking to clean and aggregate data. 

-  Run Queries to generate Data

- **The following CSV's were generated to create the Dashboard and Visuals** 
    - restaurant_type_volatility.csv to generate "Average Volatility for each restaurant type" in Visual 1 
    - monthly_sales.csv to generate "Average Revenue Volatility Across All Restaurants" and "Max Revenue Volatility for all Restaurants" KPI cards in Visual 1 as well as "What is the Average Revenue Volatility by the Month" in Visual 2
    - restaurant_type_volatility.csv to generate both Highest and Lowest AVG Volatility KPI cards for each restaurant type in Visual 1
    - daytype_volatility.csv to generate AVG weekday and weekend Volatility KPI cards as well as comparison chart for AVG weekday vs weeekend Volatility Chart in Visual 1
    - daily_revenue.csv to generate "Daily Revenue Volatility by Restaurant" Matrix Visual in Visual 3
    - weather_volatility.csv to generate weather volatilty by reported incidents visual in Visual 3
    - restaurant_volatility.csv to generate "Statistical Values for Volatility Across Restaurant Type" in Visual 4
    - location_risk.csv to generate Risk Explanation Matrix in Visual 4 

-  CSV's from generated data can be loaded into PowerBI from Visual and Dashboard Creation

-  Explore queries and modify filters for deeper analysis

### 📎 Author

[Dare Oyeleke]
Data Analyst | Healthcare Analytics
[(https://www.linkedin.com/in/dareoyeleke/)] | [(https://github.com/dareoyeleke)]
