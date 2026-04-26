# Digital-Twin-IoT
# Digital Twin IoT Pipeline Monitoring System

Python GIS project for pipeline monitoring using **Digital Twin + IoT + Spatial Analysis** concepts.

This project simulates an infrastructure monitoring system where sensors detect abnormal pipeline conditions, generate alerts, analyze proximity to water bodies, and visualize risks on an interactive map.

---

## Project Overview

The system combines:

* **IoT Sensors** — pressure / temperature monitoring
* **Digital Twin Logic** — virtual representation of pipeline segments
* **Spatial Analysis** — distance from incidents to water bodies
* **Risk Engine** — combines technical + environmental risk
* **Interactive Mapping** — Folium visualization

---

## Main Logic

### 1. Sensors

Each sensor stores:

* coordinates
* pressure
* temperature
* risk level

### 2. Segments

A segment is created between two sensors.

The system analyzes:

* pressure drop between sensors
* abnormal conditions
* midpoint of incident area

### 3. Alerts

If pressure loss exceeds threshold:

* alert is generated
* severity is assigned
* alert location is created

### 4. Water Risk Analysis

The project calculates distance from alert location to nearest water object.

Water layer source:

**OpenStreetMap**

### 5. Final Risk Score

Technical pipeline risk + environmental water risk are combined into one final severity level.

---

## Technologies Used

* Python
* Pandas
* GeoPandas
* Shapely
* Folium
* OOP (Classes)

---

## Project Structure

```text
Digital-Twin-IoT/

script.py
map3.html
README.md
```

---

## Map Output

Interactive map with:

* sensors
* pipeline segments
* alerts
* combined risk levels

Open file:

```text
map/map(3).png
```

---

## Example Use Cases

* Pipeline leak detection
* Pressure anomaly monitoring
* Environmental impact estimation
* Infrastructure risk visualization
* Digital Twin prototype systems

---

## Future Improvements

* Live sensor data stream
* Dashboard with charts
* Time-series monitoring
* Real pipeline datasets
* Web application version

---

## Author

Madina

---
