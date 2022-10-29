Bellabeat Case Study - Google Data Analytics Capstone Project 2
================
Anna Mándoki
2022-10-25

![Bellabeat](logo.png)

## 1. Introduction

### 1.1 About the project

This case study is my additional capstone project for the Google Data
Analytics Professional Certificate course. Previously, I completed the
[Cyclistic Bike-Share Case Study](https://github.com/annamandoki/cyclistic_case_study). 
The purpose of this second case study is to keep experimenting with RStudio and to practice the skills I
acquired during the course.

In this project I am assuming the role of a junior data analyst working
on the marketing analyst team at *Bellabeat*, a high-tech manufacturer
of health-focused products for women.

I am going to analyze publicly available fitness tracker data in order
to gain insights into how consumers are using their smart devices.
Identifying any trends in this data will be key to help determine
*Bellabeat*’s marketing strategy in the future.

### 1.2 About Bellabeat

*Bellabeat* is a high-tech wellness company that manufactures
health-focused smart products. Founded in 2013 by artist Urška Sršen and
mathematician Sandro Mur, *Bellabeat* develops technology that informs
women about their health and habits by collecting data on activity,
sleep, stress and reproductive health.

By 2016, *Bellabeat* had opened offices around the world and launched
multiple products, such as the *Bellabeat app*, the *Leaf* pendant, the
*Time* watch and the *Spring* water bottle.

*Bellabeat* is successful small company that has the potential to become
a larger player in the global smart device market.

“Empowering Women to Unlock Their Full Potential.”

More information can be found on their
[website](https://bellabeat.com/).

#### 1.2.1 Marketing strategy of Bellabeat

The company has invested in traditional advertising media, but focuses
on digital marketing extensively:

- Google Search
- Facebook, Instagram and Twitter pages
- Video ads on Youtube
- Ads on Google Display Network

Urška Sršen, cofounder and Chief Creative Officer of Bellabeat, believes
that analyzing smart device fitness data could help unlock new growth
opportunities for the company.

## 2. Ask Phase

### 2.1 Business Objective

- Analyze smart device usage data in order to gain insight into how
  consumers use non-Bellabeat smart devices.
- Select one Bellabeat product to apply these insights to in a
  presentation.

Question that will guide the analysis:

1.  What are some trends in smart device usage?
2.  How could these trends apply to Bellabeat customers?
3.  How could these trends help influence Bellabeat marketing strategy?

### 2.2 Business Task for the Junior Data Analyst

Analyze a public dataset containing personal fitness tracker data from
thirty *FitBit* users to explore the users’ daily habits and identify
trends on how users interact with their smart devices.

### 2.3 About FitBit

Fitbit offers a compact, wireless, wearable sensor, called FitBit
Tracker that tracks a person’s daily activities such as calories burned,
sleep quality, steps and distance, in order to promote a healthy
lifestyle.

The activity data is collected automatically while it is worn by the
user all day and uploaded to a website, where users can see their
progress and share with others. They can manually log nutrition, weight
and other health information in order to gain a complete picture of
their health.

### 2.4 Bellabeat vs FitBit

- **Similarities**: both offer smart wearable products that
  automatically collect data on daily activities to inform users about
  their health

- **Differences**: FitBit’s main product is a tracker device similar to
  a watch used by all genders, while Bellabeat offers a wider selection
  of products that are specifically designed to and used by women.

### 2.5 Stakeholders at Bellabeat

- **Urška Sršen**: Bellabeat’s cofounder and Chief Creative Officer
- **Sando Mur**: Mathematician and Bellabeat’s cofounder; key member of
  the Bellabeat executive team
- **Bellabeat marketing analytics team**: A team of data analysts
  responsible for collecting, analyzing, and reporting data that helps
  guide Bellabeat’s marketing strategy. I am a Junior Data Analyst in
  this team.

### 2.6 Key steps taken in the Ask Phase

- Defined Business Objective and Task for the Junior Data Analyst
- Researched FitBit and examined similarities and differences to
  Bellabeat
- Defined the stakeholders

## 3. Prepare Phase

### 3.1 Dataset location

The publicly available FitBit tracker data proposed by Bellabeat can be
found on Kaggle: [FitBit Fitness Tracker
Data](https://www.kaggle.com/arashnic/fitbit) (CC0: Public Domain,
dataset made available through
[Mobius](https://www.kaggle.com/arashnic))

Alternatively, the data is also made available
[here](https://zenodo.org/record/53894#.Y054AfzP2Un), stored in the
open-access repository Zenodo, created by the authors Furberg Robert,
Brinton Julia, Keating Michael and Ortiz Alexa.

### 3.2 Data organization

The dataset consists of 18 csv files, generated by respondents to a
distributed survey via *Amazon Mechanical Turk* between March 12, 2016 -
May 12, 2016.

- dailyActivity_merged.csv
- dailyCalories_merged.csv
- dailyIntensities_merged.csv
- dailySteps_merged.csv
- heartrate_seconds_merged.csv
- hourlyCalories_merged.csv
- hourlyIntensities_merged.csv
- hourlySteps_merged.csv
- minuteCaloriesNarrow_merged.csv
- minuteCaloriesWide_merged.csv
- minuteIntensitiesNarrow_merged.csv
- minuteIntensitiesWide_merged.csv
- minuteMETsNarrow_merged.csv
- minuteSleep_merged.csv
- minuteStepsNarrow_merged.csv
- minuteStepsWide_merged.csv
- sleepDay_merged.csv
- weightLogInfo_merged.csv

### 3.3 Credibility and bias

Thirty eligible Fitbit users consented to the submission of personal
tracker data, including minute-level output for physical activity, heart
rate, and sleep monitoring.

- **Reliable**: LOW - The dataset is not very reliable, as the sample
  size is small (30), that implies sampling bias.

- **Original**: LOW - The data was collected via Amazon Mechanical Turk,
  not directly by the company (FitBit), therefore the originality level
  if low.

- **Comprehensive**: MEDIUM - The datasets contain information that
  would help determine users’ habits, however the number of participants
  vary across the files: 8 to 33. Apart from this, we have no
  information on participants’ demographic characteristics, such as
  gender or age group.

- **Current**: LOW - The dataset is not current, as it was first
  published in 2016. It is 6 years old as of October 2022, however
  fitness and wellness habits do not necessarily change drastically,
  even if we take into consideration slight shifts as result of the
  recent pandemic.

- **Cited**: MEDIUM - The dataset is well documented, the names of the
  authors is shown, however it was collected through a third party.

**Conclusion**: In a real-life scenario, I would be cautious with using
this dataset for conducting comprehensive analysis and for making
business recommendations based on it.

### 3.4 Licensing, privacy, security

The data is anonymized; it contains no personally identifiable
information. Privacy in ensured.

As mentioned above, the dataset is publicly available through a Kaggle
user named [Mobius](https://www.kaggle.com/arashnic) and through
repository [Zenodo](https://zenodo.org/record/53894#.Y054AfzP2Un) by the
authors Furberg Robert, Brinton Julia, Keating Michael and Ortiz Alexa.

### 3.5 Is the data helpful in answering the question in the Business Task?

To be able to answer the business question, we need to have access to
FitBit tracker data from real-life users on different kinds of wellness
information. We can find such information in the provided csv files, but
it is important to be mindful of the limitations and issues of the data
(discussed above in the ‘Credibility and bias’ section) during our
analysis.

### 3.6 Datasets selected for analysis

After taking a first look at the data using LibreOffice Calc, I decided
to start my analysis with the exploration of the following files:

- dailyActivity_merged.csv
- dailyCalories_merged.csv
- dailyIntensities_merged.csv
- dailysteps_merged.csv
- hourlySteps_merged.csv
- sleepDay_merged.csv
- weightLogInfo_merged.csv

### 3.7 Key steps taken in the Prepare Phase

- Downloaded data and stored on computer
- Identified how the data is organized
- Took a first look at the data using LibreOffice Calc
- Determined credibility of the data.
- Selected datasets to analyze

## 4. Process Phase

### 4.1 Tools

After taking a first look into each of the csv files using LibreOffice
Calc, I switched to RStudio Desktop to further explore the selected
datasets.

### 4.2 Setting up my environment

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.2 ──
    ## ✔ ggplot2 3.3.6      ✔ purrr   0.3.4 
    ## ✔ tibble  3.1.8      ✔ dplyr   1.0.10
    ## ✔ tidyr   1.2.1      ✔ stringr 1.4.1 
    ## ✔ readr   2.1.2      ✔ forcats 0.5.2 
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

``` r
library(janitor)
```

    ## 
    ## Attaching package: 'janitor'
    ## 
    ## The following objects are masked from 'package:stats':
    ## 
    ##     chisq.test, fisher.test

``` r
library(skimr)
library(lubridate)
```

    ## 
    ## Attaching package: 'lubridate'
    ## 
    ## The following objects are masked from 'package:base':
    ## 
    ##     date, intersect, setdiff, union

### 4.3 Data importing

Read the selected 7 csv files.

``` r
daily_activity <- read.csv("dailyActivity_merged.csv")
daily_calories <- read.csv("dailyCalories_merged.csv")
daily_intensities <- read.csv("dailyIntensities_merged.csv")
daily_steps <- read.csv("dailySteps_merged.csv")
hourly_steps <- read.csv("hourlySteps_merged.csv")
sleep_day <- read.csv("sleepDay_merged.csv")
weight_log <- read.csv("weightLogInfo_merged.csv")
```

### 4.4 Viewing the data frames

Take a closer look into the data frames one by one.

#### 4.4.1 daily_activity

``` r
glimpse(daily_activity)
```

    ## Rows: 940
    ## Columns: 15
    ## $ Id                       <dbl> 1503960366, 1503960366, 1503960366, 150396036…
    ## $ ActivityDate             <chr> "4/12/2016", "4/13/2016", "4/14/2016", "4/15/…
    ## $ TotalSteps               <int> 13162, 10735, 10460, 9762, 12669, 9705, 13019…
    ## $ TotalDistance            <dbl> 8.50, 6.97, 6.74, 6.28, 8.16, 6.48, 8.59, 9.8…
    ## $ TrackerDistance          <dbl> 8.50, 6.97, 6.74, 6.28, 8.16, 6.48, 8.59, 9.8…
    ## $ LoggedActivitiesDistance <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ VeryActiveDistance       <dbl> 1.88, 1.57, 2.44, 2.14, 2.71, 3.19, 3.25, 3.5…
    ## $ ModeratelyActiveDistance <dbl> 0.55, 0.69, 0.40, 1.26, 0.41, 0.78, 0.64, 1.3…
    ## $ LightActiveDistance      <dbl> 6.06, 4.71, 3.91, 2.83, 5.04, 2.51, 4.71, 5.0…
    ## $ SedentaryActiveDistance  <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ VeryActiveMinutes        <int> 25, 21, 30, 29, 36, 38, 42, 50, 28, 19, 66, 4…
    ## $ FairlyActiveMinutes      <int> 13, 19, 11, 34, 10, 20, 16, 31, 12, 8, 27, 21…
    ## $ LightlyActiveMinutes     <int> 328, 217, 181, 209, 221, 164, 233, 264, 205, …
    ## $ SedentaryMinutes         <int> 728, 776, 1218, 726, 773, 539, 1149, 775, 818…
    ## $ Calories                 <int> 1985, 1797, 1776, 1745, 1863, 1728, 1921, 203…

#### 4.4.2 daily_calories

``` r
glimpse(daily_calories)
```

    ## Rows: 940
    ## Columns: 3
    ## $ Id          <dbl> 1503960366, 1503960366, 1503960366, 1503960366, 1503960366…
    ## $ ActivityDay <chr> "4/12/2016", "4/13/2016", "4/14/2016", "4/15/2016", "4/16/…
    ## $ Calories    <int> 1985, 1797, 1776, 1745, 1863, 1728, 1921, 2035, 1786, 1775…

#### 4.4.3 daily_intensities

``` r
glimpse(daily_intensities)
```

    ## Rows: 940
    ## Columns: 10
    ## $ Id                       <dbl> 1503960366, 1503960366, 1503960366, 150396036…
    ## $ ActivityDay              <chr> "4/12/2016", "4/13/2016", "4/14/2016", "4/15/…
    ## $ SedentaryMinutes         <int> 728, 776, 1218, 726, 773, 539, 1149, 775, 818…
    ## $ LightlyActiveMinutes     <int> 328, 217, 181, 209, 221, 164, 233, 264, 205, …
    ## $ FairlyActiveMinutes      <int> 13, 19, 11, 34, 10, 20, 16, 31, 12, 8, 27, 21…
    ## $ VeryActiveMinutes        <int> 25, 21, 30, 29, 36, 38, 42, 50, 28, 19, 66, 4…
    ## $ SedentaryActiveDistance  <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ LightActiveDistance      <dbl> 6.06, 4.71, 3.91, 2.83, 5.04, 2.51, 4.71, 5.0…
    ## $ ModeratelyActiveDistance <dbl> 0.55, 0.69, 0.40, 1.26, 0.41, 0.78, 0.64, 1.3…
    ## $ VeryActiveDistance       <dbl> 1.88, 1.57, 2.44, 2.14, 2.71, 3.19, 3.25, 3.5…

#### 4.4.4 daily_steps

``` r
glimpse(daily_steps)
```

    ## Rows: 940
    ## Columns: 3
    ## $ Id          <dbl> 1503960366, 1503960366, 1503960366, 1503960366, 1503960366…
    ## $ ActivityDay <chr> "4/12/2016", "4/13/2016", "4/14/2016", "4/15/2016", "4/16/…
    ## $ StepTotal   <int> 13162, 10735, 10460, 9762, 12669, 9705, 13019, 15506, 1054…

#### 4.4.5 hourly_steps

``` r
glimpse(hourly_steps)
```

    ## Rows: 22,099
    ## Columns: 3
    ## $ Id           <dbl> 1503960366, 1503960366, 1503960366, 1503960366, 150396036…
    ## $ ActivityHour <chr> "4/12/2016 12:00:00 AM", "4/12/2016 1:00:00 AM", "4/12/20…
    ## $ StepTotal    <int> 373, 160, 151, 0, 0, 0, 0, 0, 250, 1864, 676, 360, 253, 2…

#### 4.4.6 sleep_day

``` r
glimpse(sleep_day)
```

    ## Rows: 413
    ## Columns: 5
    ## $ Id                 <dbl> 1503960366, 1503960366, 1503960366, 1503960366, 150…
    ## $ SleepDay           <chr> "4/12/2016 12:00:00 AM", "4/13/2016 12:00:00 AM", "…
    ## $ TotalSleepRecords  <int> 1, 2, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, …
    ## $ TotalMinutesAsleep <int> 327, 384, 412, 340, 700, 304, 360, 325, 361, 430, 2…
    ## $ TotalTimeInBed     <int> 346, 407, 442, 367, 712, 320, 377, 364, 384, 449, 3…

#### 4.4.7 weight_log

``` r
glimpse(weight_log)
```

    ## Rows: 67
    ## Columns: 8
    ## $ Id             <dbl> 1503960366, 1503960366, 1927972279, 2873212765, 2873212…
    ## $ Date           <chr> "5/2/2016 11:59:59 PM", "5/3/2016 11:59:59 PM", "4/13/2…
    ## $ WeightKg       <dbl> 52.6, 52.6, 133.5, 56.7, 57.3, 72.4, 72.3, 69.7, 70.3, …
    ## $ WeightPounds   <dbl> 115.9631, 115.9631, 294.3171, 125.0021, 126.3249, 159.6…
    ## $ Fat            <int> 22, NA, NA, NA, NA, 25, NA, NA, NA, NA, NA, NA, NA, NA,…
    ## $ BMI            <dbl> 22.65, 22.65, 47.54, 21.45, 21.69, 27.45, 27.38, 27.25,…
    ## $ IsManualReport <chr> "True", "True", "False", "True", "True", "True", "True"…
    ## $ LogId          <dbl> 1.462234e+12, 1.462320e+12, 1.460510e+12, 1.461283e+12,…

### 4.5 Check the number of unique ‘Id’ numbers

Confirm how many users provided information for each dataset by counting
the unique ‘Id’ numbers using the `lenght()` and `unique()` functions.

``` r
length(unique(daily_activity$Id))
```

    ## [1] 33

``` r
length(unique(daily_calories$Id))
```

    ## [1] 33

``` r
length(unique(daily_intensities$Id))
```

    ## [1] 33

``` r
length(unique(daily_steps$Id))
```

    ## [1] 33

``` r
length(unique(hourly_steps$Id))
```

    ## [1] 33

``` r
length(unique(sleep_day$Id))
```

    ## [1] 24

``` r
length(unique(weight_log$Id))
```

    ## [1] 8

### 4.6 Observations on the data frames

- **daily_activity**

Rows: 940, Columns: 15, Unique Id = Participants: 33

- **daily_calories**

Rows: 940, Columns: 3, Unique Id: 33

- **daily_intensities**

Rows: 940, Columns: 10, Unique Id: 33

- **daily_steps**

Rows: 940, Columns: 3, Unique Id: 33

- **hourly_steps**

Rows: 22,099 Columns: 3, Unique Id: 33

- **sleep_day**

Rows: 413, Columns: 5, Unique Id: 24

- **weight_log**

Rows: 67, Columns: 8, Unique Id: 8

The ‘daily_activity’, ‘daily_calories’, ‘daily_intensities’ and
‘daily_steps’ data frames have the same number of rows (entries) and the
same number of participants.

The ‘hourly_steps’ data frame has 22,099 rows (hourly entries).

The ‘sleep_day’ data frame has significantly less entries, from only 24
participant. The ‘weight_log’ dataset has even less, 67 entries from 8
participants.

### 4.7 Comparing columns and values

The column names in the ‘daily_activity’, ‘daily_calories’,
‘daily_intensities’ and ‘daily_steps’ seem pretty similar. Let’s take
closer look using the `compare_df_cols()` function.

``` r
compare_df_cols(daily_activity,daily_calories,daily_intensities,daily_steps)
```

    ##                 column_name daily_activity daily_calories daily_intensities
    ## 1              ActivityDate      character           <NA>              <NA>
    ## 2               ActivityDay           <NA>      character         character
    ## 3                  Calories        integer        integer              <NA>
    ## 4       FairlyActiveMinutes        integer           <NA>           integer
    ## 5                        Id        numeric        numeric           numeric
    ## 6       LightActiveDistance        numeric           <NA>           numeric
    ## 7      LightlyActiveMinutes        integer           <NA>           integer
    ## 8  LoggedActivitiesDistance        numeric           <NA>              <NA>
    ## 9  ModeratelyActiveDistance        numeric           <NA>           numeric
    ## 10  SedentaryActiveDistance        numeric           <NA>           numeric
    ## 11         SedentaryMinutes        integer           <NA>           integer
    ## 12                StepTotal           <NA>           <NA>              <NA>
    ## 13            TotalDistance        numeric           <NA>              <NA>
    ## 14               TotalSteps        integer           <NA>              <NA>
    ## 15          TrackerDistance        numeric           <NA>              <NA>
    ## 16       VeryActiveDistance        numeric           <NA>           numeric
    ## 17        VeryActiveMinutes        integer           <NA>           integer
    ##    daily_steps
    ## 1         <NA>
    ## 2    character
    ## 3         <NA>
    ## 4         <NA>
    ## 5      numeric
    ## 6         <NA>
    ## 7         <NA>
    ## 8         <NA>
    ## 9         <NA>
    ## 10        <NA>
    ## 11        <NA>
    ## 12     integer
    ## 13        <NA>
    ## 14        <NA>
    ## 15        <NA>
    ## 16        <NA>
    ## 17        <NA>

Apparently, the ‘daily_activity’ data frame contains all columns from
the other three data frames. Naming is different for two column pairs,
but we can assume that ActivityDate = ActivityDay and StepsTotal =
TotalSteps.

At this point, I assume that the ‘daily_activity’ data frame contains
all the information we need and makes the other three data frames
redundant.

To confirm this, I am going to make two other comparisons.

#### 4.7.1 Compare unique ‘Id’ numbers

First, let’s compare the 33 unique ‘Id’ numbers to confirm that we have
information from the same set of users across data frames.

Create a vector for each set of unique ’Id’s to test exact equality
using the `identical()` function:

``` r
vec_daily_act <- c(unique(daily_activity$Id))
vec_daily_cal <- c(unique(daily_calories$Id))
vec_daily_int<- c(unique(daily_intensities$Id))
vec_daily_st <- c(unique(daily_steps$Id))

identical(vec_daily_act,vec_daily_cal,vec_daily_int,vec_daily_st)
```

    ## [1] TRUE

It is now confirmed that all four datasets contain information from the
same 33 participants.

#### 4.7.2 Compare dates

Second, to confirm that the entries were made on the same dates, let’s
test equality of date columns with the `identical()` function:

``` r
identical(daily_activity$ActivityDate, daily_calories$ActivityDay)
```

    ## [1] TRUE

``` r
identical(daily_activity$ActivityDate,daily_intensities$ActivityDay)
```

    ## [1] TRUE

``` r
identical(daily_activity$ActivityDate, daily_steps$ActivityDay)
```

    ## [1] TRUE

We have the same user ‘Id’ numbers and same dates across the datasets.
It confirms that the ‘daily_activity’ dataset contains all the
information we need for our analysis.

Moving forward, I am going to use **‘daily_activity**’,
**’hourly_steps’** and **‘sleep_day’** datasets.

The ‘weight_log’ dataset contains too little information, so it wouldn’t
provide much value. However, we can draw one conclusion from the lack of
data: users do not tend to log their weight on a regular basis.

### 4.8 Convert to datetime

I noticed that the values in the date columns are characters instead of
datetime. I am going to convert them now. The dates are in mm/dd/yyyy
format, so I am using the `mdy()` function.

#### 4.8.1 Convert datetime: ‘daily_activity’

``` r
daily_activity <- daily_activity %>%
  mutate(ActivityDate = mdy(ActivityDate))

glimpse(daily_activity)
```

    ## Rows: 940
    ## Columns: 15
    ## $ Id                       <dbl> 1503960366, 1503960366, 1503960366, 150396036…
    ## $ ActivityDate             <date> 2016-04-12, 2016-04-13, 2016-04-14, 2016-04-…
    ## $ TotalSteps               <int> 13162, 10735, 10460, 9762, 12669, 9705, 13019…
    ## $ TotalDistance            <dbl> 8.50, 6.97, 6.74, 6.28, 8.16, 6.48, 8.59, 9.8…
    ## $ TrackerDistance          <dbl> 8.50, 6.97, 6.74, 6.28, 8.16, 6.48, 8.59, 9.8…
    ## $ LoggedActivitiesDistance <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ VeryActiveDistance       <dbl> 1.88, 1.57, 2.44, 2.14, 2.71, 3.19, 3.25, 3.5…
    ## $ ModeratelyActiveDistance <dbl> 0.55, 0.69, 0.40, 1.26, 0.41, 0.78, 0.64, 1.3…
    ## $ LightActiveDistance      <dbl> 6.06, 4.71, 3.91, 2.83, 5.04, 2.51, 4.71, 5.0…
    ## $ SedentaryActiveDistance  <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ VeryActiveMinutes        <int> 25, 21, 30, 29, 36, 38, 42, 50, 28, 19, 66, 4…
    ## $ FairlyActiveMinutes      <int> 13, 19, 11, 34, 10, 20, 16, 31, 12, 8, 27, 21…
    ## $ LightlyActiveMinutes     <int> 328, 217, 181, 209, 221, 164, 233, 264, 205, …
    ## $ SedentaryMinutes         <int> 728, 776, 1218, 726, 773, 539, 1149, 775, 818…
    ## $ Calories                 <int> 1985, 1797, 1776, 1745, 1863, 1728, 1921, 203…

#### 4.8.2 Convert datetime:‘sleep_day’

``` r
sleep_day <- sleep_day %>%
  mutate(SleepDay = mdy_hms(SleepDay))

glimpse(sleep_day)
```

    ## Rows: 413
    ## Columns: 5
    ## $ Id                 <dbl> 1503960366, 1503960366, 1503960366, 1503960366, 150…
    ## $ SleepDay           <dttm> 2016-04-12, 2016-04-13, 2016-04-15, 2016-04-16, 20…
    ## $ TotalSleepRecords  <int> 1, 2, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, …
    ## $ TotalMinutesAsleep <int> 327, 384, 412, 340, 700, 304, 360, 325, 361, 430, 2…
    ## $ TotalTimeInBed     <int> 346, 407, 442, 367, 712, 320, 377, 364, 384, 449, 3…

#### 4.8.3. Convert datetime and split columns: ‘hourly_steps’

The ‘ActivityHour’ column contains both date and time. First I convert
the character to datetime with `parse_date_time()` to be able to handle
the AM/PM, then I split the column into two separate columns: ‘Day’ and
‘Hour’ using the `separate()` function.

``` r
hourly_steps <- hourly_steps %>%
 mutate(ActivityHour = parse_date_time(ActivityHour, "%m/%d/%Y %I:%M:%S %p")) %>%
  separate(ActivityHour, into = c("Day", "Hour"), sep = " ")

glimpse(hourly_steps)
```

    ## Rows: 22,099
    ## Columns: 4
    ## $ Id        <dbl> 1503960366, 1503960366, 1503960366, 1503960366, 1503960366, …
    ## $ Day       <chr> "2016-04-12", "2016-04-12", "2016-04-12", "2016-04-12", "201…
    ## $ Hour      <chr> "00:00:00", "01:00:00", "02:00:00", "03:00:00", "04:00:00", …
    ## $ StepTotal <int> 373, 160, 151, 0, 0, 0, 0, 0, 250, 1864, 676, 360, 253, 221,…

### 4.9 Convert ‘Id’ numbers to character

We do not need Id number to be numbers (double), as we do not want to
make calculations with them, but we might want to display the different
users on charts and for this we need the Id-s as characters.

#### 4.9.1 Convert ‘Id’ numbers to character: ‘daily_activity’

``` r
daily_activity <- daily_activity %>%
  mutate(Id = as.character(Id))

glimpse(daily_activity)
```

    ## Rows: 940
    ## Columns: 15
    ## $ Id                       <chr> "1503960366", "1503960366", "1503960366", "15…
    ## $ ActivityDate             <date> 2016-04-12, 2016-04-13, 2016-04-14, 2016-04-…
    ## $ TotalSteps               <int> 13162, 10735, 10460, 9762, 12669, 9705, 13019…
    ## $ TotalDistance            <dbl> 8.50, 6.97, 6.74, 6.28, 8.16, 6.48, 8.59, 9.8…
    ## $ TrackerDistance          <dbl> 8.50, 6.97, 6.74, 6.28, 8.16, 6.48, 8.59, 9.8…
    ## $ LoggedActivitiesDistance <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ VeryActiveDistance       <dbl> 1.88, 1.57, 2.44, 2.14, 2.71, 3.19, 3.25, 3.5…
    ## $ ModeratelyActiveDistance <dbl> 0.55, 0.69, 0.40, 1.26, 0.41, 0.78, 0.64, 1.3…
    ## $ LightActiveDistance      <dbl> 6.06, 4.71, 3.91, 2.83, 5.04, 2.51, 4.71, 5.0…
    ## $ SedentaryActiveDistance  <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ VeryActiveMinutes        <int> 25, 21, 30, 29, 36, 38, 42, 50, 28, 19, 66, 4…
    ## $ FairlyActiveMinutes      <int> 13, 19, 11, 34, 10, 20, 16, 31, 12, 8, 27, 21…
    ## $ LightlyActiveMinutes     <int> 328, 217, 181, 209, 221, 164, 233, 264, 205, …
    ## $ SedentaryMinutes         <int> 728, 776, 1218, 726, 773, 539, 1149, 775, 818…
    ## $ Calories                 <int> 1985, 1797, 1776, 1745, 1863, 1728, 1921, 203…

#### 4.9.2 Convert ‘Id’ numbers to character: ‘sleep_day’

``` r
sleep_day <- sleep_day %>%
  mutate(Id = as.character(Id))

glimpse(sleep_day)
```

    ## Rows: 413
    ## Columns: 5
    ## $ Id                 <chr> "1503960366", "1503960366", "1503960366", "15039603…
    ## $ SleepDay           <dttm> 2016-04-12, 2016-04-13, 2016-04-15, 2016-04-16, 20…
    ## $ TotalSleepRecords  <int> 1, 2, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, …
    ## $ TotalMinutesAsleep <int> 327, 384, 412, 340, 700, 304, 360, 325, 361, 430, 2…
    ## $ TotalTimeInBed     <int> 346, 407, 442, 367, 712, 320, 377, 364, 384, 449, 3…

#### 4.9.3 Convert ‘Id’ numbers to character: ‘hourly_steps’

``` r
hourly_steps <- hourly_steps %>%
  mutate(Id = as.character(Id))

glimpse(hourly_steps)
```

    ## Rows: 22,099
    ## Columns: 4
    ## $ Id        <chr> "1503960366", "1503960366", "1503960366", "1503960366", "150…
    ## $ Day       <chr> "2016-04-12", "2016-04-12", "2016-04-12", "2016-04-12", "201…
    ## $ Hour      <chr> "00:00:00", "01:00:00", "02:00:00", "03:00:00", "04:00:00", …
    ## $ StepTotal <int> 373, 160, 151, 0, 0, 0, 0, 0, 250, 1864, 676, 360, 253, 221,…

### 4.10 Check missing values if any

``` r
sum(is.na(daily_activity))
```

    ## [1] 0

``` r
sum(is.na(sleep_day))
```

    ## [1] 0

``` r
sum(is.na(hourly_steps))
```

    ## [1] 0

There are no missing values in either data frames.

### 4.11 Check duplicated values if any

``` r
sum(duplicated(daily_activity))
```

    ## [1] 0

``` r
sum(duplicated(sleep_day))
```

    ## [1] 3

``` r
sum(duplicated(hourly_steps))
```

    ## [1] 0

There are 3 duplicates in ‘sleep_day’.

### 4.12 Remove duplicates

Let’s remove the duplicates. We should get 410 remaining rows as result.

``` r
sleep_day <- sleep_day %>%
  distinct()

glimpse(sleep_day)
```

    ## Rows: 410
    ## Columns: 5
    ## $ Id                 <chr> "1503960366", "1503960366", "1503960366", "15039603…
    ## $ SleepDay           <dttm> 2016-04-12, 2016-04-13, 2016-04-15, 2016-04-16, 20…
    ## $ TotalSleepRecords  <int> 1, 2, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, …
    ## $ TotalMinutesAsleep <int> 327, 384, 412, 340, 700, 304, 360, 325, 361, 430, 2…
    ## $ TotalTimeInBed     <int> 346, 407, 442, 367, 712, 320, 377, 364, 384, 449, 3…

### 4.13 Check 0 values

#### 4.13.1 Check 0 values and create data frame ‘usage’ from ‘daily_activity’

I noticed there are many 0 entries in the ‘daily_activity’ data frame. I
was curious which columns contain the most 0 values. My assumption is
that these values appear as 0 because the users didn’t use this feature
in the app or the values have been omitted from the dataset for privacy
reasons (GPS location data).

I decided to create a data frame to display the results named
**‘usage’**. It might be useful later to visualize as information on
most used / least used features.

``` r
entry_name <- c("TotalSteps", "TotalDistance", "TrackerDistance", "LoggedActivitiesDistance", "VeryActiveDistance", "ModeratelyActiveDistance", "LightActiveDistance", "SedentaryActiveDistance", "VeryActiveMinutes", "FairlyActiveMinutes","LightlyActiveMinutes", "SedentaryMinutes", "Calories")

zero_value <- c(sum(daily_activity$TotalSteps == 0), sum(daily_activity$TotalDistance == 0), sum(daily_activity$TrackerDistance == 0), sum(daily_activity$LoggedActivitiesDistance == 0), sum(daily_activity$VeryActiveDistance == 0), sum(daily_activity$ModeratelyActiveDistance == 0), sum(daily_activity$LightActiveDistance == 0), sum(daily_activity$SedentaryActiveDistance == 0), sum(daily_activity$VeryActiveMinutes == 0), sum(daily_activity$FairlyActiveMinutes == 0), sum(daily_activity$LightlyActiveMinutes == 0), sum(daily_activity$SedentaryMinutes == 0), sum(daily_activity$Calories == 0))
# can be interpreted as not logged activity

non_zero_value <- c(sum(daily_activity$TotalSteps != 0), sum(daily_activity$TotalDistance != 0), sum(daily_activity$TrackerDistance != 0), sum(daily_activity$LoggedActivitiesDistance != 0), sum(daily_activity$VeryActiveDistance != 0), sum(daily_activity$ModeratelyActiveDistance != 0), sum(daily_activity$LightActiveDistance != 0), sum(daily_activity$SedentaryActiveDistance != 0), sum(daily_activity$VeryActiveMinutes != 0), sum(daily_activity$FairlyActiveMinutes != 0), sum(daily_activity$LightlyActiveMinutes != 0), sum(daily_activity$SedentaryMinutes != 0), sum(daily_activity$Calories != 0))
# can be interpreted as logged activity

usage <- data.frame(entry_name, zero_value, non_zero_value)

print(usage)
```

    ##                  entry_name zero_value non_zero_value
    ## 1                TotalSteps         77            863
    ## 2             TotalDistance         78            862
    ## 3           TrackerDistance         78            862
    ## 4  LoggedActivitiesDistance        908             32
    ## 5        VeryActiveDistance        413            527
    ## 6  ModeratelyActiveDistance        386            554
    ## 7       LightActiveDistance         85            855
    ## 8   SedentaryActiveDistance        858             82
    ## 9         VeryActiveMinutes        409            531
    ## 10      FairlyActiveMinutes        384            556
    ## 11     LightlyActiveMinutes         84            856
    ## 12         SedentaryMinutes          1            939
    ## 13                 Calories          4            936

There are a lot of 0 values in the distance-related columns.

#### 4.13.2 Check 0 values in ‘sleep_day’

``` r
print(paste("TotalSleeprecords: ", sum(sleep_day$TotalSleeprecords == 0)))
```

    ## [1] "TotalSleeprecords:  0"

``` r
print(paste("TotalMinutesAsleep: ", sum(sleep_day$TotalMinutesAsleep == 0)))
```

    ## [1] "TotalMinutesAsleep:  0"

``` r
print(paste("TotalTimeInBed: ", sum(sleep_day$TotalTimeInBed == 0)))
```

    ## [1] "TotalTimeInBed:  0"

No 0 values in the ‘sleep_day’ dataset.

#### 4.13.3 Check 0 values in ‘hourly_steps’

``` r
print(paste("Day: ", sum(hourly_steps$Day == 0)))
```

    ## [1] "Day:  0"

``` r
print(paste("Hour: ", sum(hourly_steps$Hour == 0)))
```

    ## [1] "Hour:  0"

``` r
print(paste("StepTotal: ", sum(hourly_steps$StepTotal == 0)))
```

    ## [1] "StepTotal:  9297"

There are a bunch of 0 values in the ‘hourly_steps’ dataset. These
values probably reflect the night hours when users are asleep.

### 4.14 Extract day from date and add new column

#### 4.14.1 Add column ‘Weekday’ to ‘daily_activity’

Calculating the day of week when the activity has been logged using the
`wday()` function.

``` r
daily_activity$Weekday <- wday(daily_activity$ActivityDate, label = TRUE, week_start = 1)

glimpse(daily_activity)
```

    ## Rows: 940
    ## Columns: 16
    ## $ Id                       <chr> "1503960366", "1503960366", "1503960366", "15…
    ## $ ActivityDate             <date> 2016-04-12, 2016-04-13, 2016-04-14, 2016-04-…
    ## $ TotalSteps               <int> 13162, 10735, 10460, 9762, 12669, 9705, 13019…
    ## $ TotalDistance            <dbl> 8.50, 6.97, 6.74, 6.28, 8.16, 6.48, 8.59, 9.8…
    ## $ TrackerDistance          <dbl> 8.50, 6.97, 6.74, 6.28, 8.16, 6.48, 8.59, 9.8…
    ## $ LoggedActivitiesDistance <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ VeryActiveDistance       <dbl> 1.88, 1.57, 2.44, 2.14, 2.71, 3.19, 3.25, 3.5…
    ## $ ModeratelyActiveDistance <dbl> 0.55, 0.69, 0.40, 1.26, 0.41, 0.78, 0.64, 1.3…
    ## $ LightActiveDistance      <dbl> 6.06, 4.71, 3.91, 2.83, 5.04, 2.51, 4.71, 5.0…
    ## $ SedentaryActiveDistance  <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …
    ## $ VeryActiveMinutes        <int> 25, 21, 30, 29, 36, 38, 42, 50, 28, 19, 66, 4…
    ## $ FairlyActiveMinutes      <int> 13, 19, 11, 34, 10, 20, 16, 31, 12, 8, 27, 21…
    ## $ LightlyActiveMinutes     <int> 328, 217, 181, 209, 221, 164, 233, 264, 205, …
    ## $ SedentaryMinutes         <int> 728, 776, 1218, 726, 773, 539, 1149, 775, 818…
    ## $ Calories                 <int> 1985, 1797, 1776, 1745, 1863, 1728, 1921, 203…
    ## $ Weekday                  <ord> K, Sze, Cs, P, Szo, V, H, K, Sze, Cs, P, Szo,…

Note: weekday names are in Hungarian due to my computer’s system
settings. (H = Monday, K = Tuesday, Sze = Wednesday, Cs = Thursday, P =
Friday, Szo = Saturday, V = Sunday)

#### 4.14.2 Add column ‘Weekday’ and ‘TotalMinutesAwake’ to ‘sleep_day’

Calculate the minutes users spend in time awake from ‘TotalTimeInBed’
and ‘TotalMinutesAsleep’.

``` r
sleep_day$Weekday <- wday(sleep_day$SleepDay, label = TRUE, week_start = 1)

sleep_day$TotalMinutesAwake <- (sleep_day$TotalTimeInBed) - (sleep_day$TotalMinutesAsleep)

glimpse(sleep_day)
```

    ## Rows: 410
    ## Columns: 7
    ## $ Id                 <chr> "1503960366", "1503960366", "1503960366", "15039603…
    ## $ SleepDay           <dttm> 2016-04-12, 2016-04-13, 2016-04-15, 2016-04-16, 20…
    ## $ TotalSleepRecords  <int> 1, 2, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, …
    ## $ TotalMinutesAsleep <int> 327, 384, 412, 340, 700, 304, 360, 325, 361, 430, 2…
    ## $ TotalTimeInBed     <int> 346, 407, 442, 367, 712, 320, 377, 364, 384, 449, 3…
    ## $ Weekday            <ord> K, Sze, P, Szo, V, K, Sze, Cs, Szo, V, H, K, Cs, P,…
    ## $ TotalMinutesAwake  <int> 19, 23, 30, 27, 12, 16, 17, 39, 23, 19, 46, 29, 27,…

### 4.15 Key steps taken in the Process Phase

- Viewed datasets one by one
- Compared columns
- Noted observations, decided to ignore ‘weight_log’ (too little
  information)
- Tested equality for values - unique Id and dates in ‘daily_activity’,
  ‘daily_intensities’, ‘daily_calories’, ‘daily_steps’
- Identified redundant data frames (‘daily_activity’ contains all the
  information)
- Chose datasets for the Analyze Phase: ‘daily_activity’, ‘hourly_steps’
  and ‘sleep_day’
- Converted dates to datetime
- Separated ‘ActivityHour’ column in ‘hourly_steps’ to ‘Day’ and ‘Hour’
- Converted Id numbers to character
- Checked missing values
- Checked and removed duplicates
- Checked 0 values, created data frame ‘usage’ displaying zero and
  non-zero values
- Created new column: ‘Weekday’ in ‘daily_activity’
- Created new column: ‘Weekday’ and ‘TotalMinutesAwake’ in ‘sleep_day’

## 5. Analyze Phase

Data frames used:

- **‘daily_activity’**
- **‘hourly_steps’**
- **‘sleep_day’**

### 5.1 Statistics

Some key statistics about the data frames using the `summary()`
function.

#### 5.1.1 ‘daily_activity’ summary

``` r
daily_activity %>%
  select(TotalSteps,TotalDistance, SedentaryMinutes, LightlyActiveMinutes, FairlyActiveMinutes, VeryActiveMinutes, Calories) %>%
  summary()
```

    ##    TotalSteps    TotalDistance    SedentaryMinutes LightlyActiveMinutes
    ##  Min.   :    0   Min.   : 0.000   Min.   :   0.0   Min.   :  0.0       
    ##  1st Qu.: 3790   1st Qu.: 2.620   1st Qu.: 729.8   1st Qu.:127.0       
    ##  Median : 7406   Median : 5.245   Median :1057.5   Median :199.0       
    ##  Mean   : 7638   Mean   : 5.490   Mean   : 991.2   Mean   :192.8       
    ##  3rd Qu.:10727   3rd Qu.: 7.713   3rd Qu.:1229.5   3rd Qu.:264.0       
    ##  Max.   :36019   Max.   :28.030   Max.   :1440.0   Max.   :518.0       
    ##  FairlyActiveMinutes VeryActiveMinutes    Calories   
    ##  Min.   :  0.00      Min.   :  0.00    Min.   :   0  
    ##  1st Qu.:  0.00      1st Qu.:  0.00    1st Qu.:1828  
    ##  Median :  6.00      Median :  4.00    Median :2134  
    ##  Mean   : 13.56      Mean   : 21.16    Mean   :2304  
    ##  3rd Qu.: 19.00      3rd Qu.: 32.00    3rd Qu.:2793  
    ##  Max.   :143.00      Max.   :210.00    Max.   :4900

#### 5.1.2 Observations from the ‘daily_activity’ summary

- Users take 7638 steps a day on average. According to the
  recommendations from CDC (Center for Disease Control and Prevention),
  most adults should aim for 10,000 steps per day for general fitness.
  (However, this number has been disputed.)
  ([Reference](https://www.medicalnewstoday.com/articles/how-many-steps-should-you-take-a-day))

- User are getting 21.16 very active minutes a day on average, which
  means around 148.12 minutes a week. CDC recommends 75 minutes of
  vigorous-intensity physical activity a week, so the FitBit users who
  participated in the survey are doing well in this area.
  ([Reference](https://www.cdc.gov/physicalactivity/walking/index.html))

- Users spend an average of 991.2 minutes = 16.52 hours of sedentary
  time a day! This number seems rather high. It is recommended that
  adults limit sedentary time and replace it with activity whenever
  possible.
  ([Reference](https://health.gov/sites/default/files/2019-09/Physical_Activity_Guidelines_2nd_edition.pdf))

- The average user burns 2304 calories a day. According to the U.S.
  Department of Health and Human Services, the average adult woman
  expends roughly 1,600 to 2,400 calories per day, and the average adult
  man uses 2,000 to 3,000 calories per day, but this is highly dependent
  on a lot of factors. FitBit users who participated in the survey fit
  into these categories, but we do not have enough information on users’
  weight, gender and age to accuaretly interpret this information.
  ([Reference](https://www.everydayhealth.com/weight/how-to-achieve-one-pound-of-weight-loss.aspx))

#### 5.1.3 ‘sleep_day’ summary

``` r
sleep_day %>%
  select(TotalSleepRecords,TotalMinutesAsleep,TotalTimeInBed,TotalMinutesAwake) %>%
  summary()
```

    ##  TotalSleepRecords TotalMinutesAsleep TotalTimeInBed  TotalMinutesAwake
    ##  Min.   :1.00      Min.   : 58.0      Min.   : 61.0   Min.   :  0.00   
    ##  1st Qu.:1.00      1st Qu.:361.0      1st Qu.:403.8   1st Qu.: 17.00   
    ##  Median :1.00      Median :432.5      Median :463.0   Median : 25.50   
    ##  Mean   :1.12      Mean   :419.2      Mean   :458.5   Mean   : 39.31   
    ##  3rd Qu.:1.00      3rd Qu.:490.0      3rd Qu.:526.0   3rd Qu.: 40.00   
    ##  Max.   :3.00      Max.   :796.0      Max.   :961.0   Max.   :371.00

#### 5.1.4 Observations from the sleep_day summary

- Most users sleep once a day for 419.5 minutes on average, which is
  roughly 7 hours. CDC recommends 7 or more hours of sleep per night for
  adults. They also emphasize the importance of good quality sleep.
  ([Reference](https://www.cdc.gov/sleep/about_sleep/how_much_sleep.html))

- The average participant spends 458.6 minutes in bed, little more than
  7.5 hours, meaning that they spend around 39 minutes awake in bed.
  Normal sleep for adults means that you fall asleep within 10 to 20
  minutes.
  ([Reference](https://www.healthline.com/health/healthy-sleep/how-long-does-it-take-to-fall-asleep#normal-sleep))

#### 5.1.5 ‘hourly_steps’ summary

``` r
hourly_steps %>%
  select(Hour,StepTotal) %>%
  summary()
```

    ##      Hour             StepTotal      
    ##  Length:22099       Min.   :    0.0  
    ##  Class :character   1st Qu.:    0.0  
    ##  Mode  :character   Median :   40.0  
    ##                     Mean   :  320.2  
    ##                     3rd Qu.:  357.0  
    ##                     Max.   :10554.0

- Users take an average of 320 steps per hour. As mentioned above, CDC
  recommends most adults to aim for 10,000 steps per day for general
  fitness, that means around 416 steps per hour. Users who participated
  in the survey lead rather sedentary lifestyles.

### 5.2 Exploratory data visualizations

#### 5.2.1 Vigorous physical activity and calories burned

``` r
ggplot(data = daily_activity, aes(x = VeryActiveMinutes, y = Calories, color = Calories)) +
  geom_point() +
  scale_color_binned(low = "#2f4b7c", high = "#fa7d88") +
  stat_smooth(method = lm) +
  labs(title = "The relationship between vigorous physical activity and \n the number of daily calories burned", x = "Vigorous activity (in minutes)", y = "No. of calories burned")
```

    ## `geom_smooth()` using formula 'y ~ x'

![](bellabeat_case_study_files/figure-gfm/scatter%20plot%20VeryActiveMinutes%20and%20Calories-1.png)<!-- -->

Positive relationship between very active minutes and total daily
calories burned. The more vigorous physical activity the users did, the
more calories they burned.

#### 5.2.2 Moderate physical activity and calories burned

``` r
ggplot(data = daily_activity, aes(x = FairlyActiveMinutes, y = Calories, color = Calories)) +
  geom_point() +
  scale_color_binned(low = "#2f4b7c", high = "#fa7d88") +
  stat_smooth(method = lm) +
  labs(title = "The relationship between moderate physical activity and \n the number of daily calories burned", x = "Moderate activity (in minutes)", y = "No. of calories burned")
```

    ## `geom_smooth()` using formula 'y ~ x'

![](bellabeat_case_study_files/figure-gfm/scatter%20plot%20FairlyActiveMinutes%20and%20Calories-1.png)<!-- -->

Users burn less calories with moderate activity.

#### 5.2.3 Light physical activity and calories

``` r
ggplot(data = daily_activity, aes(x = LightlyActiveMinutes, y = Calories, color = Calories)) +
  geom_point() +
  scale_color_binned(low = "#2f4b7c", high = "#fa7d88") +
  stat_smooth(method = lm) +
  labs(title = "The relationship between light physical activity and \n the number of daily calories burned", x = "Light activity (in minutes)", y = "No. of calories burned")
```

    ## `geom_smooth()` using formula 'y ~ x'

![](bellabeat_case_study_files/figure-gfm/scatter%20plot%20LightlyActiveMinutes%20and%20Calories-1.png)<!-- -->

#### 5.2.4 Sedentary activity and calories

``` r
ggplot(data = daily_activity, aes(x = SedentaryMinutes, y = Calories, color = Calories)) +
  geom_point() +
  scale_color_binned(low = "#2f4b7c", high = "#fa7d88") +
  stat_smooth(method = lm) +
  labs(title = "The relationship between sedentary activity and \n the number of daily calories burned", x = "Sedentary activity (in minutes)", y = "No. of calories burned")
```

    ## `geom_smooth()` using formula 'y ~ x'

![](bellabeat_case_study_files/figure-gfm/SedentaryMinutes%20and%20Calories-1.png)<!-- -->

Sedentary activity has no impact on the number of calories burned.

#### 5.2.5 Daily steps and calories burned

``` r
ggplot(data = daily_activity, aes(x = TotalSteps, y = Calories, color = Calories)) +
  geom_point() +
  scale_color_binned(low = "#2f4b7c", high = "#fa7d88") +
  stat_smooth(method = lm) +
  labs(title = "The relationship between the amount of daily steps and \n the number of calories burned", x = "No. of steps per day", y = "No. of calories burned")
```

    ## `geom_smooth()` using formula 'y ~ x'

![](bellabeat_case_study_files/figure-gfm/scatter%20plot%20TotalSteps%20and%20Calories-1.png)<!-- -->

Positive relationship between total daily steps taken and total calories
burned. The more steps the Fitbit users took, the more calories they
burned.

#### 5.2.6 Minutes asleep and total time in bed

``` r
ggplot(data = sleep_day, aes(x = TotalMinutesAsleep, y = TotalTimeInBed, color = TotalTimeInBed)) +
  geom_point() +
  scale_color_binned(low = "#2f4b7c", high = "#fa7d88") +
  stat_smooth(method = lm) +
  labs(title = "The relationship between the minutes asleep and the total time spent in bed", x = "Minutes asleep", y = "Total minutes in bed")
```

    ## `geom_smooth()` using formula 'y ~ x'

![](bellabeat_case_study_files/figure-gfm/scatter%20plot%20TotalMinutesAsleep%20and%20TotalTimeInBed-1.png)<!-- -->

The time most participants spent asleep and the time they spent in bed
is very similar. However, we found out earlier that they spend an
average of 39 minutes awake, which is higher than the ideal 10-20
minutes to fall asleep.

#### 5.2.7 Minutes asleep during the week

``` r
ggplot(data = sleep_day) +
  geom_col(mapping = aes(x = Weekday, y = TotalMinutesAsleep, fill = Weekday)) +
  scale_fill_manual(values = c("#003f5c", "#374c80", "#7a5195", "#bc5090", "#ef5675", "#ff764a", "#ffa600")) +
  labs(title = "Total minutes asleep during the week", x = "Day of the week", y = "Minutes asleep")
```

![](bellabeat_case_study_files/figure-gfm/minutes%20asleep%20during%20the%20week-1.png)<!-- -->

Users slept the most on Wednesdays.

#### 5.2.8 Number of sleep entries by users

``` r
sleep_day %>%
  group_by(Id) %>%
  summarize(no_of_entries = sum(Id != 0)) %>%
  ggplot() +
  geom_col(mapping = aes(x=reorder(Id, -no_of_entries), y = no_of_entries, fill = no_of_entries)) +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  labs(title = "Number of sleep entries by users", x = " ", y = "No. of entries") +
  theme(axis.text.x = element_text(angle = 90))
```

![](bellabeat_case_study_files/figure-gfm/sleep%20entries%20by%20users-1.png)<!-- -->

Not all users track their sleep consistently. From the 33 participants,
only 24 logged sleep data and only 12 of them have more than 20 logs for
the 2 month the data represents.

#### 5.2.9 Average time in bed

``` r
sleep_average <- sleep_day %>%
  group_by(Weekday) %>%
  summarize(avg_sleep_min = mean(TotalMinutesAsleep), avg_bed_min = mean(TotalTimeInBed), avg_awake_min = mean(TotalMinutesAwake))

head(sleep_average)
```

    ## # A tibble: 6 × 4
    ##   Weekday avg_sleep_min avg_bed_min avg_awake_min
    ##   <ord>           <dbl>       <dbl>         <dbl>
    ## 1 H                420.        457.          37.8
    ## 2 K                405.        443.          38.8
    ## 3 Sze              435.        470.          35.3
    ## 4 Cs               401.        435.          33.6
    ## 5 P                405.        445.          39.6
    ## 6 Szo              419.        460.          40.8

``` r
ggplot(data = sleep_average) +
  geom_col(mapping = aes(x = Weekday, y = (avg_sleep_min / 60), fill = Weekday)) +
  geom_hline(yintercept = 7) +
  scale_fill_manual(values = c("#003f5c", "#374c80", "#7a5195", "#bc5090", "#ef5675", "#ff764a", "#ffa600")) +
  labs(title = "Average time asleep during the week\ncompared to the recommended 7 hours", x = "Day of the week", y = "Average hours asleep")
```

![](bellabeat_case_study_files/figure-gfm/average%20sleep%20week-1.png)<!-- -->

#### 5.2.10 Average minutes awake by users

``` r
sleep_day %>%
  group_by(Id) %>%
  summarize(avg_awake_min = mean(TotalMinutesAwake)) %>%
  ggplot() +
  geom_col(mapping = aes(x = reorder(Id, -avg_awake_min), y = avg_awake_min, fill = avg_awake_min)) +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  geom_hline(yintercept = 20) +
  labs(title = "Average minutes awake by users\ncompared to the 20 minutes that is considered normal", x = " ", y = " ") +
  theme(axis.text.x = element_text(angle = 90))
```

![](bellabeat_case_study_files/figure-gfm/average%20minutes%20awake-1.png)<!-- -->

#### 5.2.11 Activity logged during the week

``` r
ggplot(data = daily_activity) +
  geom_bar(mapping = aes(x=Weekday, fill = Weekday)) +
  scale_fill_manual(values = c("#003f5c", "#374c80", "#7a5195", "#bc5090", "#ef5675", "#ff764a", "#ffa600")) +
  labs(title = "Number of logged activities during the week", x = "Day of the week", y = "No. of entries")
```

![](bellabeat_case_study_files/figure-gfm/bar%20chart%20activity%20weekday-1.png)<!-- -->

Tuesdays, Wednesday and Thursdays are the most active days, users have
the most entries on these days.

#### 5.2.12 Activities logged during the week by users

``` r
daily_activity %>%
  group_by(Id) %>%
  summarize(no_of_entries = sum(Id != 0)) %>%
  ggplot() +
  geom_col(mapping = aes(x = reorder(Id, -no_of_entries), y = no_of_entries, fill = no_of_entries)) +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  labs(title = "Number of logged activities by users", x = "User Id", y = "No. entries") +
  theme(axis.text.x = element_text(angle = 90))
```

![](bellabeat_case_study_files/figure-gfm/bar%20chart%20logged%20activity%20user-1.png)<!-- -->

Most participants used their device consistently during the two month of
the data collection.

#### 5.2.13 Number of steps during the week

``` r
  ggplot(data = daily_activity) +
  geom_col(mapping = aes(x=Weekday, y = TotalSteps, fill = Weekday)) +
  scale_fill_manual(values = c("#003f5c", "#374c80", "#7a5195", "#bc5090", "#ef5675", "#ff764a", "#ffa600")) +
  labs(title = "Total number of steps during the week", x = "Day of the week", y = "No. of steps")
```

![](bellabeat_case_study_files/figure-gfm/bar%20chart%20steps%20weekday-1.png)<!-- -->

Users took the most steps on Tuesdays.

#### 5.2.14 Average number of steps during the week by users

``` r
daily_activity %>%
  group_by(Id) %>%
  summarize(average_steps = mean(TotalSteps)) %>%
  ggplot() +
  geom_col(mapping = aes(x= reorder(Id, -average_steps), y = average_steps, fill = average_steps)) +
  geom_hline(yintercept = 10000) +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  labs(title = "Average number of daily steps by users\ncompared to the 10,000 steps recommendation", x = "User Id", y = " ") +
  theme(axis.text.x = element_text(angle = 90))
```

![](bellabeat_case_study_files/figure-gfm/bar%20chart%20steps%20user%20weekday-1.png)<!-- -->

#### 5.2.15 Average hourly steps

``` r
hourly_steps %>%
  group_by(Hour) %>%
  summarize(average_steps = mean(StepTotal)) %>%
  ggplot() +
  geom_col(mapping = aes(x = Hour, y = average_steps, fill = average_steps)) +
  labs(title = "Average number of steps during the day", x = " ", y = " ") +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  theme(axis.text.x = element_text(angle = 90))
```

![](bellabeat_case_study_files/figure-gfm/average%20hourly%20steps-1.png)<!-- -->

Most active hours are around lunchtime and after work.

#### 5.2.16 Sedentary activity during the week

``` r
ggplot(data = daily_activity) +
  geom_col(mapping = aes(x=Weekday, y = SedentaryMinutes, fill = Weekday)) +
  scale_fill_manual(values = c("#003f5c", "#374c80", "#7a5195", "#bc5090", "#ef5675", "#ff764a", "#ffa600")) +
  labs(title = "Sedentary activity during the week", x = "Day of the week", y = "Sedentary minutes")
```

![](bellabeat_case_study_files/figure-gfm/sedentary%20activity%20week-1.png)<!-- -->

#### 5.2.17 Average sedentary minutes by users

``` r
daily_activity %>%
  group_by(Id) %>%
  summarize(average_sedentary = mean(SedentaryMinutes)) %>%
  ggplot() +
  geom_col(mapping = aes(x = reorder(Id, -average_sedentary), y = average_sedentary, fill = average_sedentary)) +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  labs(title = "Average sedentary minutes by users", x = " ", y = "Sedentary minutes (average)") +
  theme(axis.text.x = element_text(angle = 90))
```

![](bellabeat_case_study_files/figure-gfm/average%20sedentary%20minutes%20user-1.png)<!-- -->

Users spend an average of 991.2 minutes = 16.52 hours of sedentary time
a day! They should be mindful of this and incorporate light activity to
their days.

#### 5.2.18 Summary of activity minutes

Create data frame **‘activity_df’**

``` r
activity <- c("Intense", "Moderate", "Light", "Sedentary")

total_minutes <- c(sum(daily_activity$VeryActiveMinutes), sum(daily_activity$FairlyActiveMinutes), sum(daily_activity$LightlyActiveMinutes), sum(daily_activity$SedentaryMinutes))

average_minutes <- c(mean(daily_activity$VeryActiveMinutes), mean(daily_activity$FairlyActiveMinutes), mean(daily_activity$LightlyActiveMinutes), mean(daily_activity$SedentaryMinutes))

activity_df <- data.frame(activity, total_minutes, average_minutes)

print(activity_df)
```

    ##    activity total_minutes average_minutes
    ## 1   Intense         19895        21.16489
    ## 2  Moderate         12751        13.56489
    ## 3     Light        181244       192.81277
    ## 4 Sedentary        931738       991.21064

``` r
ggplot(data = activity_df) +
  geom_col(mapping = aes(x = reorder(activity, -average_minutes), y = average_minutes, fill = average_minutes)) +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  labs(title = "Sedentary activity is very high", x = "Activity type", y = "Activity minutes")
```

![](bellabeat_case_study_files/figure-gfm/average%20activity%20minutes-1.png)<!-- -->

#### 5.2.19 Usage

``` r
ggplot(data = usage) +
  geom_col(mapping = aes(x = reorder(entry_name, -zero_value), y = zero_value, fill = zero_value)) +
  labs(title = "Missing entries by activity type", x = " ", y = "No. of missing entries") +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  theme(axis.text.x = element_text(angle = 90))
```

![](bellabeat_case_study_files/figure-gfm/missing%20entries-1.png)<!-- -->

``` r
ggplot(data = usage) +
  geom_col(mapping = aes(x = reorder(entry_name, -non_zero_value), y = non_zero_value, fill = non_zero_value)) +
  scale_fill_binned(low = "#2f4b7c", high = "#f95d6a") +
  labs(title = "Most documented activites", x = " ", y = "No. of entries") +
  theme(axis.text.x = element_text(angle = 90))
```

![](bellabeat_case_study_files/figure-gfm/most%20documented%20activities-1.png)<!-- -->

### 5.3 Analysis summary

#### 5.3.1 Key steps taken in the Analyze Phase

- Statistics and observations about the data frames
- Created exploratory data visualizations on the following topics:
  - relationship between the different activities and calories burned
  - sleep patterns during the week (time asleep, number of entries,
    average time awake)
  - activities logged during the week and by users
  - total and average number of steps during the week and during the day
  - sedentary activity, activity minutes comparison
  - app usage

#### 5.3.2 Key takeaways - Identified trends

**Relationship between activities and calories burned**

- Positive correlation between very active minutes and total daily
  calories burned.The more vigorous activities users did and the more
  steps they took, the more calories they burned.
- The average user burns 2304 calories per day.

**Steps**

- Users take 7638 steps a day on average. Most steps on Tuesdays. This
  is below the 10,000 steps recommendation of CDC.
- Users took the most steps between 11:00-14:00 and 17:00-19:00.

**Sleep**

- Users spend an average of 419 minutes asleep, little less than the
  recommended 7 hours.
- Around 39 minutes awake in bed, which is higher than the ideal 10-20
  minutes to fall asleep.
- One user recorded an extreme 300 awake minutes.

**Sedentary time and activities**

- Average of 991.2 minutes = 16.52 hours of sedentary time a day.
- Sedentary activity level is very high in this user group.
- Sedentary activity level is more than four times higher than intense,
  moderate and light activity levels together.
- However 21 minutes of intense activity per day on average = 147
  minutes a week, exceeding the recommended 75 minutes.

**Usage - documented activities**

- Most active days (most number of entries): Tuesday, Wednesday,
  Thursday
- Most users tracked their activities regularly during the week, only
  one user had an extremely low amount of entries.
- Lot of missing entries in distance related columns - people do not
  track this information or did not provide.
- Most users track their different activity levels (intense, moderate,
  light, sedentary) and calories.
- From the 33 participants, 24 logged sleep data and only 12 of them had
  more than 20 logs for the 2 month period the data represents.
- Only 8 users logged weight information.

## 6. Share and Act Phases

It is important to reiterate that the dataset used for this analysis had
many problems and limitations, so recommendations should be taken with
caution.

Furthermore, we have to keep in mind that the datasets used for the
analysis have been provided by FitBit users. FitBit’s products, services
and target audience are different from Bellabeat’s.

Bellabeat’s mission is to empower women with knowledge about their
health and habits, in order to understand how their bodies work and make
healthier choices.

### 6.1 Top recommendations for the Bellabeat app

**Promote physical activity through notifications, recommendations and
games**

- Notifications to get up from the desk during work hours or go for a
  walk after work.
- Short workout session recommendations for weekdays and suggestions on
  weekend activities.
- Reward system and games for those who don’t get motivated by
  notifications: reach different levels based on the amount of steps
  walked every day, gather points that are redeemable for discounts on
  other Bellabeat products.

**Help fall asleep faster and sleep better**

- Notifications for bedtime or start of the evening routine.
- Resources to help fall asleep: breathing techniques, relaxation
  exercises.
- Built-in meditation timer.

**Encourage users to log their activities and engage with the app more**

- Make manual entries hassle free: quick access options, favorites,
  widget.
- Community building option: connect with other users sharing similar
  health goals, share achievements.

**Collect and analyze further data focusing on women**

- Conduct similar survey among Bellabeat users and use data for
  analysis.
- Use larger sample group and include information on age group.
- Consider competitive intelligence research on wellness apps for women,
  including cycle and fertility tracker apps.
