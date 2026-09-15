# PRAVAH — Research Gap

## 1. Background

Research and existing systems have demonstrated the use of rainfall monitoring, satellite data, GIS, hydrological measurements and machine learning for flood prediction and susceptibility assessment.

However, practical challenges remain when these approaches are applied to rapidly developing flash floods in hilly regions.

---

## 2. Identified Gaps

### Gap 1 — Data Availability

Hilly and remote regions may have limited monitoring stations and incomplete hydrological measurements.

### PRAVAH Approach

Use multiple available data sources instead of depending on a single sensor.

Rainfall + Weather + Satellite + Terrain + Historical Data + IoT

---

### Gap 2 — Data and Prediction Uncertainty

Sensors can fail, forecasts can contain errors and some data may be unavailable.

### PRAVAH Approach

Introduce a Data Reliability and Confidence layer.

Example:

Flood Risk: HIGH
Probability: 82%
Confidence: 68%

If important data becomes unavailable, prediction confidence can be reduced.

---

### Gap 3 — Prediction Does Not Equal Impact

Knowing that a flood is likely does not directly indicate which villages, roads or infrastructure will be affected.

### PRAVAH Approach

Use terrain and hazard information to estimate potential impact areas.

Flood Risk
↓
Terrain Analysis
↓
Potentially Affected Areas
↓
Village / Infrastructure Impact

---

### Gap 4 — Different Areas Have Different Vulnerability

Two locations may have similar flood risk but different levels of exposure.

Factors include:

- Population
- Elevation
- Roads
- Bridges
- Critical infrastructure
- Accessibility
- Historical vulnerability

### PRAVAH Approach

Generate a vulnerability priority score to help identify areas requiring earlier attention.

---

### Gap 5 — Shortest Route May Not Be Safest

A conventional shortest-path algorithm may recommend a road or bridge that becomes dangerous during flooding.

### PRAVAH Approach

Consider current hazard conditions while selecting evacuation routes.

Shortest Route
≠
Safest Route

---

### Gap 6 — Rapidly Changing Conditions

Flash-flood conditions can change quickly because of rainfall, water levels and terrain-related processes.

### PRAVAH Approach

Continuously update risk, impact and evacuation information as new data becomes available.

---

# 3. Research Gap Summary

Existing approaches provide valuable capabilities for:

- Flood prediction
- Flood susceptibility mapping
- Rainfall monitoring
- Remote sensing
- Hydrological monitoring
- Emergency warnings

However, there is a need to better connect these capabilities with:

Data Reliability
+
Impact Assessment
+
Vulnerability Prioritization
+
Risk-Aware Evacuation
+
Continuous Updating

---

# 4. PRAVAH's Focus

PRAVAH aims to bridge the gap between flood prediction and emergency decision-making.

Multi-Source Data
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
↓
Alert & Continuous Update

---

## Key Research Gap Statement

"Existing flood prediction approaches can identify the likelihood of flooding, but translating uncertain multi-source information into localized impact assessment, vulnerability prioritization and safer evacuation decisions remains a practical challenge."

---

## Important Note

PRAVAH does not claim that these individual techniques are new.

The proposed contribution is their integration into a continuously updating decision-support workflow focused on hilly-region flash floods.
