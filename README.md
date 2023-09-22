# Data-Analysis-Bellabeat
Data insights for Bellbeat app
Goal of the project
The purpose of this analysis project is searching for user patterns of usage of their smart devices in order to gain insights that would later better orientate marketing decisions and unlock new growth opportunities for Bellabeat. So, main business objectives are:

How do our users use smart devices?
Identify trends in how consumers use non Bellabeat smart devices to apply insights into Bellabeat’s marketing strategy.
The analysis of fitbit tracking data and visulation of results are done using Python libraries.

Data Processing
Data will get processed and cleaned with the help of python libraries:

Correctly format columns name and types
Checking irrelevant columns and subsetting dataset
Check for duplicate rows and missing values
Analysis Approach
Category analysis will done by creating two categorization of the users, by level of physical activity and device usage.

physical activity would follow these arguments:

Sedentary: less than 6000 daily steps on average
Active: between 6000 and 12000 daily steps on average
Very active: more than 12000 daily steps on average
Device usage will follow these arguments:

Low use: less than 8 hours of use per day.
Normal use: between 8 and 16 hours of use per day.
High use: more than 16 hours of use per day.
Visualization
Correlation between total steps and calories

img1 = plt.imread('steps and calories.png')
     

plt.imshow(img1)
     
<matplotlib.image.AxesImage at 0x7f93d83c5570>


We can see in this scatterplot a somewhat positive correlation, the more steps done, the more calories burnt. Also we divided the dots by colors, using the activity_level category, so we can see which group is representing the data shown.

Average number of steps per day

img2 = plt.imread('Avg_steps_per_day.jpg')
     

plt.imshow(img2)
     
<matplotlib.image.AxesImage at 0x7f93a4b3a800>


The results show that Monday, Tuesday and Saturday are the days where the users were more physically active and above the average numbert of steps overall. Wednesday, Thursday, and Friday are below the average but the three fell into the same area. Sunday is the least active of all the weekdays.

With this information we can interpret that users tend to be more physically active during the firsts days of the week and during saturdays, giving us a hint of the activities they may do.

Percentage of activity in minutes

img3 = plt.imread('activity level in mintues.png')
     

plt.imshow(img3)
     
<matplotlib.image.AxesImage at 0x7f93a4baff40>


This pie chart shows that the users are in a sedentary state of activity most of the time, a sixth of the time doing light activity and only 2% of the time being active doing proper excercise.

Correlation Between activity level minutes and calories

img4 = plt.imread('avtivity minutes and calories.png')
     

plt.imshow(img4)
     
<matplotlib.image.AxesImage at 0x7f93a3b35b40>


Figue [0,0] shows there is no specific relation between burned calories with time in sedentary.
Figue [0,1] shows positive correlation, for very active person, more time spend on light activity the more calories are burned.
Figue [1,0] shows there is no specific relation between burned calories with fairly activity time.
Figue [1,1] shows positive correlation, for very active person, more time spend on large scale activity the more calories are burned.
Useful Insights
After analyzing FitBit Fitness Tracker Data, following are the insights that would help influence Bellabeat marketing strategy

A multipurpose device
Bellabeat can let know users, that their products are not only meant for sports, or excersice related activities As the data show, many users spend more time wearing the tracking device on weekends than on weekdays, this could mean that they relate the product just to sports or for only the usual walking to the park on sundays Bellabeat can show that their products are meant to acompany them wherever they go for any daily activities, such as work And help them track information to improve overall fitness and health This will encourage women from diverse demographic features and backgrounds to use Bellabeat's product meant for all women who care about overall health

Rewards and reminds
Bellabeat can integrate functions within the bellabeat app or other products, such as rewards or incentives, and reminds to encourage their users to hit certain marks These marks could be achieving the minimum amount of 7 500 steps per day, certain calorie burning for people who want to lose weight, or the 8 hour sleep pattern Certain rewards could be showing a leaderboard of top users who have reached and maintained the minimum steps a day for longer, virtual medals or prizes, such as discounts or offers For the reminds part, Bellabeat could send notifications to their users when they are lagging behind in such goals, and also it could offer recomendations to their users to help them with their sleep, or achieving their goals

Datasets Used
The datasets used:

