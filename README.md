# Weather-Analysis

🌤️ Weather Dashboard Project (Excel + MySQL + Power BI)
This project is a dynamic Weather Dashboard that visualizes real-time and forecast weather data using Excel for data preprocessing, MySQL for structured storage and queries, and Power BI for rich data visualization and reporting.
________________________________________
📌 Project Overview
The Weather Dashboard provides insights into:
•	Current temperature and conditions
•	Weekly forecast trends
•	Air Quality Index (AQI)
•	Sunrise and sunset times
•	Rain probability
•	Key atmospheric indicators (humidity, wind speed, pressure, UV index, etc.)
The data is gathered from external weather APIs and passed through an ETL (Extract, Transform, Load) pipeline for storage, analysis, and visualization.
________________________________________
🔧 Tools & Technologies Used
Tool	Purpose
Excel	Data cleaning, transformation, and intermediate storage
MySQL	Structured storage, relational queries, historical weather data
Power BI	Visual dashboards, reports, and interactive analytics
APIs	Weather and AQI data from OpenWeatherMap or AQICN
________________________________________
🗃️ Data Flow Architecture
css
CopyEdit
[Weather API] ---> [Excel: Clean & Structure] ---> [MySQL Database] ---> [Power BI: Dashboard & Reports]
________________________________________
📊 Dashboard Features
🟦 Current Weather Snapshot
•	Location-based temperature display (e.g., Bengaluru: 25.1°C, Partly Cloudy)
•	Cities dropdown: Bengaluru, Ajmer, Hyderabad
•	Humidity, wind speed, pressure, precipitation
📈 Forecast Weather (7 Days)
•	Line chart showing temperature trend
•	Daily conditions (icons and temperatures)
🌅 Sunrise & Sunset
•	Sunrise: 06:02 AM
•	Sunset: 06:49 PM
🌧️ Rain Probability
•	Daily % chance of rain (e.g., Friday: 96%)
🌍 Air Quality Index
•	PM10, PM2.5, NO2, SO2, CO, O3 values
•	Visual indicators (Green, Yellow, Red)
•	Overall AQI rating (Good/Moderate/Poor)
________________________________________
🧩 Database Design (MySQL)
Tables
•	weather_current
o	city, temperature, condition, humidity, wind_speed, pressure, visibility, uv_index, timestamp
•	weather_forecast
o	city, date, forecast_temp, condition
•	aqi_data
o	city, pm10, pm2_5, no2, so2, co, o3, timestamp
•	sun_data
o	city, sunrise_time, sunset_time, date
________________________________________
📥 Data Sources
•	🌐 OpenWeatherMap API
•	🌐 AQICN API
________________________________________
📌 How to Run
1.	Data Collection
o	Set up scheduled API pulls into Excel or use scripts (Python recommended for automation).
2.	Data Cleaning in Excel
o	Normalize formats, calculate derived columns, remove nulls
3.	Load into MySQL
o	Use Excel ODBC or CSV export to import data into MySQL
4.	Connect Power BI to MySQL
o	Use MySQL connector in Power BI
o	Design the dashboard layout based on KPIs
5.	Publish or Share
o	Publish to Power BI Service
o	Share dashboards with stakeholders
________________________________________
🚀 Future Enhancements
•	Automate data ingestion using Python or Power Query
•	Set up scheduled refresh in Power BI
•	Add drill-down for hourly data
•	Integrate real-time alerts for severe weather
________________________________________
📄 License
This project is licensed under the MIT License. You are free to use, modify, and distribute it with attribution.
________________________________________
🙏 Acknowledgments
•	OpenWeatherMap
•	AQICN
•	Microsoft Power BI
•	MySQL
•	Microsoft Excel
