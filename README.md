
# 🎓 Student Performance Prediction

Predicting final grades of high school students using Linear Regression, Ridge Regression, and Lasso Regression.

---

## 📌 Project Description

This project uses a dataset from UCI Machine Learning Repository to predict students' final grades based on various academic and personal attributes. The models used include:

- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**

The goal is to compare these models' performance and understand which features most influence a student’s final grade.

---

## 📁 Dataset

**Source**: [UCI Student Performance Data](https://archive.ics.uci.edu/ml/datasets/Student+Performance)  
**File Used**: `student-mat.csv` (Portuguese language course)  
**Separator**: `;`

**Target Variable**: `G3` (Final Grade)  
**Important Features**:
- `G1`, `G2` (First & second period grades)
- `studytime` (Weekly study hours)
- `failures` (Past class failures)
- `absences` (Number of school absences)

---

## 📊 Exploratory Data Analysis (EDA)

Key EDA insights include:
- Strong positive correlation between `G1`, `G2`, and final grade `G3`
- Slight negative impact of absences and failures
- Grades approximately normally distributed
- Boxplots show mild outliers in absences

Visualization tools used:
- Histograms
- Correlation heatmap
- Boxplots
- Pairplots

### EDA Steps Performed:
- Checked dataset shape, info, and descriptive stats
- Verified missing values and duplicates
- Plotted distribution of final grades (`G3`)
- Analyzed correlation matrix and heatmap
- Explored pairwise relationships with pairplots
- Used boxplots to detect outliers in numerical features

---

## ✅ Features Used


features = ['G1', 'G2', 'studytime', 'failures', 'absences']
target = 'G3'


These features were selected based on correlation values and logical importance.

---

## 🧠 Models Used

| Model              | Regularization | Notes                     |
|-------------------|----------------|---------------------------|
| Linear Regression | ❌             | Baseline model            |
| Ridge Regression  | ✅ (L2)        | Penalizes large weights   |
| Lasso Regression  | ✅ (L1)        | Performs feature selection|

---

## ⚙️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📈 Results

| Model              | RMSE  | R² Score |
|-------------------|-------|----------|
| Linear Regression | ~2.X  | ~0.85    |
| Ridge Regression  | ~2.X  | ~0.85    |
| Lasso Regression  | ~2.X  | ~0.84    |

> 💡 *Exact results may vary depending on random state, test split, and regularization strength.*

---

## 🚀 How to Run

1. **Clone the repository**:
   
   git clone https://github.com/yourusername/student-grade-prediction.git
   cd student-grade-prediction
   

2. **Install dependencies**:
  
   pip install -r requirements.txt
  

3. **Run the notebook**:
   
   jupyter notebook student_grade_prediction.ipynb
  

---

## 🖼️ Visualizations

- 📉 **Histogram**: Distribution of final grades
- 🔥 **Correlation heatmap**: Feature relationships
- 📦 **Boxplot**: Outliers in grades and absences
- 📊 **Pairplot**: Feature pair relationships

---

## 📚 Future Improvements

- Add ensemble models (Random Forest, XGBoost)
- Try polynomial regression for non-linear effects
- Turn into a web app using Streamlit or Flask
- Use full categorical data with one-hot encoding
- Perform hyperparameter tuning (GridSearchCV)

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 👩‍💻 Author

**Bisakh Patra**  
[GitHub Profile] - (https://github.com/Asphane)
