# Customer & Marketing Analytics (DS458)
## Framework for Retail Performance Evaluation and Predictive Modeling

## Project Overview
This project presents an empirical data analytics framework designed to evaluate retail transaction performance, model customer behavior, and deploy descriptive and predictive analytics pipelines. Utilizing a structured methodology across **Excel, Power BI, and Python**, the study conducts a multi-phase analysis on a statistically significant random sample of **50,000 transaction records** to address market concentration risks and optimize demand forecasting.

---

## Methodology & Technical Pipeline

### 1. Data Engineering & Preprocessing (Excel)
* **Data Cleansing:** Standardized textual attributes and product descriptions via `TRIM` and `PROPER` functions to eliminate structural inconsistencies.
* **Data Integrity:** Executed deduplication protocols and filtered structural null values by removing records lacking a validated `CustomerID`.
* **Feature Engineering:** Derived binary transactional states (`Completed` vs. `Canceled`), calculated absolute `Total Sales`, and isolated temporal dimensions (`Year`, `Month`, `Hour`) to enable chronological trend mapping.

### 2. Descriptive Business Intelligence (Power BI)
* **Data Modeling:** Developed a relational schema enforcing a many-to-one (`*:1`) cardinality between core transactional tables and product dimensions.
* **Temporal Intelligence:** Engineered a dedicated **Calendar Table** utilizing Data Analysis Expressions (DAX) to compute time-intelligence metrics including Year-to-Date (YTD) revenue and Year-over-Year (YoY) growth variance.
* **Analytical Visualizations:** Deployed analytical reporting layers including variance tracking via Waterfall charts, composition mapping via Treemaps, and target baseline evaluations via Gauge indicators.

### 3. Statistical Modeling & Explainable AI (Python)
* **Time-Series Forecasting:** Implemented AI-driven Exponential Smoothing (ETS) models to generate deterministic future revenue projections.
* **Statistical Auditing:** Deployed Z-Score filtering methodologies to differentiate data entry anomalies from legitimate macroeconomic data points.
* **Explainable AI (XAI):** Applied SHAP (SHapley Additive exPlanations) structural force plots to audit high-magnitude outlier transactions, ensuring transparency in algorithmic classifications.

---

## Empirical Findings & Quantitative Insights

* **Geographic Concentration Risk:** Exploratory Pivot Table analysis confirmed that the **UK market accounts for over 80% of aggregate revenue**, indicating a critical structural vulnerability to localized market shifts.
* **Financial Performance:** Documented **$1.05M in total sales** against an institutional target baseline of **$1.5M**.
* **Seasonal Variance:** Identified significant temporal fluctuations, with YoY growth achieving a peak variance of **+47.26%** within the December cyclical window.
* **Model Validation:** Quantitative SHAP auditing verified that a massive statistical outlier (an isolated order of 488k units) represented a legitimate wholesale transaction originating from a UK entity, mitigating data-entry error hypotheses.

---

## Strategic Recommendations

1. **Geographic Diversification:** MIT Open-market expansion strategies target emerging high-yield territories (e.g., Saudi Arabia) to reduce dependency metrics within the UK perimeter.
2. **Customer Segmentation Protocols:** Establish an institutional tiered rewards architecture optimized for the "Priority" user cohort (defined as individual transaction values exceeding $100) to lower customer attrition rates.
3. **Supply Chain Optimization:** Scale inventory buffer coefficients for high-velocity SKUs (e.g., *Regency Cakestand*) by a minimum of 60 days prior to the documented November seasonal demand surge.
4. **Data Governance Automation:** Integrate automated data validation constraints directly at the database entry level to systematically prevent manual data-entry errors.

---

## Ethical Governance & Data Privacy

* **Anonymization Protocols:** Enforced rigorous data privacy standards by excluding all Personally Identifiable Information (PII) and substituting surrogate keys for customer records.
* **Statistical Objectivity:** Utilized standardized Z-Score boundaries to preserve data distribution honesty and prevent management skew from statistical outliers.
* **Algorithmic Accountability:** Integrated deterministic SHAP analysis to ensure machine learning inferences remain interpretable, accountable, and free from algorithmic bias.

---

## Repository Structure
```text
├── BA Project REPORT.pdf    # The executive project report
├── EXEL FILE.xlsx           # Standardized transactional dataset
├── PART 1.pbix              # Relational modeling & initial transformations
├── PART 2.pbix              # Time-intelligence metrics & analytical reporting
├── PART 3.pbix              # Predictive visualizations & forecasting layers
└── README.md                # Institutional documentation
