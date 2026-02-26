# 🎮 Predictive Analysis of Game Success in STEAM Using Interpretable AI

📊 Applied Artificial Intelligence Coursework
👨‍💻 Author: Tharindu D. Mallawaarachchi


---

## 📌 Project Overview

The STEAM marketplace contains thousands of games, but predicting commercial success remains highly uncertain.

This project builds a **machine learning classification system** to predict whether a game will be successful based on structured metadata — while ensuring transparency using **Interpretable AI techniques**.

Instead of relying on black-box predictions, this study integrates **SHAP (SHapley Additive exPlanations)** to explain:

• Why the model made a prediction
• Which features contribute most to success
• How different attributes influence outcomes

The goal is not only prediction accuracy — but meaningful insight.

---

## 🎯 Objectives

✔ Predict game success using machine learning
✔ Apply structured preprocessing and feature engineering
✔ Evaluate performance using classification metrics
✔ Integrate SHAP for model interpretability
✔ Provide transparent insights into key success factors

---

## 📂 Dataset

The dataset includes STEAM game metadata such as:

• Number of user reviews
• Rating percentage
• Price
• Genre information
• Release data
• Other structured features

### Data Preparation Steps

🧹 Removed invalid and zero-recommendation entries
🔄 Handled missing values
🔢 Encoded categorical variables
📏 Normalized / scaled numerical features
✂ Split into training and testing sets

---

## 🧠 Model Architecture

The project uses:

🌳 Random Forest Classifier

Why Random Forest?

• Handles non-linear relationships well
• Robust to noise
• Strong performance on tabular datasets
• Provides built-in feature importance

---

## 📈 Model Evaluation

Performance is evaluated using:

• Accuracy
• Precision
• Recall
• F1-score
• Confusion Matrix

This ensures balanced evaluation beyond simple accuracy.

---

## 🔍 Interpretable AI Layer

To prevent black-box decisions, SHAP analysis is applied:

📊 Global Feature Importance
📌 Individual Prediction Explanations
📈 SHAP Summary Visualization

This allows us to understand *why* a game is predicted as successful.

Prediction without explanation is guessing with math.
Prediction with explanation is insight.

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Predictive-Analysis-of-Game-Success-in-STEAM-Using-Interpretable-AI.git
cd Predictive-Analysis-of-Game-Success-in-STEAM-Using-Interpretable-AI
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run Notebook

```bash
jupyter notebook
```

Open:

`STEAM Game Sucess Predictor.ipynb`

---

## 🧪 Quick Prototype Test

To quickly test the trained model:

Inside the notebook, locate the prediction section and run:

```python
sample_input = X_test.iloc[[0]]
model.predict(sample_input)
```

This generates a success prediction for a sample game.

To view explanation:

```python
shap_values = explainer(sample_input)
shap.plots.waterfall(shap_values[0])
```

This shows exactly which features influenced the prediction.

---

## 🗂 Repository Structure

```
📁 Predictive-Analysis-of-Game-Success-in-STEAM-Using-Interpretable-AI
│
├── 📓 STEAM Game Sucess Predictor.ipynb
├── 📄 README.md
├── 📄 requirements.txt
└── 📁 assets (optional – saved plots)
```

---

## 🛠 Technologies Used

🐍 Python
📊 Pandas
🔢 NumPy
🤖 Scikit-learn
🔍 SHAP
📈 Matplotlib
📉 Seaborn
📓 Jupyter Notebook

---

## 💡 Key Insights

The analysis shows that:

• Review volume strongly impacts predicted success
• Rating percentage is a dominant predictor
• Pricing influences performance patterns
• Certain categorical features contribute meaningfully

SHAP confirms these relationships quantitatively.

---

## 🔮 Future Improvements

🌐 Deploy as a web-based dashboard
📡 Integrate live STEAM API data
📊 Compare multiple ensemble models
📈 Add temporal trend modeling
🧠 Explore causal inference approaches

---

## 📜 Academic Context

This project was developed as part of an Applied Artificial Intelligence coursework module.

It demonstrates:

✔ Data preprocessing rigor
✔ Model justification
✔ Evaluation methodology
✔ Interpretability integration
✔ Analytical discussion of results

---

Now — let’s elevate this further.

To make your repository even stronger:

1️⃣ Export your confusion matrix as PNG
2️⃣ Export SHAP summary plot as PNG
3️⃣ Add them inside an `assets/` folder
4️⃣ Embed in README using:

```markdown
![Confusion Matrix](assets/confusion_matrix.png)
![SHAP Summary](assets/shap_summary.png)
```

This transforms it from “student upload” to “AI portfolio project”.

