# Students' Mental Health Analysis

YOU CAN CHECK OUT MY [PROJECT REPORT](https://github.com/khoapham1002/University-Mental-Health-Research-Study/blob/main/notebooks/students_analysis.ipynb) FIRST!

## Table of Contents
1. [Overview](#overview)
2. [Setup](#setup)
3. [Key Questions](#key-questions)
4. [Methodology](#methodology)
  - [Data](#data)
  - [Tools and Techniques](#tools-and-techniques)
5. [Findings](#findings)
  - [Social Connectedness](#social-connectedness)
  - [Acculturative Stress](#acculturative-stress)
  - [Length of Stay](#length-of-stay)
  - [Machine Learning Performance](#machine-learning-performance)
6. [Recommendations](#recommendations)

## Overview
This project investigates the mental health of international students at a university, exploring the impact of social connectedness, acculturative stress, and length of stay on depression levels. Using statistical analysis and machine learning models, the study provides actionable insights and recommendations to improve student well-being.

## Setup
Install required libraries:
<!-- Using pip: -->
```bash
pip install -r requirements.txt
```

<!-- Using conda: -->
```bash
conda env create -f environment.yml
```

<!-- Clone the repository: -->
```bash
git clone https://github.com/kdpham-01002/University-Mental-Health-Research-Study.git
```

## Key Questions
1. How do social connectedness and acculturative stress influence depression scores among international students?
2. Does length of stay moderate the effects of stress and connectedness on depression?
3. Can machine learning models accurately predict depression scores and identify high-risk students?


## Methodology

### Data
- **Dataset**: Survey responses from 200+ international students.
- **Key Variables**:
  - `todep`: Depression scores (PHQ-9).
  - `tosc`: Social connectedness scores (SCS).
  - `toas`: Acculturative stress scores (ASISS).
  - `stay`: Length of stay (in years).
  - Demographics: Age, academic level, language proficiencies.

### Tools and Techniques
- **Python**:
  - Libraries: `pandas`, `matplotlib`, `seaborn`, `statsmodels`, `sklearn`.
  - Purpose: Data preprocessing, visualization, statistical analysis, and machine learning.
- **SQL**:
  - Used for data extraction and filtering in a SQLite database.
- **Statistical Analysis**:
  - Correlation analysis and hypothesis testing to identify significant predictors.
  - Interaction effects to explore how length of stay impacts stress and connectedness relationships.
- **Machine Learning**:
  - Random Forest Regression to predict depression scores.
  - Random Forest Classification to identify high-risk students.


## Findings
1. **Social Connectedness**:
   - Strong negative correlation with depression (\(r = -0.54\), \(p < 0.01\)).
   - Students with higher social connectedness have significantly lower depression scores.

2. **Acculturative Stress**:
   - Moderate positive correlation with depression (\(r = 0.41\), \(p < 0.01\)).
   - Higher stress levels are associated with increased depression risk.

3. **Length of Stay**:
   - No direct effect on depression (\(r = 0.07\), \(p = 0.30\)).
   - Marginally weakens the impact of acculturative stress on depression over time.

4. **Machine Learning Performance**:
   - **Random Forest Regression**:
     - Mean Squared Error (MSE): 17.59.
   - **Random Forest Classification**:
     - Accuracy: 75%.
     - Precision (Class 0 - Not at Risk): 0.77.
     - Recall (Class 1 - High Risk): 0.45.


## Recommendations
1. **Peer Support Programs**:
   - Encourage social connections to reduce depression risk.
2. **Acculturation Workshops**:
   - Focus on early-stage students to alleviate acculturative stress.
3. **Early Warning Systems**:
   - Use machine learning models to identify high-risk students and prioritize interventions.
