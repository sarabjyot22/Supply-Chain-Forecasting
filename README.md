# 📦 Supply Chain Demand Forecasting

This project applies machine learning to forecast product demand using supply chain data from a fashion and beauty startup. The goal is to help businesses improve inventory management, reduce stockouts, and optimize operational efficiency.

---

## 📊 Project Overview

- **Problem Statement**: Predict the number of products sold based on various supply chain features.
- **Approach**: Build and evaluate a neural network regression model using TensorFlow and scikit-learn.
- **Dataset**: Real-world anonymized supply chain data with attributes like product details, supplier info, logistics, costs, and more.

---

## 🛠️ Tools & Technologies

- **Python 3**
- **Pandas, NumPy, Matplotlib, Seaborn** – for data analysis and visualization
- **Scikit-learn** – for preprocessing and evaluation
- **TensorFlow/Keras** – for building the neural network
- **Jupyter Notebook** – for experimentation and model development

---

## 📁 Dataset Features

Some key columns include:

- `Product type`, `SKU`, `Price`, `Availability`
- `Number of products sold` (Target)
- `Revenue generated`, `Stock levels`, `Lead times`
- `Shipping costs`, `Manufacturing costs`, `Defect rates`
- Categorical fields like `Location`, `Supplier name`, `Shipping carriers`

---

## 🧪 Workflow

### 1. **Data Preprocessing**
- Removed missing values
- One-hot encoded categorical features
- Scaled numerical features using `StandardScaler`
- Split data into training and testing sets (80/20)

### 2. **Model Building**
- Neural network with:
  - Dense(128) → ReLU
  - Dense(64) → ReLU
  - Dense(32) → ReLU
  - Output: Dense(1)
- Compiled with Adam optimizer and MSE loss
- Trained for 50 epochs with 20% validation split

### 3. **Model Evaluation**
- Evaluated using **Mean Squared Error (MSE)**
- Visualized loss curves and prediction accuracy (scatter plot)

### 4. **Model Deployment**
- Sample inference provided on new data point

---

## 📈 Results

- **Performance Metric**: MSE (varies based on training)
- **Visualizations**:
  - Training vs Validation Loss
  - True vs Predicted Sales

---

## 📌 Key Benefits

- Data-driven demand forecasting
- Inventory and cost optimization
- Enhanced decision-making for supply chain management

---

## 🗂️ File Structure

