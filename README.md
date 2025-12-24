# 📊 Media Coverage & Brand Intelligence Reporting Dashboard

## Overview
This project demonstrates an end-to-end **media intelligence and reporting workflow**, similar to those used by media monitoring and communications analytics teams. It focuses on collecting unstructured news data, applying structured content coding, enforcing data quality standards, and generating executive-ready insights through visual analysis and reporting.

The project is designed to mirror real-world responsibilities of a **Data Analyst in a media intelligence environment**, with an emphasis on accuracy, consistency, and stakeholder-friendly reporting.

---

## Business Objective
Brands generate large volumes of media coverage across publishers daily. However, raw media content is unstructured and not directly suitable for reporting.

**Objective of this project:**
- Convert raw news articles into structured, reportable intelligence
- Analyze media volume, sentiment, topics, and publisher impact
- Deliver executive-ready insights suitable for communication and strategy teams

---

## Data Source
- **NewsAPI** – Used to collect real-time news articles based on brand-specific keywords
- Coverage limited to English-language articles within a defined time window

---

## Project Workflow

### 1. Media Data Collection
- Fetched real-time news articles using NewsAPI
- Extracted structured metadata including title, source, publish date, description, and URL
- Stored raw data for reproducibility

### 2. Content Coding & Classification
Articles were coded using a **rule-based, explainable framework** across:
- **Topic** (Technology, Finance, Product, Policy, Business, Other)
- **Sentiment** (Positive, Neutral, Negative)
- **Mention Type** (Primary vs Secondary brand mention)
- **Region** (inferred conservatively from source)

### 3. Data Validation & Quality Enforcement
- URL-level deduplication to prevent over-counting
- Timestamp normalization to UTC for global consistency
- Schema and coding consistency checks
- Flagging of low-quality or incomplete records

### 4. Exploratory Analysis & Visualization
- Daily media coverage trends
- Topic and sentiment distribution
- Sentiment trends over time
- Top publishers by coverage volume
- Primary vs secondary brand mention analysis

### 5. Executive Reporting
- Insights translated into concise, neutral narratives
- Findings structured into an executive-style report
- Recommendations provided based on observed media patterns

---

## Key Insights (Sample)
- Media coverage volume remained stable with no volatility-driven spikes
- Technology-led narratives dominated overall coverage
- Neutral sentiment increased over time while negative sentiment declined
- Coverage was distributed across multiple publishers with no single-source dominance
- Majority of brand mentions were secondary, indicating presence within broader industry discussions

---

## Tools & Technologies
- **Python**
- **Pandas**
- **Matplotlib**
- **VADER Sentiment Analysis**
- **Google Colab**
- **Markdown / PowerPoint-style reporting**

---

## Repository Structure

```text
media-coverage-analysis/
│
├── data/
│   ├── raw/                # Raw NewsAPI data
│   └── processed/          # Cleaned and validated datasets
│
├── charts/                 # Exported visualizations
│
├── Media Coverage Analysis & Brand Intelligence.ipynb
│
├── Media-Coverage-and-Brand-Intelligence-Report.pptx
├── Media-Coverage-and-Brand-Intelligence-Report.pdf
└── README.md
