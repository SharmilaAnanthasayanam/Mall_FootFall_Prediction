# Mall_FootFall_Prediction
This GitHub repository contains the code and resources for a machine learning project that predicts the footfall in a shopping mall. The model utilizes the various features such as Holiday , Weather data and special events to forecast the Incount.

Datasets:
1.[Footfall.csv](https://drive.google.com/file/d/18r0RLtEAYG3gwgFDtxhLxwwmw6JUWaq0/view?usp=drive_link)
2.[overall_weather.csv](https://drive.google.com/file/d/17bAO8ekwhryUgeJWTEJjiTGeNkKwo83i/view?usp=drive_link)
3.[Easter-Sundays.csv](https://drive.google.com/file/d/130doO_RkQI0CuGuuhclHStxa_day9mh4/view?usp=drive_link)
4.[schools_long_holidays.csv](https://drive.google.com/file/d/1y5kmKxg1B1kmCdlRAFuXojIqJxiawvif/view?usp=drive_link)
5.[UKbankholidays.csv](https://drive.google.com/file/d/1Jl2nSeiwv0WjaOxC76z8GBTWXvxOd71g/view?usp=drive_link)
6.[University_Long_Holidays.csv](https://drive.google.com/file/d/1Q2aImNhmPYPfsm_jLY0L5whqDb6K3KK9/view?usp=drive_link)

Steps taken for the Prediction:
*Data cleaning and understanding:
  * Footfall.csv:
    *Converted the date to year-date-month format
    *Checked for date range in the data. (The date range is 2009-01-01 to 2016-12-31)
    *Droped the columns that are redundant.
  * Holiday Data Sets
    * Combined the seperate holiday datasets.
    * Concatenated the holiday data and removed duplicates if any.
    * Converted the date to year-date-month format.
  * Weather Data set:
      * Converted the date to year-date-month format.
  * Merge all three data sets on date and left join with the Footfall dataset. Fill the Null values in Holiday Data set and Weather dataset with N and Nan as required.
  * Picking up data which exist in the date range 2011-01-01 to 2016-12-31.
  * We now have the hourly dataset which has the incount for each hour in a day in a location.
  * Let us extract the data as daily Incount in a location by removing the hour column and aggregating the Incount for a day in a Location.
  * Pick the required data range and Remove the Incount column and duplicate data.
* Data Visualization:
 * Extract the data in following methods to vizualize in various cases.
    * Mall Level daywise Dataset: Previously we had hourly data and we aggregated it to daywise in each Location. Now we aggregate Incount value to Mall Level.
    * LocationName level daywise data: Aggregated Incount on Location Name and Date.
    * LocationName level daywise data in pivoted format
 * Observation based on Visualization:
    * There is an upward trend in the footfall year on year.
    * There is an upward trend in the footfall from August till december. December month has the highest footfall.
    * There is a gradual increase in footfall from Sunday to Saturday , saturday being the highest.




