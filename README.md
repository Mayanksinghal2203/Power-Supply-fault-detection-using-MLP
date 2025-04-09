
# 🔌 DC-DC Converter Fault Prediction using MLP (Neural Network)

This project focuses on predicting **faults in a DC-DC power converter** using a simulated dataset and a Multi-Layer Perceptron (MLP) neural network. The goal is to build a **robust and professional machine learning pipeline** that can be used in real-world scenarios for early detection of power converter faults.

## ⚙️ Tech Stack

- **Python**
- **Keras (TensorFlow backend)**
- **Pandas, NumPy**
- **Scikit-learn**
- **Seaborn & Matplotlib** (for visualization)

## 🔍 Problem Statement

A DC-DC converter can fail due to irregularities in input voltage, temperature, duty cycle variations, and other operational parameters. This project aims to **predict whether the system is faulty or not**, based on key electrical signals.

## 🧠 Features Used

- Input Voltage (`vin`)
- Output Voltage (`vout`)
- Output Current (`iout`)
- Temperature (`temp`)
- Duty Cycle (`duty`)


## 🏗️ Model Architecture

```python
model = Sequential([
    Dense(64, activation="relu", input_shape=(number_of_features,)),
    Dense(32, activation="relu"),
    Dense(1, activation="sigmoid")
])
```

- Loss Function: `binary_crossentropy`
- Optimizer: `adam`
- Metrics: `accuracy`

## 📈 Model Performance

- **Accuracy**: ~100% (on test set)
- **Loss**: ~0.00001
- **Precision / Recall / F1-Score**: 1.0 (perfect classification)
- **No overfitting observed**


## 📊 Visualizations

- **Histograms** for feature distributions
- **Boxplots** for detecting outliers
- **Heatmap** for correlation analysis
- **Loss & Accuracy curves** for overfitting detection
- **Confusion Matrix** and **Classification Report**

## ✅ Project Highlights

- Complete end-to-end ML pipeline
- Realistic dataset simulation
- Robust preprocessing & EDA
- MLP model with perfect performance

## 📌 Future Scope

- Add noise and imbalances to dataset for robustness testing
- Use CNN or LSTM if time-series features are added
- Integrate with Streamlit or Flask for live demo
