# AirWatch: Air Quality Monitoring and Pollution Alert System

**Student:** Umutoniwase Nizeyimana Queen | **ID:** 29394
**Course:** INSY 8311, Database Development with PL/SQL
**Instructor:** Eric Maniraguha

## Problem Statement
Air pollution readings are often stored in scattered files, so unhealthy
pollution days go unnoticed and are not acted on. Poor air quality
affects the health of city residents, especially children and people
with respiratory illness, and it is a growing concern in Kigali and
other cities as traffic and urbanisation increase.

## Objectives
**Main objective:** Build an Oracle PL/SQL database that stores,
validates and classifies air-quality readings and raises pollution alerts.

**Specific objectives:**
1. Store station, city and pollutant readings in 3NF tables.
2. Validate readings and block impossible values with triggers.
3. Classify readings into AQI health categories with a PL/SQL function.
4. Record every data change in an audit log.
5. Show pollution trends and alerts on a live dashboard.

## Data Source
Air Quality Data in India (2015-2020), Kaggle:
https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india
(about 29,000 daily records; licence to be confirmed on the dataset page)

## Innovation
Analytics dashboard: Power BI connected live to the Oracle database,
showing pollution trends by city and month and unhealthy-day alerts.

## Planned Tables
STATIONS, CITIES, POLLUTANTS, READINGS, ALERTS, AUDIT_LOG

## Planned PL/SQL Features
- Procedures: record_reading, generate_daily_alerts
- Function: get_aqi_category
- Cursor: monthly average per station
- Package: air_quality_pkg
- Triggers: a trigger blocks negative or impossible readings; an audit
  trigger logs every change to readings
- Exceptions: handle invalid station or pollutant

## References
See docs/research/research_log.md (APA references to be added).
