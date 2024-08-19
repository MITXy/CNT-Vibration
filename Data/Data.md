# Data Description

This dataset contains various features related to mechanical and environmental conditions, which are used to predict the frequency and displacement of a mechanical system across five modes. Below is a comprehensive description of each feature and target variable included in the dataset.

## Features

### Mechanical and Environmental Conditions

1. **Current_Mag**: Current Magnitude (mA)
   - Represents the electrical current magnitude in milliamperes (mA).
   - This feature is crucial as current can influence the magnetic fields and thus affect the mechanical vibrations.

2. **Current_Phase**: Current Phase Angle (degree)
   - The phase angle of the current, measured in degrees.
   - This feature helps in understanding the phase relationship between voltage and current, impacting the electromagnetic forces in the system.

3. **Stiff_Coeff**: Stiffness Coefficient
   - Represents the stiffness of the mechanical system.
   - Higher stiffness generally leads to higher natural frequencies and influences the system's response to vibrations.

4. **Mass_Coeff**: Mass Coefficient
   - The mass of the system or component.
   - The mass plays a critical role in determining the vibrational characteristics, with more massive systems generally having lower natural frequencies.

5. **Thermal_Cond_Mag**: Thermal Condition Magnitude (C)
   - The temperature of the system, measured in degrees Celsius (°C).
   - Temperature changes can affect material properties and thus the dynamic response of the system.

6. **Env_Temp**: Transient Environment Temperature (C)
   - The temperature of the surrounding environment, measured in degrees Celsius (°C).
   - Environmental temperature can impact the thermal expansion and contraction of materials, influencing vibrational characteristics.

7. **Pressure_Mag**: Pressure Magnitude (hbar)
   - The pressure applied to the system, measured in hectobars (hbar).
   - Pressure affects the density and stiffness of materials, altering their vibrational properties.

8. **Magnetic_Flux_Max**: Magnetic Flux Density Maximum (mT)
   - The maximum magnetic flux density, measured in milliteslas (mT).
   - Magnetic flux affects the force on charged particles within the system, impacting the overall vibrational behavior.

9. **Force_Max**: Force Maximum (N)
   - The maximum force exerted on the system, measured in newtons (N).
   - Force is directly related to the vibrational response, with higher forces generally causing more significant displacements.

10. **Mag_Field_Int_Max**: Magnetic Field Intensity Maximum (mA mm^-1)
    - The maximum intensity of the magnetic field, measured in milliamperes per millimeter (mA/mm).
    - This feature is important for understanding the magnetic forces at play within the system.

11. **Mag_Field_Int**: Magnetic Field Intensity (mA mm^-1)
    - The overall magnetic field intensity in milliamperes per millimeter (mA/mm).
    - Consistent magnetic field intensity can influence the steady-state vibrations of the system.

## Target Variables

### Displacement Variables

1. **mode1_displacement**: Mode 1 Displacement (mm)
   - The average displacement of the system in the first mode, measured in millimeters (mm).
   - This value represents the system’s response to vibrational forces in its first natural mode.

2. **mode2_displacement**: Mode 2 Displacement (mm)
   - The average displacement of the system in the second mode, measured in millimeters (mm).
   - Indicates how the system behaves under vibrational forces in the second mode.

3. **mode3_displacement**: Mode 3 Displacement (mm)
   - The average displacement of the system in the third mode, measured in millimeters (mm).
   - Critical for understanding higher-order vibrational responses.

4. **mode4_displacement**: Mode 4 Displacement (mm)
   - The average displacement of the system in the fourth mode, measured in millimeters (mm).
   - Provides insights into the vibrational behavior in the fourth mode.

5. **mode5_displacement**: Mode 5 Displacement (mm)
   - The average displacement of the system in the fifth mode, measured in millimeters (mm).
   - Important for analyzing the vibrational characteristics in the fifth mode.

### Frequency Variables

1. **mode1_frequency**: Mode 1 Frequency (Hz)
   - The frequency of the system in the first mode, measured in Hertz (Hz).
   - This frequency corresponds to the system's natural frequency in its first vibrational mode.

2. **mode2_frequency**: Mode 2 Frequency (Hz)
   - The frequency of the system in the second mode, measured in Hertz (Hz).
   - Represents the natural frequency in the second mode, crucial for avoiding resonance.

3. **mode3_frequency**: Mode 3 Frequency (Hz)
   - The frequency of the system in the third mode, measured in Hertz (Hz).
   - Helps in understanding the dynamic response in the third mode.

4. **mode4_frequency**: Mode 4 Frequency (Hz)
   - The frequency of the system in the fourth mode, measured in Hertz (Hz).
   - Essential for ensuring the system operates within safe vibrational limits in the fourth mode.

5. **mode5_frequency**: Mode 5 Frequency (Hz)
   - The frequency of the system in the fifth mode, measured in Hertz (Hz).
   - This value is important for predicting the system’s behavior in the fifth mode.

## Data Summary

- **Total Entries**: 121
- **Features**: 11
- **Target Variables**: 10
- **Missing Values**: Handled using interpolation techniques

This dataset is rich in mechanical and environmental features, providing a robust foundation for predicting the dynamic behavior of the system across different vibrational modes. The data preprocessing and feature engineering steps, such as scaling and interpolation, have been performed to ensure the quality and reliability of the predictions made by the models.
