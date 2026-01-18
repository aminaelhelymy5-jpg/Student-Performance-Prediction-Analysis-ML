# Student Performance Prediction & Analysis ML

## Description
This is a **Machine Learning project** that analyzes and predicts students’ academic performance using Python.  
The project includes **Regression** and **Classification** models to predict exam scores and pass/fail outcomes.

- **Regression:** Predicts student exam scores  
- **Classification:** Predicts whether a student will pass or fail  
- **Features used:** Age, number of absences, study hours

---

## Dataset
The dataset contains student information with the following columns:

| Feature       | Description                        |
|---------------|------------------------------------|
| age           | Age of the student                 |
| absences      | Number of school absences          |
| study_hours   | Average study hours per week       |
| score         | Exam score (for regression)        |
| pass_fail     | Pass (1) or Fail (0) (for classification) |

> The dataset file: `data/students_performance.xlsx`

---

## Project Workflow

1. **Data Exploration**
   - Load dataset with pandas
   - Inspect data (`head()`, `info()`, `describe()`)

2. **Data Preprocessing**
   - Handle missing values
   - Encode categorical features (if any)
   - Split data into train/test sets

3. **Regression Model**
   - Features: `age`, `absences`, `study_hours`
   - Target: `score`
   - Model: `LinearRegression()`
   - Train on training set, predict on test set

4. **Classification Model**
   - Features: `age`, `absences`, `study_hours`
   - Target: `pass_fail`
   - Model: `LogisticRegression()` or `KNN`
   - Train on training set, predict on test set

5. **Evaluation**
   - Regression: `R²`, `MAE`
   - Classification: `Accuracy`, `Confusion Matrix`

6. **Predictions on new students**
   - Test models on new student data
   - Compare predicted vs actual results

7. **Visualization**
   - Scatter plots for regression predictions
   - Bar charts or confusion matrices for classification

---

## Results (Example)

### Regression
- Predicted scores for new students: `[78, 85, 92]`  
- R² ≈ 0.99  
- MAE ≈ 2.5  

### Classification
- Predicted Pass/Fail for new students: `[1, 0, 1]`  
- Accuracy ≈ 95%  
- Confusion Matrix:
