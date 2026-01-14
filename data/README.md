# Data Directory

This directory contains the datasets used in the customer churn analysis for BizGrow.

## Dataset Overview

The following datasets are available for analysis:

### dataset1.csv - SalesForce Export
Contains customer contract and demographic information:
- Contract dates
- Company size
- Industry classification

**Data Quality Note:** The industry field is approximately 30% empty. This missing data must be addressed in the analysis.

### dataset2a for q1 q2.csv - Usage Logs (Q1-Q2)
Daily login activity for customers during Q1 and Q2.

**Data Quality Note:** Standard usage patterns observed during this period.

### dataset2b for q3 q4.csv - Usage Logs (Q3-Q4)
Daily login activity for customers during Q3 and Q4.

**Data Quality Note:** European server logs are corrupted for September. Analysis must account for this data quality issue.

### dataset3.csv - Support Tickets
Unstructured text of customer complaints and support interactions.
- Contains both sales-related and product-related issues
- Requires text analysis to categorize and extract insights

## Data Preprocessing Considerations

When working with these datasets, consider the following:

1. **Missing Industry Data:** Approximately 30% of records in the SalesForce export lack industry classification. Consider imputation strategies or separate analysis of records with/without this field.

2. **Corrupted EU Logs:** September usage data from European servers is unreliable. Either exclude this data or clearly flag it in visualizations and statistical analyses.

3. **Unstructured Support Tickets:** Text data requires cleaning, categorization, and potentially sentiment analysis or topic modeling.

4. **Data Integration:** Cross-referencing between datasets may require careful key matching and handling of temporal misalignments.

## Usage

All analysis scripts should load data from this directory. Example:

```python
import pandas as pd

# Load SalesForce data
salesforce_df = pd.read_csv('data/dataset1.csv')

# Load Q1-Q2 usage logs
usage_q1q2_df = pd.read_csv('data/dataset2a for q1 q2.csv')

# Load Q3-Q4 usage logs
usage_q3q4_df = pd.read_csv('data/dataset2b for q3 q4.csv')

# Load support tickets
support_df = pd.read_csv('data/dataset3.csv')
```
