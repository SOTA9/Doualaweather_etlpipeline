Overview
========
DoualaWeather_Pipeline is a data pipeline project designed to extract weather data for Douala, Cameroon from a public weather API. The pipeline performs lightweight transformations on the data and loads it into a PostgreSQL database. This ETL process is automated and orchestrated using Apache Airflow, deployed and scheduled via Astronomer.
It is scheduled to capture the weather conditions in Douala, Cameroon, every 3 hours. Using Apache Airflow via astronomer, this system automates the collection and storage of weather data, enabling the continuous monitoring of weather patterns in the region.

The collected weather data includes key metrics like temperature, wind direction, wind speed, and weather code, which are fetched from an external weather API. The data is processed and stored in a Postgres database for further analysis and reporting.

Features
================

- API integration: Connects to a public weather API to fetch current weather data.
- Data Transformation: Processes raw data to extract and clean key weather attributes: Temperature, Wind Speed , Wind Direction.
- PostgreSQL Loading: Stores transformed data in a PostgreSQL database for downstream analytics or monitoring.
- Airflow Orchestration: Pipeline runs are scheduled and monitored using Airflow.
- Astronomer Deployment: Airflow is deployed via Astronomer for reliable and scalable execution.

Setup Instructions
===========================
Prerequisites

- Docker
- Astronomer CLI
- PostgreSQL database
- API Key for weather provider (e.g., OpenWeatherMap)

Technologies Used
=================================
- Python
- Apache Airflow
- Astronomer
- PostgreSQL
- Requests (for API calls)
- Docker


Example Output (Sample Data)
=================================
| timestamp              | temperature(°C) | wind_speed (m/s) | wind_direction (°)     |
|------------------------|-----------------|------------------|------------------------|
| 2025-05-09 14:00:00    | 30.1	           | 3.4              |       190              |



