# Aviation Accident Analysis - Setup Guide

## 🚀 Quick Start Instructions

### Step 1: Get the Data
You need to download the aviation accident dataset from Kaggle:
1. Go to Kaggle and search for "Aviation Accident Database"
2. Download the CSV file (should be called something like `AviationData.csv`)
3. Place it in the same directory as your notebooks

### Step 2: Project Structure
Your project should look like this:
```
aviation-analysis/
├── Aviation_Accident_Cleaning.ipynb    (Part 1 - Data Cleaning)
├── Aviation_Accident_Analysis.ipynb   (Part 2 - Analysis & Viz)
├── AviationData.csv                   (Your downloaded data - UPDATE THE FILENAME IN NOTEBOOKS!)
├── README.md                          (Project documentation)
└── Aviation_Data_Cleaned.csv          (Created after running Part 1)
```

### Step 3: Run the Notebooks

**IMPORTANT: Run in this order!**

1. **First**: Open `Aviation_Accident_Cleaning.ipynb`
   - Update the filename in the data loading cell to match your CSV file
   - Run all cells from top to bottom
   - This will create `Aviation_Data_Cleaned.csv`

2. **Second**: Open `Aviation_Accident_Analysis.ipynb`
   - This reads the cleaned data
   - Run all cells from top to bottom
   - Generate visualizations and statistics

### Step 4: Complete Your Analysis

As you run the notebooks, fill in these sections in your README:
- [ ] Add your name and date
- [ ] Fill in the actual statistics from your results
- [ ] Save key visualizations as images
- [ ] Write interpretations of your findings
- [ ] Complete the factor analysis sections
- [ ] Write conclusions and recommendations

---

## 📊 What You'll Analyze

### Part 1: Data Cleaning (8 tasks)
1. ✅ Load and inspect data
2. ✅ Check for missing values
3. ✅ Filter to airplanes only
4. ✅ Filter to professional builds
5. ✅ Filter to 1983+
6. ✅ Create injury metrics
7. ✅ Clean Make/Model columns
8. ✅ Remove columns with too many NaNs

### Part 2: Analysis (5 main tasks)
1. ✅ Separate small vs large aircraft
2. ✅ Calculate safety metrics by Make/Model
3. ✅ Recommend top aircraft (small & large)
4. ✅ Analyze at least 2 safety factors:
   - Weather Condition
   - Engine Type
   - Number of Engines
   - Phase of Flight
   - Purpose of Flight
5. ✅ Create visualizations and statistics

---

## 🎯 Deliverables Checklist

For submission, you need:
- [ ] GitHub repository link
- [ ] `Aviation_Accident_Cleaning.ipynb` (completed)
- [ ] `Aviation_Accident_Analysis.ipynb` (completed)
- [ ] `README.md` (with your findings and visualizations)
- [ ] Both notebooks show outputs (run all cells before submitting!)

---

## 💡 Tips for Success

### Data Cleaning
- Don't skip the filtering steps - they're crucial!
- Pay attention to data types (strings vs numbers)
- Watch for missing values in key columns
- Make sure to keep enough data for statistical significance

### Analysis
- **Small sample sizes are unreliable** - use minimum thresholds
- Compare apples to apples (small vs small, large vs large)
- Use visualizations to tell a story
- Statistical significance matters - use t-tests when appropriate

### Visualizations
- Label axes clearly
- Use appropriate chart types
- Make titles descriptive
- Use color purposefully
- Save important charts for README

### Writing
- Write for your client (insurance company)
- Be clear and concise
- Support claims with data
- Provide actionable recommendations

---

## ❓ Common Issues & Solutions

**Issue**: "FileNotFoundError: AviationData.csv"
- **Solution**: Make sure the CSV file is in the same directory and the filename matches exactly

**Issue**: "KeyError: 'Weather.Condition'"
- **Solution**: Column names in your dataset might be slightly different. Check with `df.columns`

**Issue**: "Not enough data for X"
- **Solution**: Lower your minimum threshold or choose different categories

**Issue**: "Division by zero"
- **Solution**: Already handled in the notebooks with conditional logic

---

## 📝 Example Findings (Don't Copy!)

Here's what your analysis might look like:

**Small Aircraft:**
- CESSNA: 42.3% destruction rate (n=2,341 accidents)
- PIPER: 45.1% destruction rate (n=1,892 accidents)

**Large Aircraft:**
- BOEING: 28.5% destruction rate (n=456 accidents)
- AIRBUS: 31.2% destruction rate (n=234 accidents)

**Weather Impact:**
- VMC: 38.2% destruction rate
- IMC: 52.7% destruction rate
- Difference: 14.5 percentage points (p < 0.001)

---

## 🎓 Grading Criteria (Based on Assignment)

Your work will likely be evaluated on:
1. **Data Cleaning** (25%)
   - Correct filters applied
   - Proper handling of missing values
   - Metrics correctly calculated

2. **Analysis** (35%)
   - Appropriate statistical methods
   - Meaningful visualizations
   - Factor analysis depth

3. **Recommendations** (25%)
   - Clear and actionable
   - Supported by evidence
   - Separate for small/large aircraft

4. **Documentation** (15%)
   - Complete README
   - Code comments
   - Professional presentation

---

## 🔧 Troubleshooting

If you get stuck, try:
1. Read error messages carefully
2. Check that previous cells ran successfully
3. Restart kernel and run all cells
4. Verify your data file is correct
5. Check for typos in column names

---

## 📚 Additional Resources

- Pandas Documentation: https://pandas.pydata.org/docs/
- Seaborn Gallery: https://seaborn.pydata.org/examples/index.html
- Matplotlib Tutorials: https://matplotlib.org/stable/tutorials/index.html

---

**Good luck with your analysis! 🎉**

Remember: The goal is to help an insurance company make better underwriting decisions. Think like a business analyst, not just a data scientist!