Comes with 904 rows with 903 being pure data and the other one row being the column headers.
The FitBit Fitness Tracker Data is stored in Kaggle and was made available through Mobius and generated by respondents to a distributed survey via Amazon Mechanical Turk between 03.12.2016 05.12.2016. Accesible through Kaggle here
It contains the data of 33 users.



# Data Analytics Customer Segmentation

## Goal of the project
The goal of this project is to conduct a Customer Segmentation Analysis for an Automobile bike Company. Customer segmentation is performed by developing an RFM Model. RFM (Recency, Frequency, Monetary) analysis is a behavior-based approach grouping customers into segments. It groups the customers on the basis of their previous purchase transactions. In this analysis, the customer segment was divided into 11 groups. The analysis will help in determining which customer segments should be targeted in order to enhance sales revenue for the company. A **Sales Dashboard for Customer Segmentation** is developed using **Tableau** and the data quality assessment and analysis is done using **Python**.

## Tableau Dashboard
The Sales Dashboard for Customer Segmentation can be found [here](https://public.tableau.com/app/profile/chirag.arya4385/viz/Customersegmentationdashboard_16941047002960/SalesDashboard).

![Tableau Dashboard](media_files/Customer%20Segmentation%20Dashboard.png)

**In case of failure of loading Jupyter Notebooks on Github, the following notebooks can be found in the nb viewer. Click on the respective hyperlinks to view:**

+ [Data_cleaning_customer_address.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/Data_cleaning_customer_address.ipynb)
+ [Data_cleaning_customer_demographic.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/Data_cleaning_customer_demographic.ipynb)
+ [Data_cleaning_new_customer_list.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/Data_cleaning_new_customer_list.ipynb)
+ [Data_cleaning_transactions.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/Data_cleaning_transactions.ipynb)
+ [RFM_analysis.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/RFM_analysis.ipynb)

## Analysis Approach

### 1. Data Quality Assessment and Data Cleaning
The first step towards generating useful insights from the data was the data preparation, quality assessment, and data cleaning step. After the cleaning process, exploratory data analysis on the dataset and identification of customer purchasing behaviors to generate insights can be performed.

In the data cleaning step, the data quality of the following datasets was first assessed. After a data quality assessment, the following data quality issues were observed and the necessary process to mitigate the issue was followed :

+ **CustomerDemographics.xlsx :**
  + 1 Irrelevant column was present and such columns were dropped from the dataset.
  + There were 5 columns where Missing values were present. For such columns based on the volume of the missing values either the records were dropped or appropriate values were imputed at places of missing values.
  + For the gender column, there was no standardization of data. Based on the values available the column data was standardized to remove data inconsistency.
  + The Date of Birth column was transformed to create a new feature column 'Age' and 'Age Group' to check for discrepancies in age distribution. An outlier was observed and the record was removed.
  + Checked whether there are duplicate records present in the dataset. In this dataset, there were no duplicate records.
  
+ **NewCustomerList.xlsx :**
  + 5 Irrelevant column was present and such columns were dropped from the dataset.
  + There were 4 columns where Missing values were present. For such columns based on the volume of the missing values either the records were dropped or appropriate values were imputed at places of missing values.
  + The Date of Birth column was transformed to create a new feature column 'Age' and 'Age Group' to check for discrepancies in age distribution.
  + There was no data inconsistency.
  + Checked whether there are duplicate records present in the dataset. In this dataset, there were no duplicate records.
  
+ **Transaction_data.xlsx :**
  + The product_first_sold_date column is not in datetime format. The data type of this column was changed from int64 to datetime format.
  + There were 7 columns where Missing values were present. For such columns based on the volume of the missing values either the records were dropped or appropriate values were imputed at places of missing values.
  + A new feature column 'Profit' was created which is basically the difference between the list price and the standard price.
  + There was no data inconsistency.
  + Checked whether there are duplicate records present in the dataset. In this dataset, there were no duplicate records.

+ **CustomerAddress.xlsx :**
  + For the states column, there was no standardization of data. Based on the values available the column data was standardized to remove data inconsistency.
  + There were certain customer IDs from the Customer Demographics table that were getting dropped in the Address table.
  
### 2. Exploratory Data Analysis on Customer Segments
After the data cleaning process, exploratory analysis of the dataset is performed and the following insights are obtained :
+ New vs. Old Customers Age Distribution
  + Most New customers are aged between 40-49 also for Old Customers most of them are aged between 40-49.
  + The lowest number of customers for both types of customers is present in the age bracket under 30 and above 70 age groups.
  + The automobile company is popular among New Customers between the age of 40-70.
  + A steep drop in customers is observed in the 30-39 age group among the New Customers.

| Old Customers by Age Distribution | New Customers by Age Distribution |
| :------------- | :------------- |
|![](media_files/Old%20Customers%20Age%20Distribution.png)|![](media_files/New%20Customers%20Age%20Distribution.png)|

+ Bike purchases over the last 3 years by Gender
  + Most bike purchases have been done by Females over the last 3 years. Approximately 51% of the bike purchases are done by Females compared to 49% of the purchases being done by Males.
  + The Female purchases are 10,000 more than that of Male purchases (numerically).
  
![](media_files/Gender%20based%20Bike%20Purchases.png)

+ New vs. Old Customers Job Industry Distribution
  + Most New customers are from the Manufacturing and Financial Services sector (approx 20% of the New Customers).
  + The lowest number of customers are from the Agriculture and Telecom sector approx 3%.
  + A similar trend is observed among Old Customers as well.

| Old Customers by Job Industry | New Customers by Job Industry |
| :------------- | :------------- |
|![](media_files/Old%20Customers%20Job%20Industry.png)|![](media_files/New%20Customers%20Job%20Industry.png)|

+ Wealth Segmentation by Age Category
  + Across all age categories, the largest number of customers are from the 'Mass Customer' Segment.
  + The next category comes from the 'High Net Worth' customers.
  + In the age group 40-49, the Affluent segment outperforms the high-worth customers in terms of number of customers despite old or new customers.

| Old Customers Wealth by Age Group | New Customers Wealth by Age Group |
| :------------- | :------------- |
|![](media_files/Old%20Customers%20Wealth%20Segment.png)|![](media_files/New%20Customers%20Wealth%20Segment.png)|

+ Cars owned by States
  + New South Wales has the largest number of people who don't own a car.
  + In Victoria and Queensland the proportion is quite even.
  + In New South Wales the number of people owning a car is significantly lesser than those who do not have a car.

![](media_files/Car%20Owners%20by%20State.png)

### 1. Customer Segmentation and RFM Analysis
In this stage of analysis, the customer segmentation was done by developing an RFM Model. The RFM (Recency, Frequency, Monetary) analysis is a behavior-based approach grouping customers into segments. It groups the customers on the basis of their previous purchase transactions.

In this analysis, the customer segment was divided into 11 groups. The groups are:

+ Platinum Customers
+ Very Loyal Customers
+ Recent Customers
+ Potential Customers
+ Lost Customers
+ Losing Customers
+ Late Bloomer
+ High Risk Customers
+ Evasive Customers
+ Becoming Loyal
+ Almost lost Customers

As of the current state of the Automobile business the distribution of customer segments is depicted below:
![](media_files/Customer%20Segment%20Distribution.png)

+ Recency and Frequency vs. Monetary Distribution
  + Customers who purchased recently generated more revenue than customers who visited a long time ago.
  + Customers classified as "Platinum Custoers", "Very Loyal" and "Becoming Loyal" visit frequently.

| Recency vs Monetary | Frequency vs Monetary |
| :------------- | :------------- |
| ![](media_files/Recency%20vs%20Monetary.png) | ![](media_files/Frequency%20vs%20Monetary.png) |


## Datasets Used
The datasets used include:
+ **FitBit Fitness Tracker Data:** The archived file downloaded from the following [link](https://www.kaggle.com/datasets/arashnic/fitbit?resource=download) includes following files. 
  + **dailyActivity_merged.csv:** This dataset included the transaction data of the customers across all the different states in Australia.
  + **NewCustomerList.xlsx:** This dataset included the new customers who visited the automobile bike company recently.
  + **CustomerDemographic.xlsx:** This dataset included entire details of the Customer Demographics.
  + **CustomerAddress.xlsx:** This dataset included the address of the Customers.
  
## Tools and Technologies Used
The tools used in this project include:
+ **Python** - This was needed to conduct Data Quality Assessment and also for Data Cleaning processes. With Python libraries **pandas, numpy, matplotlib, seaborn, datetime** exploratory data analysis of the datasets and gaining useful insights from the data was possible.

## Built With
+ Python 3.10.11, Google Colab

## Authors
+ Chirag Arya - [Github Profile](https://github.com/AryaChirag)
