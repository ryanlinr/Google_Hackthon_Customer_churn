# Google Hackathon - Customer Churn Analysis

## Project Overview

This repository contains the team's work for the Google Hackathon focused on customer churn analysis. Our objective is to identify the single biggest leak in customer retention and provide a specific, actionable recommendation to fix it.

## Repository Structure

```
.
├── reports/          # Team reports and documentation (PDF files)
├── analysis/         # Analysis code and scripts
├── data/            # Data files (excluded from git for large files)
└── README.md        # This file
```

### 📄 Reports

The `reports/` directory contains all team reports in PDF format, including:
- Data analysis reports
- Findings and insights
- Recommendations and conclusions

See [reports/README.md](reports/README.md) for more details.

### 💻 Analysis Code

The `analysis/` directory contains all code used for the customer churn analysis, including:
- Data preprocessing scripts
- Exploratory data analysis
- Machine learning models
- Visualization code
- Jupyter notebooks

See [analysis/README.md](analysis/README.md) for more details on running the code.

### 📊 Data

The `data/` directory is for storing datasets. Large data files are excluded from version control.

See [data/README.md](data/README.md) for data descriptions and access instructions.

## Getting Started

### For Team Members

1. **Clone the repository**
   ```bash
   git clone https://github.com/ryanlinr/Google_Hackthon_Customer_churn.git
   cd Google_Hackthon_Customer_churn
   ```

2. **Upload Reports**
   - Add your PDF reports to the `reports/` directory
   - Use descriptive filenames (e.g., `customer_analysis_2024-01-15.pdf`)
   - Update `reports/README.md` with a brief description

3. **Upload Analysis Code**
   - Add your Python scripts or notebooks to the `analysis/` directory
   - Document dependencies in `requirements.txt`
   - Update `analysis/README.md` with descriptions of your scripts

4. **Commit and Push**
   ```bash
   git add .
   git commit -m "Add analysis report and code"
   git push
   ```

### Running Analysis Code

```bash
# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies (once requirements.txt is created)
pip install -r requirements.txt

# Run analysis scripts
python analysis/your_script.py
```

## Project Goals

**Objective**: Identify the single biggest leak in customer retention and give a specific, actionable recommendation to fix it.

### Key Questions
- What are the primary factors driving customer churn?
- Which customer segments are most at risk?
- What actionable interventions can reduce churn?

## Contributing

### Team Workflow

1. Create a descriptive branch for your work
2. Add your reports to `reports/` or code to `analysis/`
3. Update relevant README files with descriptions
4. Commit with clear, descriptive messages
5. Push and create a pull request

### Code Standards

- Write clean, commented code
- Include docstrings for functions
- Follow PEP 8 for Python code
- Test your code before committing

## Contact

For questions about the project or repository, contact the team lead.

## License

This project is part of the Google Hackathon competition.
