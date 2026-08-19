# 🧠 Medical Insurance Charges Prediction — Neural Network Regression

A Deep Learning regression project that predicts **medical insurance charges** based on personal attributes like age, sex, BMI, number of children, smoking status, and region — built using **TensorFlow/Keras**.

---

## 📌 Project Overview

This project demonstrates how a neural network can be used to solve a **regression problem** — predicting a continuous numerical value (insurance charges) instead of a class label. It covers the full ML workflow: data preprocessing, feature scaling, model building, training, and evaluation.

---

## 📊 Dataset

The dataset (`insurance.csv`) contains the following features:

| Feature | Description |
|----------|-------------|
| `age` | Age of the individual |
| `sex` | Gender |
| `bmi` | Body Mass Index |
| `children` | Number of dependents |
| `smoker` | Smoking status |
| `region` | Residential region |
| `charges` | Medical insurance cost (target variable) |

---

## ⚙️ Tech Stack

- **Python**
- **TensorFlow / Keras** – Model building
- **Pandas** – Data handling
- **Scikit-learn** – Preprocessing & train-test split
- **Matplotlib** – Visualization

---

## 🔄 Workflow

1. **Data Loading** – Read the insurance dataset using Pandas.
2. **Preprocessing**
   - Converted categorical columns (`sex`, `smoker`, `region`) into numeric form using one-hot encoding (`pd.get_dummies`).
   - Scaled features using `StandardScaler` for better model convergence.
3. **Train-Test Split** – 80% training data, 20% testing data.
4. **Model Architecture**
   ```
   Input → Dense(16, sigmoid) → Dense(64, relu) → Dense(16, tanh) → Dense(1)
   ```
5. **Compilation**
   - Loss: Mean Absolute Error (MAE)
   - Optimizer: SGD
   - Metric: MAE
6. **Training** – Trained for 100 epochs.
7. **Evaluation** – Plotted MAE vs. Epochs to visualize how the model's error decreases over training.

---

## 📈 Results

The model's Mean Absolute Error was tracked across 100 epochs and visualized to understand the learning curve and convergence behavior.

---

## 🚀 How to Run

1. Clone the repository
   ```bash
   git clone <your-repo-url>
   cd <repo-folder>
   ```
2. Install dependencies
   ```bash
   pip install tensorflow pandas scikit-learn matplotlib
   ```
3. Run the notebook
   ```bash
   jupyter notebook Neural_network_Regression.ipynb
   ```

---

## 🔮 Future Improvements

- Experiment with different activation functions and optimizers
- Add early stopping / learning rate scheduling
- Try deeper architectures and compare performance
- Hyperparameter tuning using Keras Tuner

---

## 🏷️ Tags

`Deep Learning` `Neural Networks` `TensorFlow` `Regression` `Machine Learning` `Python`

---

## 📬 Connect

Feel free to reach out if you have suggestions or feedback on this project!
