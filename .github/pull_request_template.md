## 📋 Learner Information
- **Name:** 
- **GitHub Username:** `@`
- **Submitted Notebook Filename:** 

---

## 📝 Summary of Work
<!-- Briefly describe what you implemented in this Pull Request (e.g., data loading, datetime indexing, resampling, rolling averages, seasonal analysis, and visualizations). -->
- 
- 
- 

---

## 🔍 Key Data Analysis Findings
<!-- Share 1–3 key insights from your analysis of the NOAA dataset (e.g., how temperatures trend from January to August 2025, monthly averages, or day-of-week patterns). -->
- 
- 

---

## ✅ Pre-Submission Checklist

### Git & GitHub Hygiene
- [ ] I created a descriptive **feature branch** (e.g., `feat/yourname-noaa-analysis`) instead of committing directly to `main`.
- [ ] I used a clear, descriptive **notebook filename** (not `Untitled.ipynb`) and removed any empty or duplicate scratch files.
- [ ] I wrote meaningful **commit messages** and a descriptive **Pull Request title**.

### Data Science & Notebook Standards
- [ ] **Portable File Path:** I loaded the dataset using a relative path (`pd.read_csv("noaa - 5000.csv")`) rather than a hardcoded local path (`C:\Users\...`).
- [ ] **Real Dataset Integrity:** All analysis and plots use the actual `noaa - 5000.csv` data (no synthetic/random `np.sin` or `np.random` overrides).
- [ ] **Datetime & Multi-Station Handling:** I converted `date` to `datetime64`, sorted chronologically, and aggregated daily station observations (`df.groupby("date")["temp"].mean()`) before computing rolling windows or reindexing.
- [ ] **Complete Time-Series Workflow:** I included date slicing (`.loc[...]`), weekly & monthly resampling (`"W"`, `"ME"`/`"MS"`), 30-day rolling average (`.rolling(30).mean()`), and calendar seasonality (`month`, `day_of_week`).
- [ ] **Visualization Best Practices:** All `plt.plot()` layers for a single chart are placed in the **same cell** before `plt.show()`, with a clear title, legend, and axis labels (`Temperature (°F)`).
- [ ] **Markdown Storytelling:** I included Markdown cells to document each step and summarize my conclusions.
- [ ] **Sequential Execution:** I ran **Restart & Run All** before committing so every cell executes cleanly in order (`[1, 2, 3, ...]`) with all outputs and plots saved.
