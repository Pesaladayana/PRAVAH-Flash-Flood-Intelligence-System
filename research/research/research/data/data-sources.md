# PRAVAH — Data Sources

PRAVAH is designed to combine multiple environmental, terrain,
hydrological and infrastructure data sources.

The system does not depend on a single data source.

---

## 1. Rainfall Data

### Primary Source — India Meteorological Department (IMD)

IMD provides rainfall observations, station rainfall information,
district-wise rainfall monitoring and rainfall forecasts.

### Data Used

- Rainfall amount
- Rainfall intensity
- Cumulative rainfall
- Historical rainfall
- Forecast rainfall

### PRAVAH Use

Rainfall data forms one of the main inputs for flood-risk prediction.

### Source

https://mausam.imd.gov.in/

---

## 2. Satellite Precipitation — NASA GPM IMERG

NASA's Integrated Multi-satellitE Retrievals for GPM (IMERG)
provides precipitation estimates using multiple satellite
observations.

IMERG provides precipitation information at frequent time intervals
and is particularly useful in areas where ground-based rainfall
measurements are limited.

### Data Used

- Precipitation rate
- Accumulated precipitation
- Historical precipitation

### PRAVAH Use

Used as an additional rainfall source and to reduce dependence
on ground stations.

### Source

https://gpm.nasa.gov/data/imerg

---

## 3. Terrain / Elevation Data

### Source — USGS SRTM

The Shuttle Radar Topography Mission (SRTM) provides global
digital elevation data.

### Data Used

- Elevation
- Slope
- Terrain characteristics
- Drainage-related terrain information

### PRAVAH Use

Terrain information is used to identify areas where topography
may increase flood exposure and to support impact assessment.

### Source

https://www.usgs.gov/centers/eros/science/usgs-eros-archive-digital-elevation-shuttle-radar-topography-mission-srtm

---

## 4. Indian Geospatial Data — ISRO Bhuvan

Bhuvan is ISRO's geospatial platform providing Indian Earth
observation and geospatial products.

Bhuvan provides access to various thematic datasets and
disaster-related information including flood-related products,
elevation data and other geospatial layers.

### Data Used

- Elevation
- Land use / land cover
- Flood hazard information
- Water bodies
- Satellite-derived information
- Other thematic layers

### PRAVAH Use

Used for terrain analysis, land characteristics and
historical/observed flood information.

### Sources

https://bhuvan.nrsc.gov.in/

https://bhuvan.nrsc.gov.in/nhp/about-portal

---

## 5. Soil Moisture Data

### Source — NASA SMAP / NASA-USDA Global Soil Moisture

NASA provides global soil-moisture datasets derived from
satellite observations and data assimilation.

### Data Used

- Surface soil moisture
- Subsurface soil moisture
- Soil moisture anomalies

### PRAVAH Use

Soil moisture can help represent the antecedent wetness of
an area and can be used as an additional feature for flood-risk
assessment.

### Source

https://earth.gsfc.nasa.gov/hydro/data/nasa-usda-global-soil-moisture-data

---

## 6. Water-Level / Hydrological Data

### Potential Sources

- Central Water Commission (CWC)
- National Hydrology Project
- State water-resource departments
- Local river/water-level sensors

### Data Used

- River water level
- River discharge
- Reservoir level
- Inflow
- Historical water levels

### PRAVAH Use

Water-level information can improve flood-risk assessment
near rivers and downstream areas.

For the prototype, simulated sensor data may be used where
live sensor access is unavailable.

---

## 7. IoT Sensor Data

### Prototype Source

Low-cost sensors can be connected using ESP32 or similar
microcontrollers.

### Possible Measurements

- Local rainfall
- Water level
- Soil moisture
- Temperature
- Other environmental parameters

### PRAVAH Use

Real-time local measurements can complement satellite,
weather and historical data.

If a sensor becomes unavailable, the system should continue
using available data sources while reducing prediction confidence.

---

## 8. Historical Flood Data

### Potential Sources

- Government disaster records
- Bhuvan flood products
- Satellite-derived flood maps
- Research datasets
- Historical disaster reports

### Data Used

- Previous flood locations
- Flood extent
- Flood frequency
- Historical severity
- Affected infrastructure

### PRAVAH Use

Historical events can be used for model training,
validation and vulnerability assessment.

---

## 9. Infrastructure and Population Data

### Possible Data

- Population
- Villages
- Roads
- Bridges
- Hospitals
- Schools
- Emergency shelters
- Critical infrastructure

### PRAVAH Use

These layers are used during impact assessment and
vulnerability prioritization.

Example:

Village A:
High flood risk + high population + vulnerable bridge

Village B:
High flood risk + low population + accessible terrain

The two locations should not necessarily receive the same
priority.

---

# Data Fusion

PRAVAH combines information from multiple sources:

Rainfall
+
Weather
+
Satellite
+
Terrain
+
Soil Moisture
+
Water Level
+
Historical Flood Data
+
Infrastructure Data
↓
Data Preprocessing & Fusion
↓
Flood Risk Prediction
↓
Confidence Assessment
↓
Impact Assessment
↓
Vulnerability Priority
↓
Risk-Aware Evacuation

---

# Prototype Data Strategy

The initial prototype will not require every data source
to be connected simultaneously.

The system can begin with:

1. Rainfall data
2. Terrain / elevation data
3. Historical flood data
4. Population / infrastructure information

Additional sources such as soil moisture, water-level sensors
and live IoT data can be integrated progressively.

This allows the prototype to remain feasible while maintaining
a scalable architecture.

---

# Important Limitation

Data availability and spatial/temporal resolution may vary
between regions and sources.

Therefore, PRAVAH treats data availability and reliability
as part of the decision-making process rather than assuming
that every input will always be available.
