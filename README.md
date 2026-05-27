# Emilio Rojas's Portfolio Analytics and Data Science Projects
Hi! I'm Emilio Rojas, a data and analytics professional with a passion for the intersection of technology, behavioral science, and business strategy. I love turning complex data into clear decisions that actually move the needle.
My background spans operations and growth analytics, experimentation, and data product building across Latin America's tech ecosystem (Rappi, Nestlé) and recently the research world at [Duke's Center for Advanced Hindsight](https://advanced-hindsight.com/), where I get to explore how behavioral science can reshape financial products.

I just finished my Master of Quantitative Management in Business Analytics at Duke Fuqua, and I'm always chasing the next thing to learn and have an impact, whether that's a new modeling technique, a framework I haven't tried, or a dataset that makes me rethink my assumptions.

When I'm not wrangling data, you'll find me on the tennis court, traveling somewhere new, playing guitar, or most recently learning the art of tattooing. I figure if you're going to be curious, you might as well be curious about everything.

Let's connect in [LinkedIn](https://www.linkedin.com/in/emilio-rojas-flores/) and/or shoot me an email (emilio.rojas@duke.edu). Happy to chat.

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

