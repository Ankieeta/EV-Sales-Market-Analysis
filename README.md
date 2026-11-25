# EV Sales & Market Analysis

## Project Overview
An end-to-end Python data analytics pipeline that cleans, transforms, and analyzes Electric Vehicle (EV) sales and market data to generate business insights, visual charts, and summary reports.

## 📂 Project Structure
```text
EV Sales & Market Analysis/
├── data/                   # Raw and processed EV datasets
├── src/                    # Modular Python scripts
│   ├── config.py           # File paths and project configuration
│   ├── data_loader.py      # Dataset ingestion utilities
│   ├── data_transformation.py # Data cleaning and feature engineering
│   └── analysis.py         # Metric calculations and market aggregations
├── outputs/                # Generated project artifacts
│   ├── analysis/           # Summary CSV tables and statistical outputs
│   ├── graphs/             # Visualizations and market trend charts
│   └── reports/            # Automated business insight reports
├── EV_Analysis.ipynb       # Interactive Jupyter Notebook with visual walkthrough
├── main.py                 # Main entry point to run the full ETL & analysis pipeline
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
'''
1: Project Overview & Objective

• Goal: Analyze Electric Vehicle (EV) registration and population data to uncover market trends, top manufacturers, and adoption patterns.
• Dataset: Electric_Vehicle_Population_Data.csv containing vehicle details such as VIN, Model Year, Make, Model, EV Type (BEV vs. PHEV), Electric Range, and Location.
• End Deliverable: Automated Python data pipeline, visual charts, a business insights summary, and a final PDF market report.

2: Tech Stack & Tools Used

• Programming Language: Python 3.14
• Data Processing: Pandas (data loading, cleaning, transformation, and aggregation)
• Data Visualization: Matplotlib / Seaborn (generating market trend charts)
• Reporting & Exploration: Automated PDF report generator (report.py) and Jupyter Notebook for interactive presentation

3: Project Architecture (Modular Pipeline)

• config.py: Centralizes all input/output file paths so the project runs cleanly across environments.
• data_loader.py: Validates and loads the raw CSV dataset with automatic delimiter and encoding handling.
• data_cleaning.py: Removes duplicates, handles missing values, and standardizes data types for accuracy.
• data_transformation.py: Creates derived features and prepares structured data for market metrics.
• analysis.py & visualization.py: Computes key business insights and exports high-resolution charts.
• report.py & main.py: Combines findings and visuals into a final PDF report with a single command (python main.py).

4: Key Analysis Areas (What the Data Answers)

• Market Growth Over Time: Year-over-year surge in EV adoption across model years.
• Top Automakers & Models: Market share dominance among leading EV brands and most popular vehicle models.
• BEV vs. PHEV Split: Comparison between Battery Electric Vehicles (100% electric) and Plug-in Hybrid Electric Vehicles.
• Range & Eligibility Insights: Distribution of electric driving range and Clean Alternative Fuel Vehicle (CAFV) eligibility.
• Geographic Distribution: Top counties and cities driving EV adoption.

5: Outputs & Business Value

• Cleaned Dataset (ev_cleaned.csv): Ready-to-use structured data for future modeling or dashboarding.
• Visual Charts (outputs/graphs/): Clear visual storytelling for stakeholders.
• Business Insights (business_insights.txt) & PDF Report (EV_Sales_Market_Report.pdf): Actionable takeaways on consumer preferences, brand competition, and infrastructure demand.

6: Future Improvements

• Interactive Dashboard: Build a live Streamlit or Power BI dashboard with filters by brand, year, and city.
• Predictive Forecasting: Add machine learning models to forecast future EV adoption rates.
• Charging Infrastructure Overlay: Combine EV population data with charging station locations to identify underserved areas.


## How to Run
1.Clone the repository:
   ```bash
   git clone https://github.com
   cd "EV Sales & Market Analysis"
   ```

2. Activate the virtual environment:
   ```bash
   .venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the analysis pipeline:
   ```bash
   python main.py
   ```

