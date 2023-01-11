# Table of Contents

* [Introduction](#introduction)
    * [Scope of Work](#scope-of-work)
    * [Case Background](#case-background)
        * [Scenario](#scenario)
        * [About the Company](#about-the-company)
        * [Key Stakeholders](#key-stakeholders)
* [Ask](#ask)
    * [Key Tasks](#ask-key-tasks)
    * [Guiding Questions](#ask-guiding-questions)
    * [Deliverable](#ask-deliverable)
* [Prepare](#prepare)
    * [Key Tasks](#prepare-key-tasks)
    * [Guiding Questions](#prepare-guiding-questions)
    * [Deliverable](#prepare-deliverable)
* [Process](#process)
    * [Key Tasks](#process-key-tasks)
    * [Guiding Questions](#process-guiding-questions)
    * [Deliverable](#process-deliverable)
    * [Process Code](#process-code)
        * [Setting up the Space](#process-setting-up-the-space)
        * [Data Cleaning](#process-data-cleaning)
* [Analyze](#analyze)
    * [Key Tasks](#analyze-key-tasks)
    * [Guiding Questions](#analyze-guiding-questions)
    * [Deliverable](#analyze-deliverable)
    * [Analyze Code](#analyze-code)
        * [Analysis Layout](#analyze-code-analysis-layout)
        * [Monthly & Weekly Trends](#analyze-code-monthly-weekly-trends)
        * [Weekday Trends](#analyze-code-weekday-trends)
        * [Start Hour Trends](#analyze-code-start-hour-trends)
        * [Rideable Type Trends](#analyze-code-rideable-type-trends)
        * [Start and End Station Trends](#analyze-code-start-and-end-station-trends)
* [Share](#share)
    * [Key Tasks](#share-key-tasks)
    * [Guiding Questions](#share-guiding-questions)
    * [Deliverable](#share-deliverable)
* [Act](#act)
    * [Key Tasks](#act-key-tasks)
    * [Guiding Questions](#act-guiding-questions)
    * [Deliverable](#act-deliverable)
* [Conclusion](#conclusion)



<a id="introduction"></a>
# Introduction
​
This is my case study for the Google Data Analytics Capstone Project - Cyclistic Bike-Share. The link to the original case study document can be found on the [Google Data Analytics Professional Certificate](https://www.coursera.org/learn/google-data-analytics-capstone/home/) site. 
​
The case study will follow the steps of the data analysis process: ask, prepare, process, analyze, share, and act. Each phase will have a deliverable and will be follow a set of key tasks and guided questions with answers.
​
<a id="scope-of-work"></a>
#### Scope of Work
1. Ask: discuss and define the project
   * Deliverables: Problem statement, define goals and expectations
​
​
2. Prepare: extract and prepare data for analysis
    * Deliverable: description of data sources used
  
  
3. Process: process data for analysis
    * Deliverable: changelog of cleaning or manipulation of data
    
    
4. Analyze: data exploration, analysis, and visualization
    * Deliverable: summary of my analysis
    
    
5. Share: communicate insights and results
    * Devliverable: supporting visualizations and key insights
    
    
6. Act: make data driven recommendations
    * Deliverable: top three recommendations based on my analysis 
​
<a id="case-background"></a>
### Case Background
<a id="scenario"></a>
#### Scenario

As a Junior Analyst on the Marketing Analyst Team at Cyclistic ("The Company") - a Chicago based bike share company, the Director of Marketing tasked me with understanding how casual riders and annual members use The Company's bikes differently. The analysis will produce actionable insights and provide support for recommendations for a marketing strategy to convert casual riders into annual members. 
<a id="about-the-company"></a>
#### About The Company
* Fleet consists of 5,824 geotracked bicycles
* There are 692 stations across Chicago; bikes can be unlocked from one station and returned at another
* Pricing plans include: single-ride passes, full-day passes, and annual memberships
   * Customers who purchase single-ride or full-day passes are referred to as **casual riders**
   * Customers who purchase annual memberships are **Cyclistic members**
* Annual members are more profitable than casual riders
* Marketing Director Lily Moreno believes that future growth of The Company is predicated on converting casual riders to annual members. She also believes that casual riders have chosen Cyclistic for their mobility needs
* In order to implement strategies to encourage casual to member conversion, the marketing team needs to understand the following: 
  1. How annual members and casual riders differ
  2. Why casual riders would buy an annual membership
  3. How digital media could affect their marketing tactics

<a id="key-stakeholders"></a>
#### Key Stakeholders
* **Cyclistic Executive Team**
    * Expectation: clear, concise insights to drive data-driven decisino making
    * Goal: deploy strategic marketing initiative to increase profitability
    
    
* **Lily Moreno, Director of Marketing**
    * Expectation: data analysis to support strategy
    * Goal: convert casual riders into annual members
    
     
* **Marketing analytics team**
    * Expectation: conduct data analysis on historical to understand difference between casual riders and annual members
    * Goal: extract data insights to inform decision making



<a id="ask"></a>
# Ask
<a id="ask-key-tasks"></a>
#### Key Tasks
1. [x] **Identify the business task**  
2. [x] **Consider key stakeholders** 

<a id="ask-guiding-questions"></a>
#### Guiding Questions
* **What is the problem you are trying to solve?**

The marketing analyst team is looking to understand the differences between Cyclistic's user base (annual members and casual riders) to determine the best marketing strategy to encourage casual to member conversion.
* **How can your insights drive business decisions?**

My insights should support the Director of Marketing's theory when presenting the recommendations to the Executive Team.

<a id="ask-deliverable"></a>
#### Deliverable

**Problem statement:** We need to clearly identify the differences in use behaviors between casual Cyclistic riders and Cyclistic members to formulate a marketing campaign aimed at converting casual riders into members in an effort to maximize annual memberships and drive profitability growth.



<a id="prepare"></a>
# Prepare
<a id="prepare-key-tasks"></a>
#### Key Tasks
1. [x] **Download data and store it appropriately**
2. [x] **Identify how it’s organized.**
3. [x] **Sort and filter the data.**
4. [x] **Determine the credibility of the data.**
<a id="prepare-guiding-questions"></a>
#### Guiding Questions
* **Where is your data located?**

Data is located on Kaggle
* **How is the data organized?**

Monthly data from April 2020 to March 2021 is split into .csv files
* **Are there issues with bias or credibility in this data? Does your data ROCCC?**

The data is automatically collected through The Company's fleet of bikes and stations, so there should be little to no bias on the data collection front. Data appears to be reliable, original, and cited. The monthly datasets are incomplete as some data are either missing or incorrect - IE: start/end stations are sometimes missing or end time precede start times.

Additionally, the lack of personally identifiable information within the data set limits our ability to identify how users from each user group are using the bikes differently. The data is restrictive or incomprehensive in that it provides data points on the trips themselves, and not user behavior or preference. To determine the preference and usage behaviors of each segment, I would recommend including personally identifiable data and/or surveying a sample of the annual member and casual rider populations.
* **How are you addressing licensing, privacy, security, and accessibility?**

The data does not feature any Personally Identifiable Information (PII). The Company also has a license over the data, and the purpose of the analysis is ethical and within compliance of the [Data License Agreement](https://ride.divvybikes.com/data-license-agreement).

* **How did you verify the data’s integrity?**

All monthly datasets collected the same data. Although some rows are missing fields, the overall integrity of the data should not be considered compromised.
* **How does it help you answer your question?**

The trip data provdes insights on differences in the usage trends between members and casual users.
* **Are there any problems with the data?**

The dataset is incomplete and not comprehensive. As discussed before, survey data and PII should be included to determine each individuals usage patterns and preferences.

<a id="prepare-deliverable"></a>
#### Deliverable
**Description of all data sources used:** The data was sourced created and owned by Lyft Bikes and Scooter, LLC (“Bikeshare”) who operates the City of Chicago’s Divvy bikeshare program. The City has authorized Bikeshare to make portions of the data public.

The spreadsheets feature structured, internal data from Cyclstic. The spreadsheets feature long data consisting of date, numeric, and string data types. The data can help to show how far and long casual riders use Cyclistic bikes compared to their member counterparts.



<a id="process"></a>
# Process
<a id="process-key-tasks"></a>
#### Key Tasks
1. [x] **Check the data for errors.**
2. [x] **Choose your tools.**
3. [x] **Transform the data so you can work with it effectively.**
4. [x] **Document the cleaning process.**
<a id="process-guiding-questions"></a>
#### Guiding Questions
* **What tools are you choosing and why?**

RStudio due to the size of the data set
* **Have you ensured your data’s integrity?**

Yes, the data is generally consistent throughout. Some rows are missing information, and time series data are illogical.
* **What steps have you taken to ensure that your data is clean?**

    1. Removed duplicate trip ID
    2. Removed rows with null fields or missing data
    3. Confirmed all data are consistent or appropriate data types
    4. Removed rows where trip end time preceded start times
    5. Removed rows where trip times were less than 30 seconds. These trips can be assumed to not provide meaningful insights.
    6. Parse dates and times from timestamp data
    7. Confirmed all data fall within a logical range
* **How can you verify that your data is clean and ready to analyze?**

I kept a changelog of the cleaning process and suummarized all columns/conducted exploratory analysis on the data set to ensure it was cleaned.
* **Have you documented your cleaning process so you can review and share those results?**

Yes, in a changelog

<a id="process-deliverable"></a>
#### Deliverable
1. 12/01: removed all empty rows and columns. 
2. 12/01: converted started_at and ended_at columns to timestamp data type
3. 12/01: parse date, month, year, weekday from started_at column
4. 12/01: calculate trip duration from started_at and ended_at columns and format in minutes
5. 12/01: remove 209 rows with duplicated trip_id
6. 12/01: removed 234,940 rows with NAs, start_station_name of 'HUBBARD ST BIKE CHECKING (LBS-WH-TEST)' and 'WATSON TESTING DIVVY', end_statiion_name of '' and 'Base - 2132 W Hubbard Warehouse', and < 0.5 minute trip_duration

<a id="process-code"></a>
#### Process Code

<a id="process-setting-up-the-space"></a>
**Setting up the Space**

```
#install.packages("tidyverse")
library(tidyverse)
library(janitor)
library(lubridate)

#Upload and label .csv files

bs202004 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202004-divvy-tripdata.csv")
bs202005 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202005-divvy-tripdata.csv")
bs202006 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202006-divvy-tripdata.csv")
bs202007 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202007-divvy-tripdata.csv")
bs202008 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202008-divvy-tripdata.csv")
bs202009 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202009-divvy-tripdata.csv")
bs202010 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202010-divvy-tripdata.csv")
bs202011 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202011-divvy-tripdata.csv")
bs202012 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202012-divvy-tripdata.csv")
bs202101 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202101-divvy-tripdata.csv")
bs202102 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202102-divvy-tripdata.csv")
bs202103 <- read.csv("../input/cyclistics-data-april-2020-march-2021/202103-divvy-tripdata.csv")

#Combine the datasets into a single dataframe

bs12mo <- rbind(bs202004, bs202005, bs202006, 
                bs202007, bs202008, bs202009,
                bs202010, bs202011, bs202012,
                bs202101, bs202102, bs202103)
```

<a id="process-data-cleaning"></a>
**Data Cleaning**

```
#Explore the dataset to understand what variables are needed to address the business problem

head(bs12mo)
dim(bs12mo)
glimpse(bs12mo)
str(bs12mo)

#Clean the Environment to allow for faster processing

rm(bs202004, bs202005, bs202006, bs202007, bs202008, bs202009, bs202010, bs202011, bs202012, bs202101, bs202102, bs202103)
```
```
#Start by removing rows and columns with empty data

bs12mo_v2 <- janitor::remove_empty(bs12mo, which = c("cols"))
bs12mo_v2 <- janitor::remove_empty(bs12mo, which = c("rows"))

print(paste("Removed", nrow(bs12mo_v2) - nrow(bs12mo), "empty rows"))
print(paste("Removed", ncol(bs12mo_v2) - ncol(bs12mo), "empty columns"))
```
```
#Transform data into correct data types - convert started_at and ended_at column from string to timestamp

bs12mo_v2$started_at <- lubridate:: ymd_hms(bs12mo_v2$started_at)
bs12mo_v2$ended_at <- lubridate:: ymd_hms(bs12mo_v2$ended_at)
```
```
#Extract data - parse date, month, hour, and weekday from started_at and ended_at variables

bs12mo_v2$start_hour <- lubridate::hour(bs12mo_v2$started_at)
bs12mo_v2$end_hour <- lubridate::hour(bs12mo_v2$ended_at)

bs12mo_v2$start_date <- as.Date(bs12mo_v2$started_at)
bs12mo_v2$end_date <- as.Date(bs12mo_v2$ended_at)

bs12mo_v2$month <- format(as.Date(bs12mo_v2$start_date), "%Y-%m")
bs12mo_v2$day <- format(as.Date(bs12mo_v2$start_date), "%d")
bs12mo_v2$year <- format(as.Date(bs12mo_v2$start_date), "%Y")

bs12mo_v2$start_wkday <- wday(bs12mo_v2$start_date, week_start = 1)
bs12mo_v2$end_wkday <- wday(bs12mo_v2$end_date, week_start = 1)
```
```
#Calculate ride duration using ended_at and started_at timestamp columns, formatted in "minutes" and rounded to the hundredth decimal point. it is assumed an additional decimal point will not provide more meaningful business insight.

bs12mo_v2$trip_duration <- round(difftime(bs12mo_v2$ended_at,bs12mo_v2$started_at,units=c("mins")),2)
```
```
#Summarize the data to ensure that all variables fall within a reasonable range

summary(bs12mo_v2)

#There do not appear to be any latitude and longitude values that fall beyond a reasonable range of the geographical location of Cyclistics operating market.
```
```
#Removed duplicate trip_ids

bs12mo_v3 <- bs12mo_v2[!duplicated(bs12mo_v2$ride_id), ]

print(paste("Removed", nrow(bs12mo_v2) - nrow(bs12mo_v3), "duplicated rows"))
```

Before running the code chunk below, follow up with Marketing Manager to confirm below:
* Can we omit rows with NAs?
* Trip_durations below 30 seconds might be considered outliers and might not be datapoints to include in the dataset. 
* How are data like the start_station_id, end_station_id, lattitude, and longitude collected? Why are some rows missing this info? Can we rely on this data when available?

```
#Read through list of start_station_names and end_station_names to determine 

unique(bs12mo_v3$start_station_name)
unique(bs12mo_v3$end_station_name)
```
```
#Filter out trip_duration below 30 seconds (0.5min) and remove all NA rows and trips with Cyclistic testing facilities, warehouses, or maintennace/repair as the station. 

cleaned_bs12mo <- bs12mo_v3[!(bs12mo_v3$start_station_name == "WATSON TESTING - DIVVY" | bs12mo_v3$start_station_name == "HUBBARD ST BIKE CHECKING (LBS-WH-TEST)" | bs12mo_v3$start_station_name == "" | bs12mo_v3$end_station_name == "" | bs12mo_v3$end_station_name == "Base - 2132 W Hubbard Warehouse" | bs12mo_v3$trip_duration < 0.5),] %>%
  drop_na()

print(paste("Removed", nrow(bs12mo_v3) - nrow(cleaned_bs12mo), "NA, start_station_name of 'HUBBARD ST BIKE CHECKING (LBS-WH-TEST)' and 'WATSON TESTING DIVVY', end_statiion_name of '' and 'Base - 2132 W Hubbard Warehouse', and < 0.5 minute trip_duration rows"))
```

Once finished with the cleaning process, export the cleaned data frame as a .csv and clean the Environment

```
cleaned_bs12mo %>%
    write.csv("cleaned_bs12mo.csv")
```
```
#Clean out environment
rm(bs12mo_v3, bs12mo_v2, bs12mo)
```


<a id="analyze"></a>
# Analyze
<a id="analyze-key-tasks"></a>
#### Key Tasks
1. [x] **Aggregate your data so it’s useful and accessible.**
2. [x] **Organize and format your data.**
3. [x] **Perform calculations.**
4. [x] **Identify trends and relationships.**

<a id="analyze-guiding-questions"></a>
#### Guiding Questions
* **How should you organize your data to perform analysis on it?**

I organized the cleaned data into a single data frame and .csv file.
* **Has your data been properly formatted?**

Yes, all columns and rows are the correct data types and formats.
* **What surprises did you discover in the data?**

1. Trip duration volatility was much higher in casual riders
2. Rapid shift in preference from docked bikes to classic and electric bikes at the turn of 2021
* **What trends or relationships did you find in the data?**

1. Ridership mostly occurs between April and October
2. Most rides are taken between 9am and 7pm
3. Over 50% of rides start or end at just 16% of the stations
4. There is a strong preference for docked bikes, but there is a growing preference toward classic and electric bikes toward the end of the analysis period.
* **How will these insights help answer your business questions?**

These insights will directly support my three recommendations in the Act phase of the process.

<a id="analyze-deliverable"></a>
#### Deliverable
**Summary of Analysis:** 

Casual users
* Most trips are taken between April and October, with a sharp decline from October to March. Majority of trips happen on Friday, Saturday, and Sunday, with trips on Monday through Thursday being relatively lower and constant throughout.
* Most rides are taken between 12pm to 7pm. Majority of rides between 12am and 4am are contributed by casual users. 
* Trip duration is typically longer and volatile than member trips, and slowly declines through colder seasons. Median trip variance over the analysis period ranges between 8min-37min - some of the variance, especially between 10pm-5am, could be attributed to outliers and skewed data.
* Trip departures and arrivals from the top 20 stations are seasonal.
* Trip are concentrated around a small subset of stations. 50% of all trips started at 87 different stations, and ended at 86 different stations. 
* There is a strong preference for docked bikes over the analysis period, however there is a growing trend toward electric and classic bikes. 

Members
* Most trips taken between April and October. This group experiences less of a decline in trips between October and March compared to the casual user group.
* While most trips are taken on Saturday, total trip count over the analysis period is more evenly distributed among weekdays with the lowest being Sunday at 247.7K and highest being Saturday at 301.2K.
* Most rides are taken between 10am-7pm. Members contribute majority of the rides between 6am-9pm.
* Trip duration is typically lower than casual riders, hovering between 10min-15min over the course of the analysis period.
* Trip departures and arrivals from the top 20 stations see less seasonality than casual riders.
* Trips are more evenly spread out among stations. 50% of all trips started and ended at 104 stations.  
* Members also have a strong preference for docked bikes, but show a growing trend toward electric and classic bikes.

<a id="analyze-code"></a>
#### Analyze Code

```
# I start the process with some exploratory analysis by grouping and summarizing the data in different ways. First we need to understand how the data is distributed between the two customer groups.

ggplot(cleaned_bs12mo, aes(member_casual, fill = member_casual)) +
  geom_bar() +
  scale_y_continuous(labels = scales::comma) +
  labs(title = "Exhibit 1: Ride Distribution", subtitle = "Member vs Casual", y = "Count", x = "User Group") + 
  guides(fill = "none")
  ```
  ```
  print(paste("Total Annual Member Rides:", nrow(cleaned_bs12mo[cleaned_bs12mo$member_casual=='member',])))
print(paste("Total Annual Casual Rides:", nrow(cleaned_bs12mo[cleaned_bs12mo$member_casual=='casual',])))
print(paste("Total Rides:", nrow(cleaned_bs12mo)))
print(paste("Annual Members ridership percentage of total:", round(nrow(cleaned_bs12mo[cleaned_bs12mo$member_casual=='member',])/(nrow(cleaned_bs12mo))*100,2),"%"))
print(paste("Casual Riders ridership percentage of total:", round(nrow(cleaned_bs12mo[cleaned_bs12mo$member_casual=='casual',])/nrow(cleaned_bs12mo)*100,2),"%"))
```

<a id="analyze-code-analysis-layout"></a>
**Analysis Layout**
* When are all annual members and casual riders using Cyclistic bikes?
    * Monthly & weekly trends
    * Weekday trends
    * Start hour trends
* How are all annual members and casual riders using Cyclistic bikes?
    * Trip_duration comparison
    * Rideable_type preference
    * Most frequented stations/where are members and casual riders coming and going?


<a id="analyze-code-monthly-weekly-trends"></a>
**Monthly & Weekly Trends**

In order to see how trips vary over the course of the year, I created a dataframe grouping the data by week and month, and then plotted the results to visualize the data over the year.
* Analysis on trip count and trip duration

```
wk <- cleaned_bs12mo %>%
  group_by(member_casual, week = floor_date(start_date,"week")) %>%
  summarize(
    mean = mean(trip_duration),
    median = median(trip_duration),
    count = n()
  )

ggplot(data=wk) +
geom_bar(aes(x = week, y = count, fill = member_casual), stat = "identity", position = "dodge", alpha = 0.6) +
geom_line(aes(x = week, y = median*3000, color = member_casual, group = member_casual), size = 1) +
theme(axis.text.x = element_text(angle = 90, vjust = 0.7)) +
scale_y_continuous(labels = scales::comma, sec.axis = sec_axis(trans = ~./3000, name = "Median Trip Duration (min)")) +
scale_x_date(date_breaks = "2 week") +
labs(title = "Exhibit 2: Weekly Rides", subtitle = "Member vs. Casual", fill = "User Group", x="Week", y = "Ride Count") +
guides(color = "none")
```
```
mo <- cleaned_bs12mo %>%
  group_by(member_casual, month) %>%
  summarize(
    mean = mean(trip_duration),
    median = median(trip_duration),
    count = n()
  )

monthnames <- c(
  '2020-04' = "Apr-20",
  '2020-05' = "May-20",
  '2020-06' = "Jun-20",
  '2020-07' = "Jul-20",
  '2020-08' = "Aug-20",
  '2020-09' = "Sep-20",
  '2020-10' = "Oct-20",
  '2020-11' = "Nov-20",
  '2020-12' = "Dec-20",
  '2021-01' = "Jan-21",
  '2021-02' = "Feb-21",
  '2021-03' = "Mar-21"
)

ggplot(data=mo) +
geom_bar(aes(x = month, y = count, fill = member_casual), stat = "identity", position = "dodge", alpha = 0.6) +
geom_line(aes(x = month, y = median*4000, color = member_casual, group = member_casual), size = 1.5) +
theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) +
scale_x_discrete(labels = as_labeller(monthnames)) +
scale_y_continuous(labels = scales::comma, sec.axis = sec_axis(trans = ~./4000, name = "Median Trip Duration (min)")) +
labs(title="Exhibit 3: Monthly Rides", subtitle = "Member vs. Casual", fill = "User Group", x="Month", y = "Ride Count") +
guides(color = "none")
```

The charts above shows how trip count and median trip duration differs on a weekly and monthly basis between member and casual users. Overall, the bar chart resembles a bell curve, starting with a lower trip count in Spring 2020, peaking during the summer, and declining in Fall/Winter 2020 until eventually increasing again. Line plots both steadily decline from Spring 2020 to Winter 2020, and slowly rebound in Spring 2021. 

Members took more trips than casual users and tended to be shorter when comparing median trip duration of the two groups. Additionally, it appears that most of the trips during the late fall and winter weeks are primarily taken by members as there was a sharp decline in trips and median trip duration among casual users. This suggests that while there is seasonality among both market segments, casual riders are much more sensitive to seasonality. 

While the weekly chart aggregates trip count and median trip information over a shorter period of time helping to narrow in on trends over the course of the analysis period, it will become more difficult to make out any trends in data aggregations moving forward. Because of this, data will be aggregated by month when grouping by additional variables.


<a id="analyze-code-weekday-trends"></a>
**Weekday Trends**
* Analysis on trip count and trip duration

```
wkday <- cleaned_bs12mo %>% 
  group_by(member_casual, start_wkday) %>% 
  summarize(
    count = n(), 
    median = median(trip_duration)
  )

weekdaynames <- c(
  "1" = "Mon",
  "2" = "Tue",
  "3" = "Wed",
  "4" = "Thurs",
  "5" = "Fri",
  "6" = "Sat",
  "7" = "Sun"
)

 ggplot(data = wkday) +
  geom_bar(aes(x = factor(start_wkday), y = count, fill = member_casual), stat = "identity", position = "dodge", alpha = 0.6) +
  geom_line(aes(x = start_wkday, y = median*10000, color = member_casual, group = member_casual), size = 1, alpha = 1.5) +
  theme(axis.text.x = element_text (vjust = 0.7)) +
  scale_x_discrete(labels = as_labeller(weekdaynames)) + 
  scale_y_continuous(labels = scales::comma, sec.axis = sec_axis(trans = ~./10000, name = "Median Trip Duration (min)")) +
  labs(title = "Exhibit 4: Rides by Weekday", subtitle = "Member vs Casual", fill = "User Group", x = "Weekday", y = "Ride Count") +
  guides(color = "none")
```
```
mo_wkday <- cleaned_bs12mo %>%
  group_by(member_casual, month, start_wkday) %>%
  summarize(
    mean = mean(trip_duration),
    median = median(trip_duration),
    count = n()
  ) %>% 
  arrange(month, start_wkday)
```
```
ggplot(data = mo_wkday) +
geom_bar(aes(x = month, y = count, fill = member_casual), stat = "identity", position = "dodge", alpha = 0.6) +
geom_line(aes(x = month, y = median*1000, color = member_casual, group = member_casual), size = 1, alpha = 1.5) +
facet_wrap(~start_wkday, labeller = as_labeller(weekdaynames)) + 
theme(axis.text.x = element_text(angle = 90, vjust = 0.7)) +
scale_x_discrete(labels = as_labeller(monthnames)) +
scale_y_continuous(labels = scales::comma, sec.axis = sec_axis(trans = ~./1000, name = "Median Trip Duration (min)")) +
labs(title="Exhibit 5: Monthly Rides by Weekday", subtitle = "Member vs. Casual", fill = "User Group", x = "Month", y = "Ride Count") + 
guides(color = "none")

cleaned_bs12mo %>% 
  group_by(member_casual, start_wkday) %>% 
  summarize(
    count = n(),
    median_duration = median(trip_duration)
  ) %>% 
  arrange(member_casual,desc(count))
```

While trip count for members is more evenly distributed among weekdays having a range of 54,000 trips and highest amount of trips taken on Saturday, Friday, and Wednesday, casual ridership is more heavily skewed toward the weekend having a range of 182,000 trips and most trips taken on Saturday, Sunday, and Friday.  Median trip duration line plots do not reveal vast differences between this and the previous plot, with the exception of a few outliers.


<a id="analyze-code-start-hour-trends"></a>
**Start Hour Trends**
* Analysis on trip count and trip duration

```
mo_hr <- cleaned_bs12mo %>%
  group_by(member_casual, month, start_hour) %>%
  summarize(
    mean= mean(trip_duration),
    median= median(trip_duration),
    count=n() 
  ) %>% 
  ungroup()

ggplot(data=mo_hr) +
geom_bar(aes(x = month, y = count, fill = member_casual), stat = "identity", position = "dodge", alpha = 0.7) + 
geom_line(aes(x = month, y = median*1000, color = member_casual, group = member_casual), size = 0.5, alpha = 1.5) +
facet_wrap(~start_hour) + 
theme(axis.text.x = element_text(angle = 90, vjust = 0.5, size = 6), axis.text.y = element_text(size = 6)) +
scale_y_continuous(labels = scales::comma, limits = c(0, 35000), sec.axis = sec_axis(trans = ~./1000, name = "Median Trip Duration (min)")) + 
scale_x_discrete(labels = as_labeller(monthnames)) +
labs(title="Exhibit 6: Monthly Rides by Hour", subtitle = "Member vs Casual", fill = "User Group", x = "Month", y = "Ride Count") +
guides(color = "none")
```

The chart above above consists of 24 combo bar and bar charts each corresponding to start hour, with x-axes representing Months, y-axes representing Trip Count and Median Trip Duration, with colors corresponding to member and casual users.

The chart shows that trip count in morning hours between 6am-9am are dominated by members at most months of the year. From 10am-7pm, the bar charts show that member and casual users are similar in total ride count between June 2020 to the end of October 2020, but we see a dramatic decline in casual user ridership after this time frame. Ride counts from 8pm-12am between June 2020 and October 2020 are mostly contributed by casual users, however we see the same drop off in ride count post-October 2020. Median trip duration generally shows a similar trend between groups over the course of the year. While median trip duration for members is relatively consistent for each start hour and across the analysis period, casual user median trip duration shows more volatility overall, with the most variance between 10pm - 5am. This could be attributable to skewed data and/or outliers.

```
wkday_hr <- cleaned_bs12mo %>%
  group_by(member_casual, start_wkday, start_hour) %>%
  summarize(
    mean= mean(trip_duration),
    median= as.numeric(median(trip_duration)),
    count=n() 
  ) %>% 
  ungroup()
  
ggplot(data=wkday_hr) +
geom_bar(aes(x = factor(start_hour), y = count, fill = member_casual), stat = "identity", position = "dodge", alpha = 0.7) + 
geom_line(aes(x = start_hour, y = median*1000, color = member_casual, group = member_casual), size = 0.5) +
facet_wrap(~as.factor(start_wkday), labeller = as_labeller(weekdaynames)) + 
theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) +
scale_y_continuous(labels = scales::comma, limits = c(0, 40000), sec.axis = sec_axis(trans = ~./1000, name = "Median Trip Duration (min)")) + 
labs(title="Exhibit 7: Hourly Rides by Weekday", subtitle = "Member vs. Casual", fill = "User Group", x = "Start Hour", y = "Count") +
guides(color = "none")
```

Exhibit 7 shows ride count and median ride duration over all hours of the day divided into seven plots for each day of the week. These plots show that the members dominate the rides during the weekdays at most hours of the day, but ride counts even out over all hours on the weekend. 


To simplify the Exhibits 6 and 7 above, I plot the chart below aggregating trip counts into columns by start hour.

```
ggplot(data = mo_hr) +
geom_bar(aes(x = factor(start_hour), y = count, fill = member_casual), stat = "identity", position = "dodge") +
theme(axis.text.x = element_text(vjust = 0.5)) +
scale_y_continuous(labels = scales::comma) + 
labs(title="Exhibit 8: Ride Count by Start Hour", subtitle = "Member vs. Casual", fill = "User Group", x = "Start Hour", y = "Ride Count") 
```
```
ggplot(data = mo_hr) + 
geom_boxplot(aes(x = factor(start_hour), y = median, fill = member_casual)) +
theme(axis.text.x = element_text(vjust = 0.5)) +
ylim(0,50) + 
labs(title="Exhibit 9: Median Monthly Ride Duration by Hour", subtitle = "Member vs. Casual", fill = "User Group", x = "Start Hour", y = "Median Duration (min)")
```
```
cleaned_bs12mo %>% 
  group_by(member_casual, start_hour) %>% 
  summarize(
    count=n(),
    median_duration=median(trip_duration)
  ) %>% 
  arrange(member_casual, desc(count))
```

The charts above show the total count of trips that started at each hour of the day and the monthly variance of median trip duration at each hour. It reinforces the insights gained previously aggregating trip count and trip duration data over the course of the year, however it does not show how trip count at each start hour and trip duration change throughout the year since these are not plotted over time.


Now that we understand how much and how long each user group is using Cyclistic bikes, I want to understand the difference between member and casual users for the most frequented start and end stations, what the most popular rideable type is, and any trends in these categories over the analysis period.

Start by summarizing the data


<a id="analyze-code-rideable-type-trends"></a>
**Rideable Type Trends**

```
mo_type <- cleaned_bs12mo %>% 
  group_by(member_casual, month, rideable_type) %>% 
  summarize(
    count = n()
  ) 

ggplot(data = mo_type, aes(x = member_casual, y = count, fill = rideable_type)) +
geom_bar(stat = "identity", color = "white") +
facet_grid(~month, labeller = as_labeller(monthnames)) +
theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) + 
scale_y_continuous(labels = scales::comma) +
labs(title = "Exhibit 10: Rideable Type", subtitle = "Member vs. Casual", y = "Ride Count", x = "User Group", fill = "Rideable Type")
```

Exhibit 9 above shows docked bikes account for the largest portion of trips for both members and casual users, however we see a trend of increasing usage of electric bikes among both groups from August 2020, and classic bikes from December 2020. Another trend that emerges over time is that riders, both members and casual users alike, are choosing to use classic bikes over the other two bike types, although we'll need to monitor how rideable types change going forward.


<a id="analyze-code-start-and-end-station-trends"></a>
**Start and End Station Trends**
* Where are Cyclistic users arriving and departing from?

```
start_station <- cleaned_bs12mo %>% 
  group_by(member_casual, start_station_name) %>% 
  summarize(
    count=n()
  ) %>% 
  arrange(desc(count))

start_station$pct_total = (100*(start_station$count/sum(start_station$count)))

start_station$pct_group = 
  if_else(start_station$member_casual == "casual", (100*(start_station$count/1338712)), (100*(start_station$count/1915887))) 

start_station$cumct_total =
  cumsum(start_station$count)

start_station$cumct_group <- ave(start_station$count, start_station$member_casual, FUN=cumsum)

start_station$cumpct_total = (100*(start_station$cumct_total)/sum(start_station$count))

start_station$cumpct_group = 
  if_else(start_station$member_casual == "casual", (100*(start_station$cumct_group/1338712)), (100*(start_station$cumct_group/1915887)))

head(start_station)
```
```
start_station %>% 
  top_n(20, count) %>% 
  ggplot(aes(x = start_station_name, y = count, fill = member_casual)) + 
  geom_bar(stat = "identity") +
  theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) +
  scale_y_continuous(labels = scales::comma) +
  labs(title = "Exhibit 11: Top 20 Start Stations", subtitle = "Member vs Casual", fill = "User Group", x = "Start Station", y = "Ride Count")
```

This graph shows the top 20 start stations in ride count for members and casual riders. It shows that nearly half of the stations are either groups' top 20, showing that members and casual riders share alike share a high number of trip departures from these stations.

```
start_station %>% 
  filter(pct_group >= 0.01) %>% 
  mutate(percent_ranges = cut(pct_group, seq(0, 2, 0.05))) %>%
  group_by(member_casual, percent_ranges) %>% 
  summarize(
    count = n()
    ) %>% 
  ggplot(aes(x = percent_ranges, y = count, fill = member_casual)) +
  geom_bar(stat = "identity", position = "dodge") +
  theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) +
  labs(title = "Exhibit 12: Distribution of Rides per Start Station", subtitle = "Percent of Total Member and Casual Rides", x = "Contribution Percentage Range", y = "Number of Start Stations", fill = "User Group") +
  annotate("text", x = "(0.3,0.35]", y = 175, label = "*exlcudes start stations <0.01% of member/casual ride percentages", size = 2.25)


start_station %>% 
  mutate(percent_ranges = cut(pct_group, seq(0, 2, 0.05))) %>%
  group_by(member_casual, percent_ranges) %>% 
  summarize(
    count = n()
    )
```

The bar chart above plots the number of start stations that fall within of contribution percentage ranges on the x-axis. The contribution ranges are groupings for ride count percentage of each start station for members and casual riders. For example, over 150 start stations contributed between 0.00% and 0.05% of all casual rides.

This shows how ride counts between members and casual riders are distributed among start stations on a percent of total rides of each group basis. The visual along with the data table are skewed to the left, meaning that most stations contribute a very small percentage of the total ridership among groups. For example, 87 start stations account for 50% of casual rides, while 104 stations account for 50% of member rides. 

```
end_station <- cleaned_bs12mo %>% 
  group_by(member_casual, end_station_name) %>%
  summarize(
    count = n()
  ) %>%
  arrange(desc(count))

end_station$pct_total = (100*(end_station$count/sum(end_station$count)))

end_station$pct_group = 
  if_else(end_station$member_casual == "casual", (100*(end_station$count/1338712)), (100*(end_station$count/1915887))) 

end_station$cumct_total =
  cumsum(end_station$count)

end_station$cumct_group <- ave(end_station$count, end_station$member_casual, FUN=cumsum)

end_station$cumpct_total = (100*(end_station$cumct_total)/sum(end_station$count))

end_station$cumpct_group = 
  if_else(end_station$member_casual == "casual", (100*(end_station$cumct_group/1338712)), (100*(end_station$cumct_group/1915887)))

head(end_station)
```
```
end_station %>% 
  top_n(20, count) %>% 
  ggplot(aes(x = end_station_name, y = count, fill = member_casual)) + 
  geom_bar(stat = "identity") +
  theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) +
  scale_y_continuous(labels = scales::comma) +
  labs(title = "Exhibit 13: Top 20 End Stations", subtitle = "Member vs Casual", fill = "User Group", x = "End Station", y = "Ride Count")
```

This graph shows the top 20 end stations in ride count for members and casual riders. Comparing the top 20 start and end stations among members and casual riders, the visuals similar. In addition to both plots sharing much of the same stations, trip counts among common stations are very similar as well. 

```
end_station %>% 
  filter(pct_group >= 0.01) %>% 
  mutate(percent_ranges = cut(pct_group, seq(0, 2.15, 0.05))) %>%
  group_by(member_casual, percent_ranges) %>% 
  summarize(
    count = n()
    ) %>% 
  ggplot(aes(x = percent_ranges, y = count, fill = member_casual)) +
  geom_bar(stat = "identity", position = "dodge") +
  theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) +
  labs(title = "Exhibit 14: Distribution of Rides per End Station", subtitle = "Percent of Total Member and Casual Rides", x = "Contribution Percentage Range", y = "Number of End Stations", fill = "User Group") +
  annotate("text", x = "(0.3,0.35]", y = 165, label = "*exlcudes end stations <0.01% of member/casual ride percentages", size = 2.25)


end_station %>% 
  mutate(percent_ranges = cut(pct_group, seq(0, 2.15, 0.05))) %>%
  group_by(member_casual, percent_ranges) %>% 
  summarize(
    count = n()
    )
```

Similar to the "Distribution of Rides per Start Station", this shows how ride counts between members and casual riders are distributed among end stations on a percent of total rides of each group basis. The visual along with the data table are skewed to the left, meaning that most stations contribute a very small percentage of the total ridership among groups. For example, 86 end stations account for 50% of casual rides, while 104 end stations account for 50% of member rides. 

This shows that rides are more evenly distributed among stations for members then casual riders. 

Next, I wanted to see how trip counts to and from the top 20 stations for members and casual riders changed over the course of the year.

```
top_casual_start_stations <- cleaned_bs12mo %>% 
  group_by(member_casual, month, start_station_name) %>% 
  summarize(
    count = n()
  ) %>% 
  filter(member_casual == "casual", start_station_name == "Buckingham Fountain" | start_station_name == "Clark St & Armitage Ave" | start_station_name == "Clark St & Elm St" | start_station_name == "Clark St & Lincoln Ave" | start_station_name == "Columbus Dr & Randolph St" | start_station_name == "Fairbanks Ct & Grand Ave" | start_station_name == "Indiana Ave & Roosevelt Rd" | start_station_name == "Lake Shore Dr & Monroe St" | start_station_name == "Lake Shore Dr & North Blvd" | start_station_name == "Michigan Ave & 8th St" | start_station_name == "Michigan Ave & Lake St" | start_station_name == "Michigan Ave & Oak St" | start_station_name == "Michigan Ave & Washington St" | start_station_name == "Millennium Park" | start_station_name == "Shedd Aquarium" | start_station_name == "Streeter Dr & Grand Ave" | start_station_name == "Theater on the Lake" | start_station_name == "Wabash Ave & Grand Ave" | start_station_name == "Wells St & Concord Ln" | start_station_name == "Wells St & Elm St")

top_casual_start_stations %>% 
  ggplot(aes(x = month, y = start_station_name, fill = count)) +
  geom_tile(color = "white", lwd = 0.5, linetype = 1) +
  coord_fixed() +
  scale_fill_distiller() + 
  theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) + 
  scale_x_discrete(label = as_labeller(monthnames)) + 
  labs(title = "Exhibit 15: Top 20 Start Station Heat Map", subtitle = "Among Casual Riders", x = element_blank(), y = "Station Name", fill = "Ride Count")
```
```
top_casual_end_stations <- cleaned_bs12mo %>% 
  group_by(member_casual, month, end_station_name) %>% 
  summarize(
    count = n()
  ) %>% 
  filter(member_casual == "casual", end_station_name == "Buckingham Fountain" | end_station_name == "Clark St & Armitage Ave" | end_station_name == "Clark St & Elm St" | end_station_name == "Clark St & Lincoln Ave" | end_station_name == "Fairbanks Ct & Grand Ave" | end_station_name == "Indiana Ave & Roosevelt Rd" | end_station_name == "Lake Shore Dr & Belmont Ave" | end_station_name == "Lake Shore Dr & Monroe St" | end_station_name == "Lake Shore Dr & North Blvd" | end_station_name == "Lake Shore Dr & Wellington Ave" | end_station_name == "Michigan Ave & 8th St" | end_station_name == "Michigan Ave & Lake St" | end_station_name == "Michigan Ave & Oak St" | end_station_name == "Michigan Ave & Washington St" | end_station_name == "Michigan Ave & Washington St" | end_station_name == "Millennium Park" | end_station_name == "Streeter Dr & Grand Ave" | end_station_name == "Theater on the Lake" | end_station_name == "Wabash Ave & Grand Ave" | end_station_name == "Wabash Ave & Roosevelt Rd" | end_station_name == "Wells St & Concord Ln")

top_casual_end_stations %>% 
  ggplot(aes(x = month, y = end_station_name, fill = count)) +
  geom_tile(color = "white", lwd = 0.5, linetype = 1) +
  coord_fixed() +
  scale_fill_distiller() + 
  theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) + 
  scale_x_discrete(label = as_labeller(monthnames)) + 
  labs(title = "Exhibit 16: Top 20 End Station Heat Map", subtitle = "Among Casual Riders", x = element_blank(), y = "Station Name", fill = "Ride Count")
```

The heat maps above show how ride count for the top 20 start/end stations for casual riders vary over the analysis period. Arrivals and departures peak at these stations during the summer months, followed by a sharp decline in ride count across all stations headed into the winter months, and a slight rebound at the start of spring.

The start and end station heat maps for casual riders are largely the same, not only in the start/end stations in the charts, but also in the inflections in the heat map. 

```
top_member_start_stations <- cleaned_bs12mo %>% 
  group_by(member_casual, month, start_station_name) %>% 
  summarize(
    count = n()
  ) %>% 
  filter(member_casual == "member", start_station_name == "Broadway & Barry Ave" | start_station_name == "Broadway & Cornelia Ave" | start_station_name == "Clark St & Armitage Ave" | start_station_name == "Clark St & Elm St" | start_station_name == "Clark St & Lincoln Ave" |  start_station_name == "Clark St & Schiller St" | start_station_name == "Columbus Dr & Randolph St" | start_station_name == "Dearborn Pkwy & Delaware Pl" | start_station_name == "Dearborn St & Erie St" |  start_station_name == "Desplaines St & Kinzie St" | start_station_name == "Kingsbury St & Kinzie St" |  start_station_name == "Lake Shore Dr & North Blvd" |  start_station_name == "Lake Shore Dr & Wellington Ave" |  start_station_name == "Larrabee St & Webster Ave" | start_station_name == "St. Clair St & Erie St" | start_station_name == "Theater on the Lake" | start_station_name == "Wabash Ave & Grand Ave" | start_station_name == "Wells St & Concord Ln" | start_station_name == "Wells St & Elm St" | start_station_name == "Wells St & Huron St")

top_member_start_stations %>% 
  ggplot(aes(x = month, y = start_station_name, fill = count)) +
  geom_tile(color = "white", lwd = 0.5, linetype = 1) +
  coord_fixed() +
  scale_fill_distiller() + 
  theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) + 
  scale_x_discrete(label = as_labeller(monthnames)) + 
  labs(title = "Exhibit 17: Top 20 Start Station Heat Map", subtitle = "Among Members", x = element_blank(), y = "Station Name", fill = "Ride Count")
```
```
top_member_end_stations <- cleaned_bs12mo %>% 
  group_by(member_casual, month, end_station_name) %>% 
  summarize(
    count = n()
  ) %>% 
  filter(member_casual == "member", end_station_name == "Broadway & Barry Ave" | end_station_name == "Broadway & Cornelia Ave" | end_station_name == "Clark St & Armitage Ave" | end_station_name == "Clark St & Drummond Pl" | end_station_name == "Clark St & Elm St" |  end_station_name == "Clark St & Lincoln Ave" | end_station_name == "Dearborn Pkwy & Delaware Pl" | end_station_name == "Dearborn St & Erie St" | end_station_name == "Desplaines St & Kinzie St" |  end_station_name == "Kingsbury St & Kinzie St" |  end_station_name == "Lake Shore Dr & North Blvd" |  end_station_name == "Lake Shore Dr & Wellington Ave" |  end_station_name == "Larrabee St & Webster Ave" | end_station_name == "St. Clair St & Erie St" | end_station_name == "Theater on the Lake" | end_station_name == "Wabash Ave & Grand Ave" | end_station_name == "Wabash Ave & Roosevelt Rd" | end_station_name == "Wells St & Concord Ln" | end_station_name == "Wells St & Elm St" | end_station_name == "Wells St & Huron St")

top_member_end_stations %>% 
  ggplot(aes(x = month, y = end_station_name, fill = count)) +
  geom_tile(color = "white", lwd = 0.5, linetype = 1) +
  coord_fixed() +
  scale_fill_distiller() + 
  theme(axis.text.x = element_text(angle = 90, vjust = 0.5)) + 
  scale_x_discrete(label = as_labeller(monthnames)) + 
  labs(title = "Exhibit 18: Top 20 End Station Heat Map", subtitle = "Among Members", x = element_blank(), y = "Station Name", fill = "Ride Count")
```


<a id="share"></a>
# Share
<a id="share-key-tasks"></a>
#### Key Tasks
1. [x] Determine the best way to share your findings.
2. [x] Create effective data visualizations.
3. [x] Present your findings.
4. [x] Ensure your work is accessible

<a id="share-guiding-questions"></a>
#### Guiding Questions

**Were you able to answer the question of how annual members and casual riders use Cyclistic bikes differently?**

Yes, their use patterns are different and could be explainable through several reasons.

**What story does your data tell?**

Annual members and casual riders are very different in how they use Cyclistic bikes. While members might use Cyclistic bikes for more consistent reasons, for exmaple commuting to and from work, running errands, or exercising, casual riders seem to use Cyclistic on an ad-hoc need basis.

**How do your findings relate to your original question?**

The findings provide an understanding of the differences between annual members and casual riders. 

**Who is your audience? What is the best way to communicate with them?**

Marketing Director Lily Moreno and colleagues on the Marketing Analytics Team.

**Can data visualization help you share your findings?**

Yes, it helps to provide a quick and easy understanding of the dataset and helps reinforce insights from the data.

**Is your presentation accessible to your audience?**

Yes, visuals are properly labelled and created with vibrant colors. 
<a id="share-deliverable"></a>
#### Deliverable
**Supporting visualizations and key findings:**

* Casual Riders
    * Seasonal ridership - most rides occur in the summer to fall months, with steep declines during colder months. Casual riders have a tendency to use Cyclistic in the afternoon hours. Most of the trips occur on weekends.
    * There is a portion of the casual rider population that relies on Cyclistic for commuting during the weekdays. The remainder of the population uses Cyclistic bikes on an adhoc basis for non-commuting/leisurely needs like exercising, running errands, or for social purposes.
    * Casual riders use Cyclistic to traverse a small portion of the city arriving and departing from a small subset of Cyclistic stations (12.6%) as shown by Exhibits 11 and 13.
    
* Annual Members
    * Ridership is seasonal. While there is a fall off in ridership through the late fall through early spring months, a higher amount of ridership occurs in these month than casual riders suggesting that a small portion of the population relies on Cyclistic for all transportation needs
    * Reason for use of Cyclistic are primarily for communting purposes, but use could also span to other uses like exercise, leisure, and running errands. 
    * Members utilize traverse a larger part of the city with arrivals and departures for most of the rides coming from 15% of stations.


<a id="act"></a>
# Act
<a id="act-key-tasks"></a>
#### Key Tasks
1. [x] **Create your portfolio**
2. [x] **Add your case study**
3. [x] **Practice presenting your case study to a friend or family member**

<a id="act-guiding-questions"></a>
#### Guiding Questions
**What is your final conclusion based on your analysis?**

While Annual Members and Casual Riders largely use Cyclistic for different reasons and have different habits, there appear to be subsets of the Casual User population that could benefit from an Annual Membership
**How could your team and business apply your insights?**

The team could apply the insights by using the findings to impact the a marketing campaign aimed at converting Casual Riders to Annual Members.
**What next steps would you or your stakeholders take based on your findings?**

I would recommend additional data sources and analysis on the user population as well as extraction of secondary data that might have an impact on the Cyclistic user base - IE weather, gas price index, public transportation costs, etc.
**Is there additional data you could use to expand on your findings?**

Among those mentioned previously, data pertaining to the user poplation would probably have the most impact on the findings. One example that comes to mind is a rider ID. Although the casual rider pricing structure allows for single or one-day use, giving riders an ID would allow Cyclistic to identify where each individual is going, and each riders user habits. 
<a id="act-deliverable"></a>
#### Deliverable
**Three Recommendations Based on Analysis**
1. Devise the marketing campaign to show how Cyclistic is a great commuting option as it encourages physical activity, is a environmentally friendly method of transportation, and cost conscious
2. Compile a marketing campaigned aimed at detailing Cyclistics uses as an exercise alternative, means of transportation to and from social/leisurely events, or as a means to run errands.
3. Introduce an additional pricing tier that would either offer semi-annual membership or large price discounts during the winter months.


<a id="conclusion"></a>
# Conclusion

Thank you to anyone reading this. It was a great experience applying what I've learned through the Google Data Analytics Professional Certificate program. I am open to feedback and insights on how to improve this case study or my code. Please feel free to reach out to me via kaggle or [LinkedIn](https://www.linkedin.com/in/royce-romero/)!
