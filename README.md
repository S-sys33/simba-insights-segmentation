# Simba Insights — Customer Segmentation Pipeline

## 📌 Business Problem
Small businesses often treat all customers the same, wasting marketing budgets on broad campaigns. This project builds an automated ETL (Extract, Transform, Load) pipeline that takes raw CRM data, scores customers using RFM (Recency, Frequency, Monetary) analysis, and outputs actionable marketing segments.

## 💡 Key Insight (The "Aha!" Moment)
When run on a dataset of 2,193 customers, the pipeline revealed that the **"At Risk" segment** (24% of customers) held **39.5% of total revenue ($524,000)**. These are high-spenders who hadn't purchased recently. Identifying this segment allows businesses to deploy targeted win-back campaigns, potentially saving hundreds of thousands in revenue.

## 🛠️ Tech Stack
*   **Language:** Python (pandas, numpy)
*   **Data Transformation:** Feature engineering, data cleaning (handling missing values, deduplication, text normalization), RFM Scoring.
*   **Visualization:** Google Looker Studio
*   **Data Source:** Kaggle (Customer Personality Analysis)

## 🚀 The Live Dashboard
The output of the Python script is exported to a CSV, which feeds a live Looker Studio Dashboard. 
👉 **[View the Live Dashboard Here](https://datastudio.google.com/reporting/6c63e3d0-bdd8-4858-9efa-bd4fcaa27407)** 

## 💻 How to Run the Pipeline
1. Clone this repository.
2. Ensure you have `pandas` and `numpy` installed (`pip install pandas numpy`).
3. Run the script:
   ```bash
   python simba_insights_pipeline.py --input marketing_data.csv --outdir output/
   ```
4. The script will clean the data, assign RFM scores, and export `segment_summary.csv` for dashboarding.

---
*Built by Simbarashe Phiri | Founder of Simba Insights Marketing Agency*
