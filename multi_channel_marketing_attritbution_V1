# Multi-Channel Marketing Attribution Pipeline

## 📌 Project Overview
This project simulates a realistic digital marketing data environment to evaluate the effectiveness of multi-channel campaigns. It features an end-to-end data pipeline that ingests raw, weighted touchpoint data, transforms it, and applies multiple attribution models (First-Touch, Last-Touch, and Linear) to accurately distribute conversion revenue across channels.

## 🛠️ The Tech Stack
* **Data Generation:** Python (`pandas`, `numpy`, `faker`)
* **Data Warehousing / Processing:** DuckDB (Simulating a cloud data warehouse environment like BigQuery)
* **Data Transformation:** SQL
* **Statistical Analysis:** Python (`scipy`, `statsmodels`)
* **Visualization:** Python (`seaborn`, `matplotlib`)

## 📊 The Business Problem
Digital marketing agencies frequently struggle to accurately attribute conversion revenue to the correct channels. Standard platforms often default to Last-Touch attribution, which artificially inflates the value of bottom-of-funnel channels (like Branded Search) while under-reporting the top-of-funnel channels (like Social Media) that generated the initial demand.

This project solves that by building a relational data pipeline capable of calculating and comparing First-Touch, Last-Touch, and Linear models, validated via statistical significance testing (One-Way ANOVA).

## 💡 Key Business Insights
Based on the funnel-biased data simulation, the following strategic insights were generated:
1. **Upper Funnel Dominance:** Meta and LinkedIn Ads dominate the first-touch model, proving highly effective at generating initial brand awareness and demand. 
2. **Google Ads as the Primary Closer:** Analyzing the last-touch attribution reveals that Google Ads is a critical component for capturing intent and driving final customer conversion.
3. **Revenue Concentration Risk:** Over 70% of the generated revenue is concentrated within just three paid channels, presenting a diversification risk for future campaigns.
4. **Underperformance of Organic Channels:** Organic Search and Email do not currently drive a proportional amount of revenue compared to paid channels, indicating a need to audit the SEO strategy and email nurture sequences.

## 🚀 Data Roadmap & Next Steps
* **Incorporate Cost & Efficiency Metrics:** Integrate daily ad spend data to calculate Return on Ad Spend (ROAS) and Cost Per Acquisition (CPA).
* **Deploy Algorithmic Attribution:** Move beyond standard rule-based heuristics by implementing data-driven, machine learning approaches (e.g., Markov Chains or Shapley values) to mathematically determine true incremental lift.
* **Connect Downstream CRM Metrics:** Analyze cohort retention and B2B churn to evaluate marketing channels based on long-term Customer Lifetime Value (LTV).
