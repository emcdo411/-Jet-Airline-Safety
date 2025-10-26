# Aviation Accident Data Analysis
## Jet Airline Safety Study for Insurance Client

**Author:** [Your Name]  
**Date:** [Current Date]  
**Course:** Introduction to Data Science

---

## Executive Summary

This analysis examines aviation accident data from 1983-2023 to identify aircraft makes and models with superior safety records for insurance underwriting purposes. The study focuses on professional-built airplanes and analyzes two key metrics: aircraft destruction rates and fatal/serious injury rates.

### Key Findings:

**Small Aircraft (<20 passengers):**
- [List top 3-5 recommended makes with their destruction rates]
- Example: CESSNA: 45.2% destruction rate, 0.65 average injury rate

**Large Aircraft (≥20 passengers):**
- [List top 3-5 recommended makes with their destruction rates]
- Example: BOEING: 32.1% destruction rate, 0.58 average injury rate

**Critical Safety Factors:**
1. **Weather Conditions**: IMC operations show XX% higher destruction rates than VMC
2. **[Second Factor]**: [Brief description of impact]

---

## Project Overview

### Business Problem
An airline/airplane insurance company needs to:
- Identify aircraft makes/models with low destruction rates
- Assess injury risk profiles across different aircraft types
- Understand environmental and operational factors affecting safety
- Make separate recommendations for small vs. large passenger aircraft

### Data Source
- **Dataset**: Aviation Accident Database (1948-2023)
- **Filtered Date Range**: 1983-2023 (40-year aircraft lifetime)
- **Final Sample Size**: [X,XXX] accidents
- **Aircraft Types**: Professional-built airplanes only

---

## Methodology

### Data Cleaning Process

1. **Filtering Criteria**:
   - Aircraft Category: Airplanes only
   - Amateur Built: Professional builds only (No)
   - Date Range: 1983 onwards
   - Make: Minimum 50 accidents for statistical robustness

2. **Key Metrics Created**:
   - **Total Passengers**: Sum of all injury categories + uninjured
   - **Injury Rate**: (Fatal + Serious Injuries) / Total Passengers
   - **Aircraft Destroyed**: Binary indicator (1 = Destroyed, 0 = Not Destroyed)
   - **Aircraft Size**: Small (<20 passengers) vs Large (≥20 passengers)

3. **Data Quality**:
   - Removed columns with >80% missing values
   - Converted dates to datetime format
   - Standardized categorical variables
   - Created unique Make_Model identifier

### Analysis Approach

1. **Descriptive Statistics**: Calculated destruction and injury rates by make/model
2. **Segmentation**: Separated analysis for small vs. large aircraft
3. **Factor Analysis**: Examined impact of weather, engine type, phase of flight, etc.
4. **Statistical Testing**: Conducted hypothesis tests for significant factors
5. **Trend Analysis**: Evaluated safety improvements over time

---

## Results

### Small Aircraft Recommendations (<20 passengers)

#### Top 5 Recommended Makes

| Rank | Make | Destruction Rate | Injury Rate | Sample Size |
|------|------|------------------|-------------|-------------|
| 1 | [Make Name] | XX.X% | X.XX | XXX |
| 2 | [Make Name] | XX.X% | X.XX | XXX |
| 3 | [Make Name] | XX.X% | X.XX | XXX |
| 4 | [Make Name] | XX.X% | X.XX | XXX |
| 5 | [Make Name] | XX.X% | X.XX | XXX |

**Insight**: [Brief interpretation of small aircraft findings]

---

### Large Aircraft Recommendations (≥20 passengers)

#### Top 5 Recommended Makes

| Rank | Make | Destruction Rate | Injury Rate | Sample Size |
|------|------|------------------|-------------|-------------|
| 1 | [Make Name] | XX.X% | X.XX | XXX |
| 2 | [Make Name] | XX.X% | X.XX | XXX |
| 3 | [Make Name] | XX.X% | X.XX | XXX |
| 4 | [Make Name] | XX.X% | X.XX | XXX |
| 5 | [Make Name] | XX.X% | X.XX | XXX |

**Insight**: [Brief interpretation of large aircraft findings]

---

## Factor Analysis

### Factor 1: Weather Conditions

**Finding**: [Describe the relationship between weather and safety outcomes]

**Statistical Evidence**:
- VMC Destruction Rate: XX.X%
- IMC Destruction Rate: XX.X%
- Difference: XX.X percentage points
- Statistical Significance: p < 0.05 (t-test)

**Visualization**:
![Weather Impact](path/to/weather_chart.png)

**Recommendation**: [Practical recommendation based on findings]

---

### Factor 2: [Second Factor - Choose One]

**Finding**: [Describe the relationship]

**Evidence**:
- [Key statistics]
- [Comparison across categories]

**Visualization**:
![Factor 2 Impact](path/to/factor2_chart.png)

**Recommendation**: [Practical recommendation]

---

## Key Visualizations

### 1. Aircraft Size Distribution
[Insert or describe chart showing split between small/large aircraft]

### 2. Destruction Rate Comparison
[Insert or describe chart comparing destruction rates across top makes]

### 3. Injury Rate Trends Over Time
[Insert or describe chart showing how injury rates have changed]

### 4. [Factor] Impact on Safety
[Insert or describe chart showing relationship between factor and outcomes]

---

## Conclusions

### Main Takeaways

1. **For Small Aircraft**: [Summary of recommendations]

2. **For Large Aircraft**: [Summary of recommendations]

3. **Weather Impact**: [Brief conclusion about weather findings]

4. **[Second Factor] Impact**: [Brief conclusion about second factor]

### Limitations

- Analysis limited to accidents (does not include total flight hours/exposure)
- Missing data in some categories may affect completeness
- Historical data may not reflect current aircraft technology
- Sample sizes vary across makes/models

### Future Work

- Incorporate flight hours data for true accident rate calculation
- Analyze maintenance records and age of aircraft at time of accident
- Examine pilot experience and training factors
- Study geographical variations in accident patterns

---

## Technical Details

### Tools & Libraries
- **Python**: 3.12
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib**: Data visualization
- **Seaborn**: Statistical visualizations
- **SciPy**: Statistical testing

### Files in Repository
- `Aviation_Accident_Cleaning.ipynb`: Data cleaning and preparation
- `Aviation_Accident_Analysis.ipynb`: Exploratory data analysis
- `Aviation_Data_Cleaned.csv`: Cleaned dataset
- `README.md`: This file

### How to Run
1. Clone this repository
2. Install required packages: `pip install pandas numpy matplotlib seaborn scipy`
3. Download aviation accident data from [source]
4. Run notebooks in order:
   - First: `Aviation_Accident_Cleaning.ipynb`
   - Second: `Aviation_Accident_Analysis.ipynb`

---

## Contact

[Your Name]  
[Your Email]  
[LinkedIn Profile - Optional]

---

## Acknowledgments

- Data Source: National Transportation Safety Board (NTSB)
- Dataset available on Kaggle
- Course: [Course Name and Institution]
