# Google Hackathon - Customer Churn Analysis

## Hackathon Problem Statement: Understanding Customer Churn

### The Business Scenario

You are the Analytics Task Force for BizGrow, a SaaS platform helping SMBs manage inventory. Until recently, growth was explosive. However, Q3 results just came in, and they are disastrous: Customer Churn has spiked from 4% to 12% in a single quarter.

The Chief Operating Officer has called an emergency meeting. But there appears to be more questions than answers as various teams come up with conflicting points of view:

- **Sales Leadership claims:** "The product is broken; customers are leaving because the new dashboard is too slow."
- **Product Leadership claims:** "Sales is acquiring low-quality customers who go out of business in 3 months. The product is fine."
- **Customer Support team claims:** "We are overwhelmed by tickets and nobody listens to the customer."

The COO has called you in. They do not want a dashboard. They do not want a list of 50 charts. They have one request:

**"We have limited resources. I need you to identify the single biggest leak in our customer retention and give me a specific, actionable recommendation to fix it. Convince me I'm making the right decision."**

### The Data

You have been given access to three raw datasets. Warning: These datasets have real-world flaws (missing values, inconsistent definitions) that you must handle as you build your case.

- **SalesForce Export:** Contract dates, company size, and industry (Warning: Industry field is approximately 30% empty).
- **Usage Logs:** Daily login activity (Warning: European server logs are corrupted for September).
- **Support Tickets:** Unstructured text of customer complaints (Sales vs. Product issues).

### The Deliverable

Your team has 8 minutes to present a slide deck to the COO. Your presentation must tell a coherent story that leads to a recommendation.

While you are submitting one deck, your narrative must demonstrate that you have navigated the Analytics Project Lifecycle taught in this course:

#### I. The Setup
Don't just report "Churn." How did your team define churn for this specific crisis?

#### II. The Diagnosis
Show us how you prioritized. You cannot fix everything. Use the 80/20 rule to show which specific segment is driving the crisis.

#### III. The Evidence
Prove your diagnosis is real and not just data noise. How did you validate your findings despite the messy data?

#### IV. The Recommendation
End with a clear, narrative-driven conclusion. What is the one action the COO should take?

### Evaluation Rubric

| Criteria | Weight | What we are looking for |
|----------|--------|-------------------------|
| **Problem Scoping** | 25% | Did they clearly define what they are solving (and what they are not solving)? Did they handle the missing EU data logically? |
| **Analytical Rigor** | 25% | Did they use the data to find the "80/20" driver? Did they validate their assumptions (e.g., cross-referencing different data sources and insights)? |
| **Business Logic** | 25% | Does the recommendation actually make business sense? (e.g., "Fire the sales team" is not a realistic recommendation). |
| **Storytelling & Communication** | 25% | Is the deck "Executive Ready"? Did they focus on the "So What" rather than showing 10 slides of Python code? |

## Repository Structure

```
.
├── reports/          # Team reports and documentation (PDF files)
├── analysis/         # Analysis code and scripts
├── data/            # Dataset files
└── README.md        # This file
```

### Reports

The `reports/` directory contains all team reports in PDF format, including:
- Data analysis reports
- Findings and insights
- Recommendations and conclusions

See [reports/README.md](reports/README.md) for more details.

### Analysis Code

The `analysis/` directory contains all code used for the customer churn analysis, including:
- Data preprocessing scripts
- Exploratory data analysis
- Machine learning models
- Visualization code
- Jupyter notebooks

See [analysis/README.md](analysis/README.md) for more details on running the code.

### Data

The `data/` directory contains the datasets used in the analysis:
- `dataset1.csv` - SalesForce Export (contract dates, company size, and industry)
- `dataset2a for q1 q2.csv` - Usage Logs for Q1 and Q2
- `dataset2b for q3 q4.csv` - Usage Logs for Q3 and Q4
- `dataset3.csv` - Support Tickets (unstructured text of customer complaints)

See [data/README.md](data/README.md) for detailed data descriptions.

## Getting Started

### Prerequisites

```bash
# Clone the repository
git clone https://github.com/ryanlinr/Google_Hackthon_Customer_churn.git
cd Google_Hackthon_Customer_churn

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Running Analysis Code

```bash
# Run analysis scripts
python analysis/your_script.py
```

## Project Methodology

This analysis follows a structured approach to address the business problem:

1. **Problem Definition:** Clearly define what constitutes customer churn in the context of BizGrow's Q3 crisis
2. **Data Exploration:** Understand the structure, quality, and limitations of the available datasets
3. **Root Cause Analysis:** Use the 80/20 principle to identify the primary driver of churn
4. **Validation:** Cross-reference findings across multiple data sources to ensure robustness
5. **Actionable Recommendation:** Provide a specific, implementable solution with clear business impact

## Contributing

### Code Standards

- Write clean, well-documented code
- Include docstrings for functions and classes
- Follow PEP 8 style guidelines for Python code
- Test your code before committing
- Update relevant README files with descriptions of new scripts or analysis

## Contact

For questions about the project or repository, contact the project lead.

## License

This project is part of the Google Hackathon competition.
