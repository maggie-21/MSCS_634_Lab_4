### MSCS_634_Lab_4
## MSCS 634 - Lab 4: Regression Analysis with Regularization

### 👤 Student Name:
Muluwork Geremew

### 🎓 Course:
MSCS 634 - Advanced Big Data and Data Mining

### 🧪 Lab Objective:
This lab explores various regression techniques using the **Diabetes Dataset** from `sklearn.datasets`, including:

- **Simple Linear Regression**
- **Multiple Linear Regression**
- **Polynomial Regression (Degree 2)**
- **Ridge Regression (L2 Regularization)**
- **Lasso Regression (L1 Regularization)**

The goal is to evaluate the performance of each model, observe the impact of regularization, and understand model generalization.

---

### 📈 Methods & Metrics:

#### Regression Models Implemented:
- Simple Linear Regression (with BMI)
- Multiple Linear Regression (all features)
- Polynomial Regression (degree 2)
- Ridge Regression (α = 1.0)
- Lasso Regression (α = 0.1)

#### Evaluation Metrics:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score (Coefficient of Determination)

---

### 📊 Summary of Results:

| Model                   | MAE    | MSE     | RMSE   | R² Score |
|------------------------|--------|---------|--------|----------|
| Simple Linear (BMI)    | 52.26  | 4061.83 | 63.73  | 0.2334   |
| Multiple Linear         | 42.79  | 2900.19 | 53.85  | 0.4526   |
| Polynomial (Degree = 2) | 43.58  | 3096.03 | 55.64  | 0.4156   |
| Ridge Regression        | 46.14  | 3077.42 | 55.47  | 0.4192   |
| Lasso Regression        | 42.85  | 2798.19 | 52.90  | 0.4719   |

---

### 🔍 Key Insights:

- **Lasso Regression** achieved the best performance, effectively balancing model complexity and generalization.
- Adding more features (Multiple Regression) significantly improved model accuracy over using just one (`bmi`).
- Polynomial features increased complexity but did not improve accuracy — indicating overfitting.
- Regularization techniques (Ridge and Lasso) helped improve performance by controlling overfitting.
- **Lasso** also likely removed irrelevant features, showcasing its ability for **automatic feature selection**.

---

### ⚠️ Challenges Faced:

- Deciding optimal values for `alpha` in Ridge and Lasso.
- Managing increasing feature space in Polynomial Regression without overfitting.
- Interpreting R² versus error metrics across different model types.

---

### 📂 Repository Contents:

- `Lab4_Regression.ipynb` – Jupyter Notebook containing full code, visualizations, and markdown.
- `README.md` – This summary file.

---

### ✅ How to Run:

1. Clone the repository.
2. Open `Lab4_Regression.ipynb` in Jupyter Notebook or VS Code.
3. Run all cells in order.
4. Ensure `scikit-learn`, `matplotlib`, `pandas`, and `numpy` are installed.

```bash
pip install scikit-learn matplotlib pandas numpy
