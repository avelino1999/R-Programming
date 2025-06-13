# 🚲 Capital Bikeshare Data Analysis

This project analyzes bike-sharing data from Capital Bikeshare using R. It explores ride behaviors, distance traveled, and usage patterns between casual users and members across various bike types and time periods.

## 📁 Dataset

The dataset used is `rides_2020_2021_extract.csv`, which contains ride-level details such as:

- `ride_id`
- `member_casual` (User type)
- `rideable_type` (Bike type)
- `start_date`, `end_date`
- `start_station_name`, `end_station_name`
- `start_lat`, `start_lng`, `end_lat`, `end_lng`
- `total_time`

## 🧼 Data Cleaning

Key cleaning and transformation steps:
- Converted time columns to `POSIXct`.
- Converted coordinates to numeric.
- Standardized column names using `janitor::clean_names()`.
- Removed `NA` values for analysis accuracy.

## 📊 Analysis Performed

### ✅ 1. Ride Distribution by Time of Day
Bar chart showing ride counts by hour for members vs. casual users.

### ✅ 2. Average Distance Traveled by Bike Type
Used the Haversine formula (`distHaversine`) to compute average trip distance by bike type.

### ✅ 3. Top 5 Start Stations
Identified and visualized the most popular starting stations for each user type.

### ✅ 4. Weekday vs. Weekend Ride Share
Grouped rides into weekday/weekend categories and visualized the ride percentage using a pie chart.

## 📦 Tools & Libraries Used

- `tidyverse` (for data wrangling and visualization)
- `geosphere` (for distance calculations)
- `lubridate` (for handling dates and time)
- `janitor` (for cleaning column names)
- `ggplot2` (for plotting)


- Bar charts for usage by hour and user type
- Column plots for distance by bike type
- Pie charts for weekday vs. weekend ride share

## 📂 Folder Structure

