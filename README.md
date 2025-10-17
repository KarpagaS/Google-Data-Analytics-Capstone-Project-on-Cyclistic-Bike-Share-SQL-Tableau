# Google-Data-Analytics-Capstone-Project-on-Cyclistic-Bike-Share-SQL-Tableau
Google Data Analytics Capstone Project on Cyclistic Bike Share

**Project Quick Summary
I'll be acting as a junior data analyst at Cyclistic, a fictional company.

I'll encounter various characters and team members throughout the study.

My goal is to address critical business questions by following the data analysis process: ask, prepare, process, analyze, share, and act.

Tools used: MySQL, Tableau.

**Project Introduction**

Scenario

I am a junior data analyst at Cyclistic in the marketing analyst team.

The director of marketing thinks annual memberships are crucial for the company's success.

My team's goal is to analyze how casual riders and annual members use Cyclistic bikes differently.

We aim to use these insights to create a strategy for converting casual riders into annual members.


Our recommendations need approval from Cyclistic executives and require strong data insights and professional data visualizations.

**Characters and teams**

Cyclistic is a bike-share program that features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can't use a standard two-wheeled bike. The majority of riders opt for traditional bikes; about 8% of riders use the assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to work each day.

The Cyclistic marketing analytics team is a group of data analysts who are responsible for collecting, analyzing, and reporting data that helps guide Cyclistic marketing strategy. As a paart of the team and learning about Cyclistic's mission and business goals — as well as how I, as a junior data analyst, can help Cyclistic achieve them.


**Project Kickoff**

**Ask Phase**: Business Questions & Key Stakeholders

Three questions will guide the future marketing program:

How do annual members and casual riders use Cyclistic bikes differently?

Why would casual riders buy Cyclistic annual memberships?

How can Cyclistic use digital media to influence casual riders to become members?

**Prepare Phase:**

Data Gathering & EDA Report

Data Gathering

I plan to utilize Cyclistic's archived trip information to conduct an analysis and detect patterns. This data can be obtained through the (https://divvy-tripdata.s3.amazonaws.com/index.html) source, with permission granted by Motivate International Inc. pursuant to their licensing agreement.

Note - This is public data that you can use to explore how different customer types are using Cyclistic bikes. But note that data-privacy issues prohibit you from using riders’ personally identifiable information. This means that you won’t be able to connect pass purchases to credit card numbers to determine if casual riders live in the Cyclistic service area or if they have purchased multiple single passes.

**Concerned Source Data**

Data Timeframe: June 2022 to May 2023 (Past 1 year data)

Source Data Description and Structure:

The data is organized into individual .csv files, each corresponding to a specific month.
These files share common fields relevant to our analysis.

After our initial examination, we can confidently assert that the source data is Reliable, Original, Comprehensive, Current and Cited.

**Tool Selection for Analysis**

**Tool for Data Cleaning, Transformation, and Processing: SQL**

We chose SQL for these tasks because the dataset exceeded 5.8 million rows, making it impractical to manage with Excel (which is typically suitable for datasets of less than 1 million rows). SQL's capacity to handle large volumes of data makes it the preferred choice for data wrangling.

**Tool for Analysis and Visualization: Tableau**

While there are several tools available for data visualization, including Excel and Power BI, our selection of Tableau is deliberate. Tableau offers dynamic capabilities and a diverse range of visualization options, making it the ideal choice for our analytical and visualization needs.

**Data Loading**

File Naming Convention: Files are named in the format of YYYYMM-divvy.csv.

Data Integration into 'combined_Table': The data has been uploaded and consolidated into a unified table named 'combined_Table'. (To see the process of data upload and consolidation into a single table, please click here.)

**Data Observation**
Data Observation SQL Queries

**Size of Data (Rows & Column)**

There are 5829030 no of rows and 13 no of columns observed in 'combined_Table' table

**Data types of all columns in combined_table**


**All Null and Blank values in combined_table**

No of Null Values in each columns


No of Blank Values in each columns


**Total no of blank or null values in combined_Table table**


**Percentage of Blank Values in each columns**


Total Percentage of Blank Values

**Checking Duplicates in combined_Table**
Count of total duplicate rows
2 5 2 Count of total duplicate rows

**Checking outlier or false data in combined_Table**
Outlier or false value in ride length (ended_at - started_at)
Longer than a day


Less than a minute


Total count and percent of inconsistent values
Total inconsistent values count
Total count of rows including 'Total no of blank or null values', 'Outlier or false value of ride length longer than a day' and 'Outlier or false value of ride length less than a minute'.


Total inconsistent values percentage
Percent of rows including 'Total no of blank or null values', 'Outlier or false value of ride length longer than a day' and 'Outlier or false value of ride length less than a minute'.


Field specific observations of 'combined_Table' table
Characteristics and data format of field 'ride_id'
Data type: VARCHAR(255)

Constraints applied:

Primary Key
Unique
Not Null
Primary Key constraints added in this field

Length of field:


Characteristics and data format of Field 'rideable_type'
Data type: MEDIUMTEXT
Data format: Categorical
All Categories:

Characteristics and data format of Field 'started_at' & 'ended_at'
Data type: DATETIME -- (YYYY-MM-DD hh:mm:ss)
Characteristics and data format of Field 'start_station_name', 'end_station_name', 'start_station_id' & 'end_station_id
Data type: MEDIUMTEXT
Blank values were found in all four columns.
Characteristics and data format of Field 'start_lat', 'start_lng', 'end_lat' & 'end_lng'
Data type: Double
Blank values were found in 'end_lat' & 'end_lng' columns
Characteristics and data format of Field 'member_casual'
Data type: MEDIUMTEXT
Data format: Categorical
All Categories:
Pasted image 20230728152823
Process Phase: Data Cleaning & Transformation Report
Data Cleaning
Data Cleaning & Transformation SQL Queries

Rows with missing values are removed.
We excluded trips that were too short (less than a minute) or too long (more than a day).
A total of 1426785 rows were deleted.
Data Transformation
Created new Columns:
ride_length
month
day_of_week
hour_in_day.
Analyze, Share & Act Phase: Cyclistic Bike Share Analysis Report
The data has been tidied and formatted for analysis.
I loaded it into Tableau Public and used it to create charts and graphs to visualize the data.
I then created a Story in Tableau to share the insights I gained from the data.
Tableau Story Link: Cyclistic Bike Share Analysis | June 22 to May 23




