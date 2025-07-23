## 🌦️ Weather & Air Quality Dashboard - Power BI

This project showcases an interactive and visually appealing Weather & Air Quality Dashboard built using Power BI. It provides real-time weather updates, a 7-day forecast, and air quality index (AQI) breakdowns for various pollutants.

## 📊 Features: 

🌡️ Temperature Details

Current temperature, weather condition, and city comparison

📅 7-Day Forecast Chart

Visual line chart showing temperature trend for the upcoming week

🌇 Sunrise & Sunset Times

💨 Atmospheric Details

Humidity, Wind Speed, Visibility, Pressure, UV Index, and Precipitation

🌫️ Air Quality Index (AQI)

PM10, PM2.5, NO2, SO2, CO, and O3 pollutant values

Status text and color-coded suggestions using DAX logic

🌧️ Rain Probability by Day

Horizontal bar chart with percentage chance of rain

## 🛠️ Tech Stack:
Power BI – Data modeling, visuals, and dashboard

DAX – Dynamic logic for AQI categories, colors & suggestions

Custom Visuals – KPI cards, line charts, gauges, etc.

CSV/JSON or API Data (optional) – For weather and AQI inputs

## 📌 Purpose :
To deliver a real-time, data-driven solution that:

Informs users about current and forecasted weather

Raises awareness about air quality and health advisories

Supports informed outdoor planning and lifestyle decisions

## 📷 Dashboard Preview:
<img width="1278" height="719" alt="Group 2 (28) (2)" src="https://github.com/user-attachments/assets/617464f7-3d44-4dc9-b213-4f5b1a712075" />


<img width="1329" height="745" alt="Screenshot 2025-07-23 054814" src="https://github.com/user-attachments/assets/134f1478-d014-4331-9cdf-047a44f4d307" />


## 🚀 Getting Started
Open Power BI Desktop

Load your weather data source (CSV, API, or sample)

Create visuals based on provided layout

Add DAX measures for:

AQI category detection

AQI color formatting

AQI suggestion text

## 🧠 Sample DAX Measures
```
AQI Suggestion =
VAR AQI = SELECTEDVALUE('Current'[current.air_quality.pm10])
RETURN
SWITCH(
    TRUE(),
    AQI <= 50, "Air is clean and healthy",
    AQI <= 100, "Acceptable air quality, stay active",
    AQI <= 150, "Sensitive groups should reduce outdoor time",
    AQI <= 200, "Limit prolonged outdoor exertion",
    AQI <= 300, "Avoid outdoor activity if possible",
    "Stay indoors, wear mask if outside"
)
```
## 📬 Contact
Created by Suraj Singh — feel free to connect via LinkedIn or explore more on GitHub

## 🏷️ Tags
#PowerBI #DataVisualization #WeatherDashboard #AQI #DAX #SurajSingh #PortfolioProject
