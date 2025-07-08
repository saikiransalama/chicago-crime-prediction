# Crime Analytics in Chicago: Patterns, Predictions, and Policy Implications

## 📊 Project Overview

This comprehensive research project analyzes crime trends in Chicago from 2001 to 2025, utilizing advanced data analytics and machine learning techniques to understand crime patterns, predict arrest outcomes, and provide insights for law enforcement strategies. The study examines over 8 million crime incidents to identify spatial, temporal, and behavioral patterns that inform proactive policing approaches.

## 🎯 Research Objectives

- **Crime Pattern Analysis**: Identify the most frequent crime types and their distribution between residential and non-residential areas
- **Temporal Analysis**: Examine seasonal and daily patterns of violent vs. property crimes
- **Arrest Prediction**: Develop machine learning models to predict arrest outcomes based on incident characteristics
- **Forecasting**: Implement time-series models to forecast future crime trends
- **Policy Implications**: Provide data-driven recommendations for law enforcement resource allocation

## 📈 Key Findings

### 🏠 Spatial Distribution Patterns
- **Theft** emerges as the leading crime type, predominantly occurring in non-residential areas
- **Violent offenses** (assaults, domestic violence) primarily occur in residential neighborhoods
- **Narcotics violations** occur mostly in non-residential/public locations (>85%)
- **Burglary** shows higher rates in residential areas, requiring targeted prevention strategies

### 🌡️ Seasonal Crime Patterns
- **Violent crimes** peak significantly during summer months (June-August)
- **July** records the highest number of violent crimes, followed by August and June
- **February** (coldest month) shows the lowest violent crime rates
- **Property crimes** also increase in summer but with less dramatic variation than violent crimes
- **Arson** shows notable spikes during July (Fourth of July) and October (Halloween)

### ⏰ Temporal Patterns
- **Peak crime hours**: 6 PM to 11 PM (evening rush hours and social gatherings)
- **Violent crimes** spike during late night hours (8 PM to midnight)
- **Property crimes** continue into early hours due to shopping times and vacant residences
- **Weekend patterns**: Violent crimes peak on Saturdays, property crimes spike on Fridays
- **Lowest activity**: Early morning hours (4-6 AM)

### 🚔 Arrest Outcomes Analysis
- **High arrest rates** (>50%): Weapons violations, domestic violence incidents, public indecency
- **Low arrest rates** (<10%): Theft, burglary, arson (typically discovered post-incident)
- **Moderate arrest rates**: Assault and battery, robbery
- **Key factors** influencing arrests: Crime type, location description, domestic indicator, time of day

## 🔬 Methodology

### Data Source
- **Dataset**: City of Chicago Open Data Portal "Crimes from 2001 to 2025"
- **Records**: 8.14 million crime incidents
- **Variables**: 22 attributes including crime type, location, date/time, arrest outcomes
- **Time Period**: January 2001 to early 2025

### Analytical Techniques
1. **Exploratory Data Analysis (EDA)**
   - Statistical analysis of crime distributions
   - Seasonal and temporal pattern identification
   - ANOVA testing for significant differences

2. **Machine Learning Models**
   - **XGBoost Classification**: Arrest prediction (75% accuracy)
   - **LSTM Neural Networks**: Time-series crime forecasting
   - **Facebook Prophet**: Seasonal trend decomposition

3. **Statistical Analysis**
   - Two-way ANOVA for seasonal patterns
   - Post-hoc tests for month-by-month comparisons
   - Feature importance analysis

## 💻 Technical Implementation

### Analysis Notebooks
- **`Codebase_1.ipynb`**: Main analysis with comprehensive EDA, statistical testing, and machine learning models
- **`Codebase_2.ipynb`**: Additional exploratory analysis and model refinement

### Key Libraries Used
- **Data Manipulation**: pandas, numpy
- **Visualization**: matplotlib, seaborn, plotly
- **Machine Learning**: scikit-learn, xgboost, tensorflow
- **Time Series**: prophet, statsmodels
- **Statistical Analysis**: scipy, statsmodels

### Model Performance
- **XGBoost Arrest Prediction**: 75% cross-validated accuracy
- **Feature Importance**: Crime type, location, domestic indicator, time of day
- **Precision-Recall**: 0.6 precision, 0.5 recall for arrest class

## 📋 Project Structure

```
├── Codebase_1.ipynb              # Main analysis notebook (clean version)
├── Codebase_2.ipynb              # Additional analysis and model refinement
├── Research Paper.pdf            # Complete research findings and conclusions
└── README.md                    # This file
```

## 🎯 Policy Implications

### Resource Allocation
- **Summer months**: Increase patrol presence for violent crime prevention
- **Residential areas**: Focus on burglary prevention and domestic violence intervention
- **Commercial districts**: Implement theft prevention and surveillance measures
- **Weekend deployment**: Adjust officer schedules based on crime patterns

### Prevention Strategies
- **Community programs**: Summer youth programs and conflict resolution teams
- **Environmental design**: Improved lighting, locks, and surveillance in high-risk areas
- **Targeted interventions**: Domestic violence prevention in residential areas
- **Public awareness**: Seasonal crime prevention campaigns

## ⚠️ Limitations and Ethical Considerations

### Data Limitations
- Missing location descriptions may introduce bias
- Unreported crimes not captured in dataset
- Arrest variable oversimplifies complex law enforcement processes
- Temporal changes in demographics and policies may affect trends

### Ethical Considerations
- **Bias Prevention**: Fairness assessments in model development
- **Transparency**: Open communication about prediction methods
- **Community Impact**: Ensuring models don't disproportionately affect specific neighborhoods
- **Privacy Protection**: Safeguarding individual rights in predictive systems

## 🚀 Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/saikiransalama/chicago-crime-prediction
   cd chicago-crime-prediction
   ```

2. **Install dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow prophet
   ```

3. **Explore the analysis**:
   - Start with `Codebase_1.ipynb` for the main analysis
   - Review `Codebase_2.ipynb` for additional insights
   - Read `Research Paper.pdf` for complete findings

4. **Data Requirements**:
   - The analysis requires the Chicago crime dataset (2001-2025)
   - Dataset available from [Chicago Open Data Portal](https://data.cityofchicago.org/)
   - Large dataset files are excluded from this repository due to size constraints

## 📊 Results Summary

This research demonstrates the power of data-driven crime analysis in informing law enforcement strategies. Key contributions include:

- **Pattern Identification**: Clear seasonal and temporal crime patterns in Chicago
- **Predictive Modeling**: Successful implementation of machine learning for arrest prediction
- **Policy Recommendations**: Data-driven insights for resource allocation and prevention strategies
- **Methodological Framework**: Comprehensive approach combining EDA, statistical analysis, and ML
  
**Note**: This repository contains the analysis code and documentation. The large dataset files (Chicago crime data) are excluded due to size constraints but can be obtained from the Chicago Open Data Portal. 
