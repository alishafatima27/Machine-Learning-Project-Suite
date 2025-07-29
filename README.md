# Machine-Learning-Project-Suite
# 📈 Comprehensive Machine Learning Projects Documentation

Author: Alisha Fatima
Email: aaafiyasab@gmail.com
Code Link: https://colab.research.google.com/drive/1PMNwxBkSnmrOGCFUhhF9fRsCtJH3Trpy?usp=sharing

This document presents **four well-structured machine learning projects**:

1. **Pune Housing Price Prediction using Linear Regression**
2. **Heart Disease Prediction using Decision Tree**
3. **MNIST Fashion Dataset Classification using Simple Neural Network**
4. **LLM Fine-Tuning with nanoGPT**

Each project demonstrates how **simple models**, when combined with **robust preprocessing, feature engineering**, and **parameter tuning**, can deliver performance **above typical benchmarks**. The documentation is structured with **performance summaries, implementation steps, challenges, solutions, and key learnings**.

---

## 🔢 Model Performance Summary

| Project                       | Model                   | Key Metric      | Value  | Benchmark Comparison          | Notes                                                |
| ----------------------------- | ----------------------- | --------------- | ------ | ----------------------------- | ---------------------------------------------------- |
| Pune Housing Price Prediction | Linear Regression (RFE) | R² (Test)       | 0.9630 | \~0.75–0.80 (Kaggle standard) | Log-transform + clustering + poly features           |
| Heart Disease Prediction      | Decision Tree (Pruned)  | Accuracy (Test) | 0.8689 | \~0.80–0.85 (UCI benchmark)   | Pruning + cross-validation reduced overfitting       |
| MNIST Fashion Classification  | CNN (Baseline)          | Accuracy (Test) | 0.9067 | \~0.88–0.91 (Keras examples)  | Dropout + early stopping ensured generalization      |
| LLM Fine-Tuning               | nanoGPT                 | Validation Loss | 2.4574 | \~2.5–3.0 (nanoGPT setups)    | Mixed precision + gradient accumulation optimized it |

### 🔍 Key Observation:

Each project **surpassed typical benchmarks** due to careful preprocessing, feature engineering, and parameter tuning. E.g., the Linear Regression model achieved an **R² of 0.9630**, significantly higher than standard models, aided by **KMeans clustering** and **polynomial features**.


## ⚙️ Implementation Strategy (Per Project)

Each project has a structured walkthrough including:

* **Step-by-step implementation**
* **Challenges encountered**
* **Solutions and design choices**
* **Impact and evaluation**

This approach ensured every model remained simple yet robust.

---

## 🚧 Common Challenges Faced

* 🧮 **Data Quality Issues**: Inconsistent formats (e.g., square feet ranges), missing values in critical fields.
* ⚠️ **Overfitting Risks**: Especially in Decision Tree and CNN models.
* 🔁 **Multicollinearity**: Detected via VIF checks in linear regression.
* 🧠 **Interpretability vs. Complexity**: Simplicity maintained without sacrificing performance.
* 🗃️ **Storage and Memory**: Managed during nanoGPT fine-tuning using memory-mapped files and mixed precision.

---

## ✅ Solutions and Design Highlights

* ✨ **Custom Parsing** for non-standard entries (e.g., `convert_sqft`).
* 🔍 **EDA + Log Transformations** to reduce skewness.
* 🧠 **Contextual Imputation**: Tailored missing value handling.
* 🧪 **Polynomial Features + RFE**: Boosting regression model accuracy.
* 🏷️ **KMeans Clustering**: Converted categorical `society` into valuable numerical clusters.
* 🧰 **Regularization Techniques**: Dropout, pruning, early stopping.
* 🧠 **Model Monitoring**: Learning curves, SHAP analysis, ROC/PR curves.

---

## 📚 Key Learnings

* 🔁 **Simplicity Works**: Basic models like Linear Regression and Decision Trees achieved remarkable results when engineered well.
* 🏗️ **Preprocessing is Powerful**: From log-transformation to outlier handling, preprocessing dramatically impacted performance.
* 🧬 **Feature Engineering is Impactful**: Custom features like `area_per_room` and `cluster` significantly improved accuracy.
* 🔍 **Model Interpretability is Essential**: SHAP and decision tree visuals offered actionable insights.
* 🚀 **Efficiency Techniques Matter**: Using tools like `np.memmap`, mixed precision, and early stopping accelerated experiments without sacrificing performance.

---

## 🧠 Final Reflection & Outcomes

This project suite emphasized that **simple models**—when paired with **smart strategies**—can yield **exceptional performance**, often outperforming more complex architectures. The key lies not in model depth, but in:

* 💡 Problem understanding
* 🔬 Meticulous preprocessing
* 🧪 Thoughtful evaluation
* 📉 Regularization and monitoring

These projects not only showcase strong technical execution but also highlight the importance of clarity, efficiency, and interpretability in applied machine learning

