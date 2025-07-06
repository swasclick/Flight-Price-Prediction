# ✈ Predicting Flight Fares with ML: A Deep Dive from Chaos to Clarity 🚀

Just completed a hands-on Flight Fare Prediction project that went beyond the basics — not just another regression model, but a data science journey filled with learning, iteration, and surprising results.

---

## 🔍 What I Did:

### 🧹 Smart Missing Value Imputation:
Instead of dropping rows or using simple mean/mode, I leveraged **Random Forest Classifier** and **KNN-based imputation** which included **label encoding** the categorical data to predict missing values intelligently, preserving valuable patterns in the data.

---

### 🧠 Insightful Feature Engineering:

- Clipped outliers based on **IQR-based bounds**  
- Used **one-hot encoding** for features with fewer classes, and **target encoder** for features with large class numbers

---

## 🧪 Model Building & Results:

🧠 **11 different Models** — From Linear Regression to Neural Network Regressors, battled it out to crush **Mean Squared Errors**, but the takeaway?

👉 **More complex ≠ better predictions**.  
- I tried to **log transform** a few numerical columns that were right-skewed, but the models made way worse predictions, because they **overfit the clumped-up data points!**
- Simply clipping the (very few) outliers boosted the performance several fold.  
- Despite tuning, **Neural Networks were outperformed by simpler ensemble models**.

---

### 🥇 In the end, the good ol' **Random Forest Regressor** dominated — delivering:

✅ **Max Baseline R²**: `97.8%`  
✅ **Tuned, Cross-Validated, Generalized R²**: `97.6%`

---

## 📌 Key Takeaways:

- **EDA + Feature Engineering = 70% of the work that drives results**  
- **Simpler models can outperform deep ones — especially on structured tabular data**  
- **Ensemble models like Random Forest can be both powerful and interpretable**
