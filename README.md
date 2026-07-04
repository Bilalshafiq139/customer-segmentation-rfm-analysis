# RFM Customer Segmentation Analysis

This project is a portfolio-ready customer analytics case study built with RFM analysis: Recency, Frequency, and Monetary value. It uses online retail transaction data to segment customers, understand purchasing behavior, and recommend practical marketing actions.

The project includes Python analysis, Power BI dashboarding, a written report, and a presentation deck. It is structured to show both technical execution and business communication.

## Executive Summary

Customer segmentation helps a retail business move from generic promotions to targeted customer engagement. In this project, raw transaction data is transformed into customer-level RFM metrics, scored, segmented, visualized, and converted into recommendations for retention, reactivation, and revenue growth.

The analysis answers:

- Which customers are most valuable?
- Which customers show loyal or repeat-purchase behavior?
- Which customers may need reactivation?
- Which countries and products contribute most to customer value?
- Which marketing actions should be prioritized for each segment?

## Business Problem

Retail teams often have large transaction datasets but limited visibility into customer behavior. Without segmentation, campaigns can become broad, expensive, and difficult to prioritize.

This project solves that problem by grouping customers based on:

- How recently they purchased
- How frequently they purchased
- How much monetary value they generated

These metrics create a practical foundation for loyalty campaigns, reactivation campaigns, premium offers, and product-focused recommendations.

## Project Objectives

- Clean and prepare online retail transaction data.
- Calculate customer-level Recency, Frequency, and Monetary metrics.
- Create stable RFM scores using rank-based quartiles.
- Assign customers to business-friendly segments.
- Analyze customer behavior by segment, country, product, spend, and purchase frequency.
- Present findings through notebook, dashboard, report, and presentation outputs.

## Deliverables

- Analysis notebook: `notebooks/rfm_customer_segmentation_analysis.ipynb`
- Power BI dashboard: `dashboard/rfm_powerbi_dashboard.pbix`
- Final report: `reports/rfm_analysis_report.pdf`
- Presentation deck: `presentation/rfm_analysis_presentation.pptx`
- Project brief: `docs/project_brief.md`
- Raw dataset: `data/data.csv`
- Cleaned RFM output: `data/cleaned_rfm_customer_segments.csv`
- Dataset notes: `data/README.md`

## Methodology

1. Imported and inspected the online retail dataset.
2. Removed records that could not support valid customer-level RFM analysis.
3. Converted invoice dates into a usable time-series format.
4. Calculated Recency, Frequency, and Monetary values for each customer.
5. Applied quartile scoring to create RFM scores.
6. Assigned customers to meaningful business segments.
7. Compared segment behavior across geography, products, frequency, and spend.
8. Built visual outputs and translated the results into recommendations.

## Customer Segments

The notebook identifies practical customer groups, including:

- High-Value Customers
- Potential Loyal Customers
- Big Spenders
- Recent Customers
- Churn Risk Customers
- Other Customers

## Key Insights

- High-value customers are concentrated in major markets, especially the United Kingdom.
- Potential loyal customers show repeat-purchase behavior and are strong candidates for retention campaigns.
- Big spenders contribute meaningfully to revenue and can be targeted with premium offers.
- Recent customers should receive follow-up campaigns that encourage a second purchase.
- Product-level patterns help identify which items are most relevant for each segment.

## Recommendations

- Prioritize loyalty campaigns for high-value and potential loyal customers.
- Use reactivation campaigns for customers with high recency values.
- Create premium offers for big spenders.
- Promote frequently purchased products to segments that already show demand.
- Build country-specific campaigns where customer concentration is strongest.
- Track RFM movement over time to detect customers moving into risk or high-value groups.

## Tools and Technologies

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Plotly
- PrettyTable
- Power BI
- Jupyter Notebook

## Repository Structure

```text
RFM-Analysis/
  dashboard/
    rfm_powerbi_dashboard.pbix
  data/
    README.md
    cleaned_rfm_customer_segments.csv
    data.csv
    data_source.txt
  docs/
    project_brief.md
  notebooks/
    rfm_customer_segmentation_analysis.ipynb
  presentation/
    rfm_analysis_presentation.pptx
  reports/
    rfm_analysis_report.pdf
  .gitignore
  requirements.txt
  README.md
```

## How to Run

Install dependencies:

```bash
pip install -r requirements.txt
```

Register the project environment as a notebook kernel:

```bash
python -m ipykernel install --user --name rfm-analysis --display-name "Python (RFM Analysis)"
```

Open the notebook and select the kernel `Python (RFM Analysis)`:

```bash
jupyter notebook notebooks/rfm_customer_segmentation_analysis.ipynb
```

To execute the notebook from the command line:

```bash
python -m jupyter nbconvert --to notebook --execute notebooks/rfm_customer_segmentation_analysis.ipynb --inplace
```

## Data

The repository includes the raw dataset and the cleaned RFM output so the project can be cloned and run without extra download steps.

- Raw input: `data/data.csv`
- Cleaned output: `data/cleaned_rfm_customer_segments.csv`

The final notebook cell regenerates the cleaned output after the analysis is run. Dataset source references are available in `data/data_source.txt`.

## Portfolio Value

This project demonstrates a complete analytics workflow: data cleaning, feature engineering, customer segmentation, visualization, business interpretation, dashboarding, reporting, and executive-style presentation.
