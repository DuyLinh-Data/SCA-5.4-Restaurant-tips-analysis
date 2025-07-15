# 🍽️ Restaurant Tips Analysis

This project explores tipping behavior in a restaurant setting using Python. The goal is to identify patterns and factors that influence how much customers tip, such as time of day, gender, meal size, and day of the week.

<img width="1790" height="490" alt="3plot" src="https://github.com/user-attachments/assets/f2cfafcf-d79a-4e85-a8b5-95b242dc2ab6" />

---

## 🎯 Objectives

- Understand how different variables affect the amount of tips.
- Visualize relationships and distributions among key features.
- Detect outliers and test hypotheses (e.g., gender differences in tipping).
- Summarize actionable insights using data storytelling techniques.

---

## 📊 Dataset

- **Source**: Built-in `seaborn` dataset `tips`
- **Rows**: 244 records
- **Columns**:
  - `total_bill`, `tip`, `sex`, `smoker`, `day`, `time`, `size`

---

## 🧪 Key Analysis Performed

- Descriptive statistics & data cleaning
- Correlation analysis (Pearson)
- Boxplots to compare tipping across:
  - Time (Lunch vs Dinner)
  - Gender
  - Days of the week
- Outlier detection (IQR)
- Hypothesis testing: gender vs tip amount
- Feature engineering (e.g., tip ratio, bill categories)

---

## 📍 Key Insights

- 🕒 **Dinner tips are usually higher** than lunch tips.

<img width="1389" height="490" alt="tipdinnerlunch" src="https://github.com/user-attachments/assets/a03ca95a-3acf-4ddd-90a8-1fdff5c2d3f8" />

  
- 👩‍🦰 No significant difference between male and female tipping behavior after removing outliers.

<img width="790" height="490" alt="tipmalefemale" src="https://github.com/user-attachments/assets/46c49055-dcc3-42a3-a681-687c082e104d" />

- 📅 Weekends (Sat & Sun) show **higher total bills and tips**.

<img width="790" height="490" alt="tipwkwday" src="https://github.com/user-attachments/assets/a4844055-da35-4cb5-8517-596758401d73" />


- 💸 Tip percentage varies more at lower bill sizes.

---

## 🛠️ Technologies Used

- Python 3.x
- Jupyter Notebook
- Pandas, NumPy
- Seaborn, Matplotlib
- SciPy (for statistical testing)

---

## 📁 Folder Structure (if applicable)


