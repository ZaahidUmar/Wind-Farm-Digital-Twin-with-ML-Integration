# Wind Turbine Power Prediction – Digital Twin Project

This project implements a lightweight digital twin for a wind turbine system using
machine learning, IoT data streaming, and a Unity-based 3D simulation. A 
Random Forest Regression model is trained on real SCADA data to predict 
LV ActivePower (kW) from Wind Speed (m/s), and the model is exported to ONNX 
for real-time inference inside Unity.

## Features
- Random Forest–based wind power prediction  
- ONNX model for cross-platform ML inference  
- Unity 3D farm with interactive UI  
- Live wind-speed data from Arduino → MQTT → Unity  
- Real-time predicted & live output updates  

## Tech Stack
- **ML:** Python, Scikit-learn, ONNX  
- **IoT:** Arduino Uno R4 WiFi, HiveMQ MQTT  
- **Visualization:** Unity (URP), C#, ONNX Runtime  

## How It Works
1. Train a Random Forest Regression model using Wind Speed as input  
2. Export the trained model as `wind_power_rf_model.onnx`  
3. Unity loads the ONNX model and runs predictions in real-time  
4. Arduino publishes mock wind-speed data through MQTT  
5. Unity displays both live and predicted power values  

## Outputs
- Trained `.pkl` and `.onnx` model files  
- Real-time Unity digital twin simulation  
- Live & predicted power estimation display  
