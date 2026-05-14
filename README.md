# Urban Sprawl Prediction in Hyderabad using GeoAI

> Team Project • Optical Remote Sensing (ORS), Spring 2026

A large-scale GeoAI and spatial machine learning project for predicting urban expansion in Hyderabad (2020–2050) using satellite imagery, Random Forest classification, Multinomial Logistic Regression, Genetic Algorithm optimization, and Cellular Automata simulation.

---

## Team

* Vishakha Agrawal
* Goni Anagha
* Gandlur Valli
* Nunna Sri Abhinaya

---

## Overview

This team project develops a hybrid GeoAI framework to model and simulate urban sprawl in Hyderabad Metropolitan Area using historical satellite imagery and spatial drivers.

The pipeline integrates:

* Remote sensing and land-use classification
* Spatial feature engineering
* Machine learning probability estimation
* Genetic Algorithm optimization
* Cellular Automata-based urban growth simulation
* Large-scale raster prediction over 2.86 million spatial cells

The model predicts future built-up expansion from 2020 to 2050 at 30 m spatial resolution.

---

## Key Highlights

* Processed multi-temporal Landsat imagery from 1990–2020
* Built Random Forest classifier for LULC classification
* Generated spatial probability surfaces using Multinomial Logistic Regression
* Optimized CA parameters using Genetic Algorithms
* Simulated urban expansion over 2.86M+ spatial cells
* Achieved high calibration and validation accuracy
* Developed interactive visualization atlas for spatial analysis

---

## Results

| Metric                         | Value         |
| ------------------------------ | ------------- |
| RF Classification Accuracy     | 80.12%        |
| RF Kappa Score                 | 0.735         |
| CA Calibration Accuracy        | 93.50%        |
| CA Validation Accuracy         | 93.48%        |
| Predicted Built-up Area (2050) | 1006.91 km²   |
| Growth from 2020 to 2050       | +120.4%       |
| Study Area Grid Size           | 1691 × 1691   |
| Spatial Cells Simulated        | 2.86 Million+ |

---

## Tech Stack

### Languages & Libraries

* Python
* NumPy
* Pandas
* Scikit-learn
* SciPy
* Matplotlib
* Rasterio
* GeoPandas
* geemap

### Geospatial & ML Tools

* Google Earth Engine
* Google Colab
* Random Forest Classification
* Multinomial Logistic Regression
* Cellular Automata
* Genetic Algorithms
* Raster Processing
* Remote Sensing
* Spatial Modeling

---

## Methodology

### Phase 1 — LULC Classification

Historical Landsat 5/7/8 imagery (1990–2020) was classified into:

* Water
* Vegetation
* Barren
* Built-up

A Random Forest classifier trained on ESA WorldCover 2020 reference data was used for classification.

---

### Phase 2 — Spatial Driver Extraction

Five spatial drivers were extracted and standardized:

* Slope
* Elevation
* Population Density
* Distance to Roads
* Distance to City Center

All drivers were tested for multicollinearity using Variance Inflation Factor (VIF).

---

### Phase 3 — Probability Estimation

A Multinomial Logistic Regression model generated spatial transition probabilities for urban growth.

The model produced continuous probability surfaces representing urbanization likelihood across the study area.

---

### Phase 4 — CA-GA Simulation

Cellular Automata simulation was combined with Genetic Algorithm optimization to model future urban expansion.

Optimized parameters:

* Neighborhood Weight (ω)
* Stochasticity (α)
* Iteration Count

---

### Phase 5 — Urban Growth Prediction

The final model simulated urban sprawl for:

* 2025
* 2030
* 2035
* 2040
* 2045
* 2050

using quota-based demand allocation and probability-driven spatial transitions.

---

## Study Area

* Hyderabad Metropolitan Area, India
* 25 km radius from city center
* Spatial Resolution: 30 m
* Projection: UTM Zone 43N

---

## Repository Structure

```text
urban-sprawl-prediction-hyderabad/
│
├── notebooks/
│   └── urban_growth_prediction_pipeline.ipynb
│
├── assets/
│   ├── figures/
│   └── maps/
│
├── report/
│   └── Report.pdf
│
├── outputs/
│   └── sample_results/
│
├── requirements.txt
└── README.md
```

---

## Interactive Visualization Atlas

The project includes an interactive visualization atlas with spatial analytics, temporal growth visualization, and urban expansion insights.

Features:

* Urban growth maps
* LULC evolution
* Spatial probability surfaces
* Driver analysis
* Growth trend visualizations
* Comparative scenario analysis

---

## ML Concepts Used

* Random Forest Classification
* Feature Engineering
* Probability Modeling
* Multinomial Logistic Regression
* Spatial Machine Learning
* Cellular Automata Simulation
* Genetic Algorithm Optimization
* Spatial Statistics
* Raster-based Prediction
* Multicollinearity Testing (VIF)

---

## Applications

* Urban Planning
* GeoAI Research
* Smart Cities
* Land Use Monitoring
* Spatial Decision Support Systems
* Urban Growth Forecasting
* Environmental Planning

---

## Future Improvements

* Streamlit deployment
* Real-time GIS dashboard
* XGBoost / Deep Learning comparison
* Temporal population forecasting
* GPU acceleration
* Interactive web mapping
* Explainable AI for spatial drivers

---

## Dataset Sources

| Dataset             | Source |
| ------------------- | ------ |
| Landsat 5/7/8       | USGS   |
| ESA WorldCover 2020 | ESA    |
| SRTM DEM            | NASA   |
| GHS-POP             | JRC    |
| OpenStreetMap Roads | OSM    |

---

## Author

Nunna Sri Abhinaya
B.Tech ECE — IIIT Hyderabad

---

## License

This project is intended for educational and research purposes.

---

## Keywords

GeoAI • Machine Learning • GIS • Remote Sensing • Urban Sprawl • Spatial AI • Satellite Imagery • Cellular Automata • Urban Growth Modeling • Geospatial Analysis
