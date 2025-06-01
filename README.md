# 📊 Telco Customer Churn Prediction

A machine learning project to **predict customer churn** for a telecommunications company. The goal is to identify customers likely to leave, enabling proactive retention strategies.

---

## 🚀 Features

* **Dataset:** Telco Customer Churn (includes demographics, service details, account info, and churn status)
* **Model:** Tuned **LightGBM (LGBM)** Classifier
* **Key Metrics (Test Set):**

  * 🎯 **F1-Score (Churn Class):** 0.8729
  * ✅ Accuracy: 0.9312
  * 📈 ROC AUC: 0.9814
* **Top Churn Drivers:** Monthly Charges, Tenure Months, CLTV (Customer Lifetime Value)

---

## 🧠 Methodology

1. **Data Preprocessing:**

   * Cleaning & imputation (median on training set)
   * One-hot encoding & standard scaling
   * Stratified train-test split (*before* scaling/encoding)
2. **Model Selection:**

   * Compared multiple classifiers
   * Chose LightGBM for its performance and speed
3. **Hyperparameter Tuning:**

   * Used `RandomizedSearchCV` to maximize F1-score
4. **Model Evaluation:**

   * Accuracy, Precision, Recall, F1-score, ROC AUC
   * Confusion Matrix

---

## 🛠 Tech Stack

* **Language:** Python 3.x
* **Libraries:**

  * `pandas`, `numpy`
  * `scikit-learn`
  * `lightgbm`
  * `joblib` (for saving model artifacts)

---

## 📂 Project Structure (Example)

```
Customer_Churn_Prediction/
│
├── data/
│   └── Telco_customer_churn.xlsx
├── notebooks/
│   └── Customer_churn_prediction.ipynb
├── src/
│   └── model_pipeline.py
├── outputs/
│   └── churn_model.pkl
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup & Run

1. **Clone the Repository**

   ```bash
   git clone https://github.com/khurrambhutto/Customer_Churn_Prediction.git
   cd Customer_Churn_Prediction
   ```

2. **Create Virtual Environment**

   ```bash
   python -m venv venv
   venv\Scripts\activate  # On Windows
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Notebook**
   Open `Customer_churn_prediction.ipynb` in Jupyter Notebook or VS Code and execute step-by-step.

---

## 📄 License

This project is licensed under the **MIT License**.
See the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributions

Contributions, suggestions, and forks are welcome!
Feel free to open an issue or submit a pull request.

---

## ✉️ Contact

For any questions or collaboration ideas, reach out via [GitHub](https://github.com/khurrambhutto).
