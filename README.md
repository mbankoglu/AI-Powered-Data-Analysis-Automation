*Project: AI-Powered Data Analysis Automation*

Overview: This project automates key steps of the data analysis process using n8n, JavaScript, and AI. The workflow accepts CSV and Excel files, cleans and analyzes the data, generates AI-assisted findings, and produces visual HTML and Markdown reports.

The goal of this project was to reduce time spent on repetitive data preparation and initial exploratory analysis while providing a structured starting point for deeper investigation.

🔗 View the HTML Dashboard: 
https://mbankoglu.github.io/AI-Powered-Data-Analysis-Automation/auto_data_analysis_report.html

🔗 Data Analysis Automation Workflow:
Screenshots/n8n workflow.png

Tools:
- n8n
- Gemini AI
- JavaScript
- HTML
- CSV/XLSX

Features:
- Data cleaning:
    + Standardizes column names and text formatting
    + Removes unnecessary spaces and text-entry errors
    + Detects and removes duplicate records
    + Identifies numerical and categorical fields automatically

- Missing value imputation:
    + Fills missing numerical values using median imputation
    + Fills missing categorical values using mode imputation
    + Produces a complete dataset for downstream analysis

- Statistical analysis:
    + Calculates row and column counts
    + Generates missing value summaries
    + Computes descriptive statistics including mean, median, minimum, and maximum values
    + Produces categorical frequency distributions

- AI-generated recommendations
    + Uses an AI agent to interpret analysis results
    + Identifies notable patterns and potential data quality issues
    + Suggests next steps for deeper investigation and analysis
    + Generates executive-style summaries and findings

- HTML dashboard reporting
    + Creates a visual HTML report automatically
    + Includes KPI cards, summary tables, charts, and AI-generated insights
    + Provides a shareable report that can be opened in any web browser

- Markdown reporting
    + Generates a text-based analysis report
    + Summarizes dataset characteristics, key findings, and recommendations
    + Suitable for documentation and project records

- - Workflow Architecture

Manual Trigger
- Import CSV / Excel File
- Data cleaning
- Missing Value Imputation (median/mode)
- Save cleaned dataset
- Statistical Analysis
- AI Analysis & Recommendations
- HTML Dashboard Generation
- Markdown Report Generation
- Export Results 

Example Outputs
- Cleaned Dataset (CSV)
- Markdown Analysis Report
- HTML Dashboard Report with Visualizations

Future Advancements:
- implement Advanced Imputation techniques: KNN & MICE



  
