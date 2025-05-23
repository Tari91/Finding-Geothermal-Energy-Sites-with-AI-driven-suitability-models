# Geothermal Site Suitability Prediction

This project demonstrates a machine learning pipeline for classifying the suitability of geographic sites for geothermal energy development. It uses a synthetic dataset to train and evaluate a Random Forest classifier.

## 🔍 Overview

The dataset simulates 1,000 geothermal sites with the following features:
- **temperature_gradient (°C/km)**: Subsurface temperature change with depth
- **heat_flow (mW/m²)**: Thermal energy transfer rate
- **rock_permeability (mD)**: Ability of rocks to transmit fluids
- **seismic_activity (0–10)**: Local seismic magnitude
- **water_availability (0–1)**: Normalized measure of water accessibility

A binary target label `suitable` indicates whether the site meets ideal geothermal criteria.

## 🧠 Machine Learning Workflow

1. **Data Generation**: Synthetic features are sampled from realistic distributions.
2. **Labeling**: Sites are marked as suitable (`1`) if they meet thresholds on all features.
3. **Training**: A `RandomForestClassifier` is trained on 80% of the data.
4. **Evaluation**: Accuracy, precision, recall, and confusion matrix are computed on the test set.
5. **Prediction**: Model predicts suitability for new site samples.

## 📁 Files

- `synthetic_geothermal_data.xlsx`: The dataset used in this project.
- `geothermal_model.py`: Python script for training and evaluation.
- `README.md`: Project documentation.

## 🛠 Requirements

- Python 3.7+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Install dependencies:
```bash
pip install -r requirements.txt
📈 Sample Output
Confusion matrix and classification report printed after training, with predictions made on new data points.

👤 Author
Tarinabo williamtarinabo@gmail.com
