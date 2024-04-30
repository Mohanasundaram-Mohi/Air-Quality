# Beijing Air Quality - dashboard

I've just finished analysing the Beijing Air Quality. My dynamic Power BI dashboards delve deep into factors help to understand Humidity, harmful gases, rare compounds. 

 ## Here's what you can expect from this dashboard:

1. 1. Comprehensive Air Quality Insights: Average hourly Air contents month wise data. 

2. Dynamic Air Quality Analysis: Dive deep into various gases in the air. 

3. Represent the presents of different gases various charts. 

## Followed steps: 
Dashboard – Following preparation methods for creating below dashboard: 

Data cleaning : Carefully removed all null values and replaced with average values for all columns. Date and time merged using merging option. Used split column by position to align the data and time. 

DAX : Created new measure to find hottest date with time. 
Hottest date with time = CALCULATE(MAX(AirQualityUCI[Date and Time]),filter(AirQualityUCI,AirQualityUCI[Temperatue on C]=MAX(AirQualityUCI[Temperatue on C])))
 
Slicer – Essentially includes date and time, to select the range. 
DAX : Created new measure to find most Humid day. 
Most Humid day = CALCULATE(MAX(AirQualityUCI[Date and Time]),filter(AirQualityUCI,AirQualityUCI[Absolute Humidity]=MAX(AirQualityUCI[Absolute Humidity])))

Represent the presents of different gases by using stacked bar chart

Average presence of NO and NO2, Non Methane Hydro carbon for month and years. 

Harmful gases – Line charts

Donut chart for harmful gases. 

Utilize the table format for conditional formatting to show the degree of hotness increases.

![Screenshot (13)](https://github.com/Mohanasundaram-Mohi/Air-Quality/assets/168515064/104ce4ba-267a-46ac-8d46-296c36020ec7)



 
