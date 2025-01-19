# A/B Testing for User Completion Rates and Behavior Analysis

This project analyzes an A/B test conducted to evaluate the impact of a new user experience variation (Test) compared to the existing design (Control). The goal was to measure completion rates, time spent on steps, error rates, and drop-off rates to determine whether the Test variation improves user engagement and efficiency.

## Dataset Description
The dataset consists of user interactions at different process steps:
- **Process Steps:** `start`, `step_1`, `step_2`, `step_3`, `confirm`
- **Key Metrics Analyzed:** 
  - Completion rates
  - Time spent per step
  - Error rates (step backs, step repeats)
  - Drop-off rates

## Hypothesis & Testing Approach
### 1️. Completion Rates
- **Hypothesis:** Users in the Test group will have a significantly higher completion rate.
- **Null Hypothesis:** No significant difference between Test and Control completion rates.
- **Result:** Test group completion rate **↑ 1.53%** compared to Control (**statistically significant**).

### 2️. Time Spent Per Step
- **Hypothesis:** The Test group will complete steps faster than the Control group.
- **Findings:** Test users were **slower at start and step 1**, but **faster at step 2 and step 3**.

### 3️. Error Rates (Step Backs & Step Repeats)
- **Hypothesis:** Test users will experience fewer errors.
- **Findings:** Error rates were **mostly similar**, but Test users had **more step back errors at the start**.

### 4️. Drop-Off Rates
- **Hypothesis:** The Test group will have lower drop-offs at key steps.
- **Findings:** Drop-off rates **were slightly higher in the Test group at the start**, indicating initial friction.

## Key Findings & Insights
- **Test variation led to a 1.53% absolute increase in completion rates** (statistically significant).  
- **Test group had higher drop-offs and step-back errors at the start**, indicating possible UX friction.  
- **Test users were faster in later steps (`step_2` and `step_3`)**, suggesting an overall efficiency gain.  
- **Step 1 took longer in the Test group**, which may indicate complexity in navigation.  

### Recommendation
- **Optimize the start step UX** to reduce initial drop-offs.
- **Investigate delays in step 1** to improve efficiency.
- **Iterate on the Test variation based on user feedback** and run a follow-up experiment.

## Repository Structure
/ab_testing_project/
│── 📄 README.md  # Project documentation
│── 📄 data.csv   # Dataset used for analysis
│── 📄 analysis.ipynb  # Jupyter Notebook with data exploration and statistical tests
│── 📄 results_summary.md  # Summary of results & conclusions
│── 📄 requirements.txt  # Dependencies for running the project

## How to Run the Analysis

git clone https://github.com/akprodromou/vanguard-ab-testing.git

pip install -r requirements.txt




