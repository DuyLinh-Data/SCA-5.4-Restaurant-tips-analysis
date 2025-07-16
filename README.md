
# 🍽️ Restaurant Tips Analysis

This project explores tipping behavior in a restaurant setting using Python. The goal is to identify patterns and factors that influence how much customers tip, such as time of day, gender, meal size, and day of the week.

<img width="100%" alt="overview" src="https://github.com/user-attachments/assets/f2cfafcf-d79a-4e85-a8b5-95b242dc2ab6" />

---

## 🎯 Objectives

- Explore how variables like time, gender, and day impact tipping behavior
- Visualize relationships and highlight statistical patterns
- Detect outliers and test hypotheses
- Summarize findings with clear, visual storytelling

---

## 📊 Dataset

- **Source**: Built‑in `seaborn` dataset **tips**
- **Records**: 244 rows × 7 columns
- **Columns**: `total_bill`, `tip`, `sex`, `smoker`, `day`, `time`, `size`

---

## 📌 Key Analyses

- Descriptive statistics & data cleaning
- Correlation analysis (Pearson)
- Boxplots comparing tips by:
  - 🕒 Time (Lunch vs Dinner)
  - 👩 Gender
  - 📅 Day of week
- Outlier detection (IQR)
- Hypothesis testing
- Feature engineering (tip ratio, bill categories)

---

## 📍 Key Insights

| Insight | Visualization |
|---------|---------------|
| **Dinner tips are generally higher than lunch tips** | <img width="90%" alt="tipdinnerlunch" src="https://github.com/user-attachments/assets/a03ca95a-3acf-4ddd-90a8-1fdff5c2d3f8" /> |
| **No strong gender difference after removing outliers** | <img width="70%" alt="tipmalefemale" src="https://github.com/user-attachments/assets/46c49055-dcc3-42a3-a681-687c082e104d" /> |
| **Weekends show higher total bills and tips** | <img width="70%" alt="tipwkwday" src="https://github.com/user-attachments/assets/a4844055-da35-4cb5-8517-596758401d73" /> |
| **Lower bill amounts show more variation in tip %** | – |

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/AntoniNguyen123/restaurant-tip-analysis.git
cd restaurant-tip-analysis

# 2. Install dependencies
pip install pandas numpy seaborn matplotlib scipy jupyter

# 3. Launch Jupyter Notebook
jupyter notebook notebooks/"[5.4] Restaurant tips analysis.ipynb"
```

---

## 🛠️ Technologies Used

- Python 3.x • Jupyter Notebook
- Pandas • NumPy • Seaborn • Matplotlib
- SciPy (statistical tests)

---

## 📁 Folder Structure

```
📦 restaurant-tip-analysis
├── notebooks/
│   └── [5.4] Restaurant tips analysis.ipynb
├── images/
├── README.md
```

---

## 🔭 Future Improvements

- Build an interactive dashboard with Plotly or Streamlit
- Analyse tip percentage by party size
- Predict tip amount using regression models
- Cluster diners based on tipping behaviour

---

## 📝 License

This project is released under the MIT License – feel free to use and adapt with attribution.

---

## 🙋‍♂️ About Me

**Nguyễn Duy Linh** • Aspiring Data Analyst passionate about uncovering insights from data.

- 📧 linhnguyen.asia@gmail.com  
- 🔗 [LinkedIn](https://www.linkedin.com/in/nguy%E1%BB%85n-duy-linh/) • [GitHub](https://github.com/AntoniNguyen123)

_“It’s not about having data, it’s about what you do with it.”_ 🚀
