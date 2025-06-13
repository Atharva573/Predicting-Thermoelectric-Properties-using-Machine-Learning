# Predicting-Thermoelectric-Properties-using-Machine-Learning
A ML project to predict key thermoelectric properties—Lattice Thermal Conductivity, Seebeck Coefficient, and Electrical Conductivity—using simple elemental descriptors. The model is trained on a broad dataset of ~5200 data points, leveraging techniques like XGBoost and Random Forest, achieving high accuracy in thermal conductivity predictions.

# ML-Based Prediction of Thermoelectric Properties

This repository contains code and data for building machine learning models that predict key thermoelectric properties **Lattice Thermal Conductivity** and **Seebeck Coefficient** using only elemental descriptors. These models attempts to eliminate the need for computationally intensive ab initio methods by enabling fast, data-driven predictions.

## 🔍 Motivation

Accurate prediction of thermoelectric performance is essential for the discovery and design of materials for energy conversion. Traditional methods like DFT are accurate but computationally expensive. This project uses machine learning to bridge the gap between accuracy and computational cost, enabling rapid screening of potential thermoelectric materials.

## 📘 Project Overview

- **Data:** 5205 samples, 880 unique compounds (mostly tellurides & selenides)
- **Features:** 18 elemental descriptors including atomic number, electronegativity, melting point, thermal conductivity, and temperature.
- **Targets:**  
  - Lattice Thermal Conductivity  
  - Seebeck Coefficient  

  ## 🧠 Algorithms Used
 
- K-Nearest Neighbors (KNN)  
- Random Forest Regressor (with and without RFE)  
- XGBoost Regressor (with and without RFE)

## 🎯 Performance Highlights

- **Lattice Thermal Conductivity**:  
  - XGBoost achieved **R² > 0.90** on test data  
  - Model captured temperature dependence accurately  
- **Seebeck Coefficient**:  
  - Random Forest & XGBoost performed well  
  - Feature importance aligned with domain knowledge  
  
## 🧪 Candidate Testing

Predictions were made on two test sets:
- **Candidate Set 1:** Telluride-family materials → High accuracy
- **Candidate Set 2:** Mixed-family materials → Model struggled due to unseen chemistry

## 🔍 Folder Structure
📁 data/ — training sets & candidate sets  
📁 notebooks/ — model training notebooks  
📁 candidate set/- Testing the model on unseen chemstries 
📄 README.md, LICENSE, requirements.txt  

## 📚 References

- [Machine-learning guided discovery of new thermoelectric materials](https://doi.org/10.1038/s41598-019-39278-z)  
- [ML for Lattice Thermal Conductivity Prediction](https://doi.org/10.1016/j.commatsci.2019.109155)  
- [Material Descriptors for Thermoelectrics](https://doi.org/10.1039/C4EE03157A)

