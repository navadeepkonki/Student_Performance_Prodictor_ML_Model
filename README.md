# Student Performance Prediction using Decision Tree Regression

This project predicts a student’s final grade (**G3**) using academic, demographic, and social features from the Student Performance dataset.  
A **Decision Tree Regressor** is trained and optimized using **GridSearchCV** to improve prediction performance.

---

## 📌 Problem Statement

Student academic performance is influenced by multiple factors such as study time, failures, family support, and absences.  
The goal of this project is to build a machine learning model that can predict the final grade (**G3**) based on these features.

---

## 🧠 Machine Learning Approach

- **Type**: Supervised Learning  
- **Task**: Regression  
- **Model Used**: Decision Tree Regressor  
- **Evaluation Metrics**:
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
  - R² Score

---

## 📂 Dataset

- **Source**: Student Performance Dataset  
- **Target Variable**: `G3` (Final Grade)  
- **Preprocessing Steps**:
  - Encoded categorical variables (`sex`, `schoolsup`)
  - Applied one-hot encoding using `pd.get_dummies`
  - Feature scaling using `StandardScaler`

---

## ⚙️ Tech Stack & Libraries

- Python  
- pandas  
- numpy  
- matplotlib  
- scikit-learn  

---

## 🔄 Workflow

1. Load and preprocess the dataset  
2. Encode categorical variables  
3. Scale features using `StandardScaler`  
4. Split data into training and testing sets  
5. Train a Decision Tree Regressor  
6. Evaluate baseline model  
7. Tune hyperparameters using `GridSearchCV`  
8. Evaluate the tuned model  
9. Visualize actual vs predicted values  

---

## 🧪 Model Training & Tuning

Hyperparameters tuned using **GridSearchCV**:
- `max_depth`
- `min_samples_split`
- `min_samples_leaf`

- **Scoring Metric**: R² Score  
- **Cross-validation**: 5-fold  

---

## 📊 Results

### Baseline Model
- MAE: Printed in console  
- RMSE: Printed in console  
- R² Score: Printed in console  

### Tuned Model
- Improved R² Score  
- Reduced MAE and RMSE  

The tuned Decision Tree performs better than the default model, indicating effective hyperparameter optimization.

---

## 📈 Visualization

The project includes a scatter plot comparing:
- Actual G3 scores  
- Predicted G3 scores  

A reference line (**y = x**) is plotted to visualize prediction accuracy.

---

## ▶️ How to Run the Project

Follow these steps to run the project locally:

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/student-performance-prediction.git
cd student-performance-prediction
```

### 2. Create a Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

* **Linux / macOS**

```bash
source venv/bin/activate
```

### 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib scikit-learn
```

### 4. Add the Dataset

* Download the **Student Performance Dataset**
* Place the CSV file (for example: `student_data.csv`) in the project root directory

### 5. Run the Python Script / Notebook

If you are using a Python script:

```bash
python decision_tree_regression.py
```

If you are using a Jupyter Notebook:

```bash
jupyter notebook
```

Then open and run all cells in the notebook.

### 6. View the Output

* Evaluation metrics (MAE, RMSE, R² Score) will be printed in the console
* A scatter plot of **Actual vs Predicted G3 scores** will be displayed

---

## 📌 Notes

* Ensure the dataset file path matches the path used in the code
* Hyperparameter tuning may take a few seconds due to cross-validation
* Results may vary slightly due to random train-test splits

---