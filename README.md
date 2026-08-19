# Emilio Rojas's Portfolio 
Hi! I'm Emilio Rojas, a data and analytics professional with a passion for the intersection of technology, behavioral science, and business strategy. I love turning complex data into clear decisions that actually move the needle.
My background spans operations and growth analytics, experimentation, and data product building across Latin America's tech ecosystem (Rappi, Nestlé) and recently the research world at [Duke's Center for Advanced Hindsight](https://advanced-hindsight.com/), where I get to explore how behavioral science can reshape financial products.

I just finished my Master of Quantitative Management in Business Analytics at Duke Fuqua, and I'm always chasing the next thing to learn and have an impact, whether that's a new modeling technique, a framework I haven't tried, or a dataset that makes me rethink my assumptions.

When I'm not wrangling data, you'll find me on the tennis court, traveling somewhere new, playing guitar, or most recently learning the art of tattooing. I figure if you're going to be curious, you might as well be curious about everything.

Let's connect in [LinkedIn](https://www.linkedin.com/in/emilio-rojas-flores/) and/or shoot me an email (emilio.rojas@duke.edu). Happy to chat.


### 🎵 [Photo Vibe Music Recommender (Picmu)](https://github.com/emiliorojasflo/picmu)
**Tech Stack:** Python, Streamlit, Anthropic API (Claude Vision), Spotify Web API, Pandas

* **The Goal:** Build and ship an end-to-end AI product. Upload a photo, get music recommendations matching its vibe in Spotify. From concept to a publicly deployed app in less than 2 hrs.
* **The Execution:** Used Claude Vision to convert images into structured genre signals, matched them against a 6,276-genre real-world taxonomy, and layered in preference-weighted recommendations with a built-in discovery pick. Integrated the Spotify API for live search, redesigning around Spotify's Feb 2026 endpoint deprecations.
* **Business Impact:** Demonstrates rapid full-stack product development and the ability to redesign an architecture on the fly when a core third-party dependency changed mid-build — a common real-world constraint in shipped software.


### 📊 [Multi-Channel Marketing Attribution Pipeline](https://github.com/emiliorojasflo/marketing_rule_based_attribution_models)
**Tech Stack:** Python (pandas, scipy), DuckDB, SQL, Seaborn
* **The Goal:** Understand the fundamentals of rule-based attribution models in digital marketing by building a relational data pipeline capable of distributing conversion revenue across multiple marketing channels.
* **The Execution:** Generated synthetic, funnel-biased B2B data to mimic real customer journeys. Built an automated ETL pipeline using DuckDB to calculate First-Touch, Last-Touch, and Linear attribution models.
* **Business Impact:** In the future, being able to apply inferential statistics (One-Way ANOVA & Tukey HSD) to mathematically prove which channels drive actual business momentum versus statistical noise, providing actionable reallocation strategies for ad spend.

### 📧 [AI-Powered Job Application Tracker](https://github.com/emiliorojasflo/job_application_tracking_automation)
**Tech Stack:** Google Apps Script (JavaScript), Gmail API, Google Sheets API, Anthropic Claude API
* **The Goal:** Eliminate manual tracking of job applications by automatically detecting application-related emails (in English and Spanish), classifying their pipeline status, and surfacing the data in a clean, editable dashboard — without standing up any backend infrastructure.
* **The Execution:** Built a serverless polling pipeline on Google Apps Script that pre-filters Gmail with a multilingual query, sends each candidate thread to Claude Haiku for structured-output classification (company, role, status, salary, location, source), and upserts the result into an auto-generated Google Sheet. Implemented a monotonic state machine so application status only advances forward, an Event Log tab for full classification auditability, and a `diagnose()` function for layer-by-layer observability.
* **Business Impact:** Reduced job-search tracking manual effort while preserving full control over the data. The architecture demonstrates a key engineering trade-off: replacing a planned full-stack web app (Next.js + Postgres + 6–8 week OAuth verification) with a zero-infrastructure Apps Script + Sheet pattern cut time-to-ship from weeks to a single afternoon, at a runtime cost of under $4/month per user.

### 📊 [Loan Portfolio Risk Monitor](https://github.com/emiliorojasflo/loan_portfolio_risk)
**Tech Stack:** dbt, Snowflake, Python (pandas, snowflake-connector), SQL, Looker Studio
* **The Goal:** Build an end-to-end analytics engineering pipeline that transforms raw consumer loan-level data into a portfolio risk monitor — using the Lending Club dataset as a proxy for consumer refinancing portfolios, with modeling patterns that translate directly to student loan refi books like Earnest's.
* **The Execution:** Designed a layered ELT pipeline that loads 2.2M+ loans into Snowflake via a chunked, idempotent Python loader storing everything as VARCHAR, then transforms the data through a dbt project structured as staging → intermediate → marts with materialization strategy chosen per layer (views for staging, ephemeral for intermediate, tables for marts). Implemented credential management via environment variables and `env_var()` in profiles, automated data quality tests at every layer, auto-generated lineage documentation via `dbt docs`, and a normalized loan status taxonomy (active / paid_off / delinquent / default / charged_off) preserving the raw source values for debug traceability.
* **Business Impact:** Delivered analyst-ready marts surfacing portfolio composition by grade and geography, vintage performance by origination cohort, and credit risk segmentation by purpose and FICO band — enabling Risk and Product teams to monitor default rates over time, identify underperforming segments, and make underwriting and pricing decisions backed by clean, version-controlled, trusted data.
