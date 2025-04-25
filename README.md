# Telecom Customer Survival Analysis

## Overview
This repository contains the code and analysis for the Survival Analysis homework assignment. The goal of this project is to analyze telecom customer churn data using Accelerated Failure Time (AFT) models, calculate Customer Lifetime Value (CLV), and identify factors affecting customer churn risk.

## Dataset
The dataset (`telco.csv`) contains information about 1,000 telecom subscribers, including:
- Demographic information (age, gender, income, etc.)
- Service usage (voice, internet, call forwarding)
- Customer category (Basic, Plus, E-service, Total service)
- Churn status

## Project Structure
- `Survival_Analysis_Telecom_Churn.ipynb`: Main Jupyter notebook containing all analysis code
- `requirements.txt`: List of Python dependencies
- `README.md`: This file providing an overview of the project
- `Report.md`: Summary of findings and recommendations

## Analysis Steps
1. Data exploration and preprocessing
2. Building and comparing different AFT models (Weibull, LogNormal, LogLogistic)
3. Feature selection to identify significant factors affecting churn
4. Customer Lifetime Value (CLV) calculation
5. Identification of valuable customer segments
6. Determination of retention budget and strategy recommendations

## Key Findings
- The LogNormal AFT model provides the best fit for this dataset
- Internet service is the strongest predictor of customer retention
- Plus service customers have the highest CLV ($1,443.77) and lowest churn rate (4.6%)
- Basic service customers have the highest churn rate (18.9%)
- Zero overlap between high-value and high-risk customers indicates a strong inverse relationship
- Recommended annual retention budget: $6,347.52

## Requirements
To run this notebook, you'll need the Python packages listed in `requirements.txt`. You can install them using:

```
pip install -r requirements.txt
```

## Usage
1. Clone this repository
2. Install the required dependencies
3. Place the `telco.csv` file in the same directory
4. Run the Jupyter notebook:
```
jupyter notebook Survival_Analysis_Telecom_Churn.ipynb
```


