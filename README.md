# Biltong Drying: Data Analysis & Machine Learning

## tl;dr
A data processing and machine learning model to predict biltong curing times based on temperature and humidity.

---

This project explores how temperature and humidity impact the drying process of biltong (jerky). Data was collected using custom-built hardware that logged environmental conditions to an SD card during multiple drying cycles.

The project consists of two main components:
1. **`Biltonger_data_analysis.ipynb`** – Handles data collection, processing, and statistical analysis.
2. **`Bilton_ML.ipynb`** – Uses the processed data to train a machine learning model.

The goal is to predict curing time using current temperature, humidity, and three lagging weight measurements. The model, a Random Forest Regressor, provides real-time estimates of drying progress and identifies optimal drying conditions.

---

## Visual Overview

### Raw Data from a Batch
![Typical data from a drying session](assets/biltong-batch-12.png "Typical data from a drying session")
*Example of raw data collected during a single biltong batch.*

### Environmental Risk Zones
![Environmental risk zones with key stats](assets/all-data-golden-biltong-curve.png "Environmental risk zones with key stats")
*Red zone indicates high risk of mold due to slow drying. Green zone typically results in safe, effective curing.*

### Curve Fitting
![Fitted curve over processed data](assets/curve-fitted-golden-biltong-curve.png "Fitted curve over processed data")
*Processed data used to compute mean, standard deviation, and apply a fitted curve.*

### Overlay of All Batches
![All batches with fitted curve](assets/golden-biltong-curve.png "All batches with fitted curve")
*Each batch plotted over the fitted curve for trend comparison.*

### Predictive Modeling
![Machine learning model predictions](assets/predicted-weight-over-time.png "Machine learning model predictions")
*Random Forest Regressor predicts weight loss over time based on environmental inputs.*

### 3D Heatmap: Curing Time Prediction
![3D curing time prediction](assets/time-to-cure-3d.png "3D curing time prediction")
*Model output shown as a 3D heatmap using humidity and temperature as inputs.*

---

## License

This work is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).

You are free to:
- **Share** — copy and redistribute the material in any medium or format  
- **Adapt** — remix, transform, and build upon the material  

Under the following terms:
- **Attribution** — You must give appropriate credit to [Nordtus.com](https://nordtus.com), provide a link to the license, and indicate if changes were made.  
- **NonCommercial** — You may not use the material for commercial purposes.  
- **Redistribution** — You may share this work, with attribution, but not for commercial gain.

