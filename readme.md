# CNT Vibration Prediction Project

This project involves predicting the frequency and displacement for five modes of a mechanical system using various machine learning models. The models implemented include Extreme Gradient Boosting (XGBoost), CatBoost, Random Forest, and Neural Networks.

## Table of Contents

- [Project Overview](#project-overview)
- [Data](#data)
- [Preprocessing](#preprocessing)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Results](#results)
- [Requirements](#requirements)
- [License](#license)

## Project Overview

The goal of this project is to develop models that can accurately predict the frequency and displacement for five modes in a mechanical system. These predictions are critical for understanding the dynamic response of the system under various conditions.

## Data

The dataset contains various features related to mechanical and environmental conditions, such as current magnitude, stiffness coefficient, mass coefficient, and thermal conditions. The target variables include the frequency and displacement for each of the five modes.

### Data Features

- **Current_Mag**: Current Magnitude (mA)
- **Current_Phase**: Current Phase Angle (degree)
- **Stiff_Coeff**: Stiffness Coefficient
- **Mass_Coeff**: Mass Coefficient
- **Thermal_Cond_Mag**: Thermal Condition Magnitude (C)
- **Env_Temp**: Transient Environment Temperature (C)
- **Pressure_Mag**: Pressure Magnitude (hbar)
- **Magnetic_Flux_Max**: Magnetic Flux Density Maximum (mT)
- **Force_Max**: Force Maximum (N)
- **Mag_Field_Int_Max**: Magnetic Field Intensity Maximum (mA mm^-1)
- **Mag_Field_Int**: Magnetic Field Intensity (mA mm^-1)
- **mode1_displacement** to **mode5_displacement**: Displacements for modes 1 to 5 (mm)
- **mode1_frequency** to **mode5_frequency**: Frequencies for modes 1 to 5 (Hz)

## Preprocessing

### Data Cleaning

- Missing values were handled using interpolation techniques.
- Stability columns were dropped as they were not necessary for the prediction tasks.
- Columns were renamed for simplicity and clarity.

### Feature Scaling

- Features were scaled using standardization techniques to ensure all input features have similar scales, which is particularly important for models like neural networks.

## Modeling

The following models were implemented:

- **Extreme Gradient Boosting (XGBoost)**
- **CatBoost**
- **Random Forest**
- **Neural Networks**

The models were trained and validated using an 80-20 split of the dataset, with early stopping implemented to prevent overfitting.

## Evaluation
The models were evaluated using Mean Squared Error (MSE) and R-squared (R²) metrics. Professional plots were generated to compare the performance of each model across the five modes.

## Results
The performance of each model was compared, and the best-performing model was selected based on the evaluation metrics. Detailed plots are provided in the results directory.

## Requirements
Python 3.x
Pandas
NumPy
Matplotlib
Seaborn
Plotly
Scikit-learn
TensorFlow
XGBoost
CatBoost
Install the required packages using:

`pip install -r requirements.txt`<br>
Run the script to train the models and generate predictions:

## License
This project is licensed under the MIT License - see the LICENSE file for details.
