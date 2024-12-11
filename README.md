# 🚀 Loan Default Prediction - README

## 📌 Project Overview
This project is designed to assist **Non-Banking Financial Companies (NBFCs)** in predicting loan repayment behavior. The goal is to classify loan applications into **default** or **non-default** categories, enabling better risk assessment and streamlined loan approvals.

---

## 📂 Contents
1. 📘 **Notebook**: `DSW_internship_assignment.ipynb` - Main implementation file.
2. 📊 **Datasets**:
   - 📂 `train_data.xlsx`: Historical loan data for training.
   - 📂 `test_data.xlsx`: Recent loan data for testing.

---

## 🎯 Objectives
- 🔍 **Identify** borrowers likely to default.
- 📈 **Improve** loan risk assessment accuracy.
- 🤝 **Enhance** financial inclusion by streamlining the loan approval process.

---

## 🧠 Models Developed
### 1️⃣ Random Forest Classifier 🌲
- **Why Use It?**: Reliable, interpretable, and handles imbalanced data effectively.
- **Features**:
  - Utilizes **SMOTE** to balance the dataset.
  - Provides **feature importance insights** for decision-making.
- **Accuracy**: **88.5%**

### 2️⃣ XGBoost Classifier ⚡
- **Why Use It?**: Optimized for performance and scalability.
- **Features**:
  - Hyperparameter tuning using **GridSearchCV**.
  - Delivers robust predictions and scalability.
- **Accuracy**: **92.3%**

---

## 💪 Steps Involved

### 📥 1. Data Preparation
- Load datasets (`train_data.xlsx` and `test_data.xlsx`) using pandas.

### 🔍 2. Data Analysis and Cleaning
- Inspect data for missing values and inconsistencies.
- Analyze the distribution of `loan_status` (target variable).

### 🧹 3. Feature Engineering
- **Transformations**:
  - Extract `transaction_month` and `days_since_transaction` from dates.
  - Create `debt_to_income` (loan amount divided by annual income).
- **Encoding**:
  - Apply label encoding to categorical variables.

### ⚖️ 4. Handling Class Imbalance
- Balance the dataset using **SMOTE** to address the minority class issue.

### 🧐 5. Model Training and Evaluation
- **Random Forest**:
  - Trained on balanced data.
  - Evaluated using:
    - 📋 Classification Report
    - 📈 **ROC-AUC Curve**
- **XGBoost**:
  - Optimized with **GridSearchCV** for better accuracy.
  - Evaluated using the same metrics.

### 🧪 6. Testing
- Test models on unseen data (`test_data.xlsx`) and compare results.

---

## 💪 Tools and Libraries
The project uses the following libraries:
- 📊 **Data Manipulation**: `pandas`, `numpy`
- 🎨 **Visualization**: `matplotlib`, `seaborn`
- 🧐 **Modeling**: `scikit-learn`, `xgboost`
- ⚖️ **Balancing**: `imbalanced-learn`
- 🔐 **Model Saving**: `joblib`

📦 Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost
```

---

## 🚦 How to Run
1. Upload the notebook (`DSW_internship_assignment.ipynb`) and datasets to **Google Colab**. 🔤️
2. Update file paths for training and testing datasets in the notebook. ✍️
3. Run all cells sequentially to preprocess, train, and evaluate the models. ▶️
4. Save the trained models for future use using `joblib`. 🔐

---

## 📊 Results Summary
- **🌲 Random Forest**:
  - Reliable baseline model with feature importance insights.
  - Well-suited for imbalanced datasets.
  - **Accuracy**: **88.5%**
- **⚡ XGBoost**:
  - Superior performance with higher accuracy and **ROC-AUC scores** due to hyperparameter tuning.
  - **Accuracy**: **92.3%**

---

## 🚀 Future Directions
- 🧹 **Data**: Include additional features to improve prediction accuracy.
- 🧠 **Models**: Experiment with advanced models like neural networks.
- 🌐 **Deployment**: Build a real-time loan evaluation application.

---

## 📩 Contact Information
For any queries or feedback, feel free to reach out:

📧 **Email**: 21106006.atul.gupta@gmail.com  
📱 **Mobile**: 9867091698  
🌐 **Name**: Atul Mahendra Gupta

---

💡 *This project showcases how machine learning can revolutionize financial decision-making. Let's make smarter and more inclusive loans together!* 🌟
