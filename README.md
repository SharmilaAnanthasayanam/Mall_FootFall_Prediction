# Mall_FootFall_Prediction
This GitHub repository contains the code and resources for a machine learning project that predicts the footfall in a shopping mall. The model utilizes the various features such as Holiday , Weather data and special events to forecast the Incount..

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
  * Merge all three data sets on date.
  * Picking up data which exist in the date range 2011-01-01 to 2016-12-31.



