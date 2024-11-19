# Energy Demand Prediction Project

## Overview
This project serves as the culmination of my college journey, representing the final project before graduating from Loyola College. Over the past three years, I've worked on approximately 20 different projects, each contributing to my growth as a student and aspiring professional. This capstone project encapsulates the skills, knowledge, and experiences gained throughout my academic career.

## Motivation
Projects have been an integral part of my college experience, bridging the gap between theory and practice. They provided opportunities to tackle real-world problems, collaborate with peers, and develop essential skills such as problem-solving, critical thinking, and communication. This final project serves as a testament to my journey and the invaluable lessons learned along the way.

## Project Description
The project focuses on predicting energy demand using machine learning techniques. Leveraging historical data on various energy generation sources, weather conditions, and other relevant factors, the goal is to develop a predictive model that can forecast energy demand accurately. The project encompasses data preprocessing, exploratory data analysis, feature engineering, model training, and evaluation.

## Dataset
The dataset consists of two CSV files:
- `electricity_data.csv`: Contains information about electricity generation from different sources and actual load.
- `weather_data.csv`: Contains weather-related data such as temperature, pressure, humidity, wind speed, and cloud cover.

## Notebook
The notebook `Energy_Demand_Prediction.ipynb` provides a step-by-step walkthrough of the project, including data exploration, preprocessing, model development, and evaluation. It also includes detailed explanations of the code and insights derived from the analysis.

## Future Work
1. Incorporate additional features to enhance model performance.
2. Explore alternative machine learning algorithms for comparison.
3. Deploy the project to a cloud platform for wider accessibility.
4. Continuously update and refine the model with new data.

## Acknowledgments
I would like to express my gratitude to Loyola College, my professors, peers, and mentors for their support and guidance throughout this journey.

---

## Data Science Project Lifecycle
1. **Business Understanding**: Define the business goal and understand the problem to be solved.
2. **Data Collection and Understanding**: Identify relevant data sources and explore data structure and relevance.
3. **Data Preparation**: Clean, integrate, treat missing values, handle outliers, and format data for analysis.
4. **Exploratory Data Analysis**: Gain insights through visualization and understand factors affecting the model.
5. **Feature Engineering**: Select, derive new features, and prepare data for modeling.
6. **Modeling**: Build predictive models using machine learning algorithms.
7. **Model Evaluation**: Rigorously evaluate models to select the best-performing one for deployment.
8. **Model Deployment**: Deploy the selected model in a production environment for predictions or recommendations.

---

## Business Understanding
The main objective of using the dataset for the project "The Hourly Energy Equation: Balancing Supply and Demand in Real-Time" is to develop a model that can accurately forecast hourly energy consumption and generation in Spain, balancing supply and demand in real-time. This forecasting model will be used to optimize the energy infrastructure and ensure a reliable and efficient energy supply.

---

## Problem Statement
The energy sector is undergoing a radical transformation, with the transition to renewable energy sources and the need to balance supply and demand in real-time becoming increasingly important. The main challenges facing the power grid are the integration of bidirectional energy flows, the management of non-dispatchable generation, and the deployment of a digital telecommunications infrastructure that allows control and automation.

In the context of this project, the problem statement can be defined as: "How can we develop a model that accurately forecasts hourly energy consumption and generation in Spain, balancing supply and demand in real-time, using the provided dataset of electrical consumption, generation, pricing, and weather data for Spain?"

The objective is to create a model that can handle the changing demand for electricity and the use of different energy sources in today's fast-changing world, ensuring a reliable and efficient energy supply. This model will be used to optimize the energy infrastructure and maintain a high level of reliability in the power grid.

---

## References
- [ENTSOE](#): European Network of Transmission System Operators for Electricity
- [REE](#): Red Electrica de Espana (Spanish TSO)

---

## Data Understanding - Short Explanation of Columns

### Electricity Data
1. **Time (Datetime Index Localized to CET)**:
   Represents the temporal aspect of the dataset, with a datetime index localized to Central European Time (CET).
   
2. **Fossil Generation**:
   - Biomass: Biomass generation in MW.
   - Brown Coal/Lignite: Coal/lignite generation in MW.
   - Coal-Derived Gas: Coal gas generation in MW.
   - Fossil Gas: Gas generation in MW.
   - Fossil Hard Coal: Hard coal generation in MW.
   - Fossil Oil: Oil generation in MW.
   - Fossil Oil Shale: Shale oil generation in MW.
   - Fossil Peat: Peat generation in MW.
   
3. **Hydro Generation**:
   - Pumped Storage Aggregated: Hydro1 generation in MW.
   - Pumped Storage Consumption: Hydro2 generation in MW.
   - Run-of-River and Poundage: Hydro3 generation in MW.
   - Water Reservoir: Hydro4 generation in MW.
   
4. **Renewable Generation**:
   - Geothermal: Geothermal generation in MW.
   - Marine: Sea generation in MW.
   - Solar: Solar generation in MW.
   - Waste: Waste generation in MW.
   - Wind Offshore: Wind offshore generation in MW.
   - Wind Onshore: Wind onshore generation in MW.
   
5. **Forecast Solar Day Ahead**:
   Reflects the forecasted solar generation, providing an estimate of solar electricity generation for the next day.
   
6. **Forecast Wind Offshore Eday Ahead**:
   Represents the forecasted offshore wind generation, offering an estimate of offshore wind electricity generation for the next day.
   
7. **Forecast Wind Onshore Day Ahead**:
   Indicates the forecasted onshore wind generation, offering an estimate of onshore wind electricity generation for the next day.
   
8. **Total Load Forecast**:
   Reflects the forecasted electrical demand, providing an estimate of the total electricity demand for a specific period.
   
9. **Total Load Actual**:
   Quantifies the actual electrical demand, indicating the real-time total electricity demand for a specific period.
   
10. **Price Day Ahead**:
    Represents the forecasted electricity price in euros per megawatt-hour (EUR/MWh) for a specific period.
    
11. **Price Actual**:
    Indicates the actual electricity price in euros per megawatt-hour (EUR/MWh) for a specific period.

### Weather Data
1. **DateTime and Location**:
   - dt_iso: Datetime index localized to CET.
   - city_name: Name of the city.
   
2. **Temperature and Pressure**:
   - temp: Temperature in Kelvin.
   - temp_min: Minimum temperature in Kelvin.
   - temp_max: Maximum temperature in Kelvin.
   - pressure: Atmospheric pressure in hPa.
   
3. **Humidity and Wind**:
   - humidity: Humidity in percentage.
   - wind_speed: Wind speed in m/s.
   - wind_deg: Wind direction.
   
4. **Precipitation and Snow**:
   - rain_1

h: Rain in the last hour in mm.
   - rain_3h: Rain in the last 3 hours in mm.
   - snow_3h: Snow in the last 3 hours in mm.
   
5. **Cloud Cover and Weather Description**:
   - clouds_all: Cloud cover in percentage.
   - weather_id: Code used to describe weather.
   - weather_main: Short description of current weather.
   - weather_description: Long description of current weather.
   - weather_icon: Weather icon code for the website.
