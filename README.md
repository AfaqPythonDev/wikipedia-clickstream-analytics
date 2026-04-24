# 🌐 Wikipedia Clickstream Analytics

**Big Data Analytics Project | BS 6th Semester**

## 👥 Group Members
| Name | Roll No |
|------|---------|
| Mehak Ali | 14862 |
| Tamseel | 14984 |
| Afaq Ahmad | 13932 |
| Laeeq Ahmad | 14923 |

**Submitted to:** Muhammad Sadique

## 📌 Project Overview
A production-grade Big Data pipeline that processes and analyzes 
Wikipedia clickstream and pageview data using the Medallion 
Architecture (Bronze → Silver → Gold) on Databricks.

## 🛠️ Technology Stack
| Tool | Purpose |
|------|---------|
| Databricks | Cloud platform & notebooks |
| Apache Spark (PySpark) | Distributed data processing |
| Delta Lake | Data storage with ACID transactions |
| Databricks SQL | Analytics & dashboard |
| GitHub | Version control |

## 🏗️ Pipeline Architecture
Raw Data → Bronze Layer → Silver Layer → Gold Layer → Dashboard

## 📊 Data Sources
- **Wikipedia Clickstream** (~500MB/month) - wikimedia.org
- **Wikipedia Pageviews** (~2GB/day) - wikimedia.org

## 📓 Notebooks
| Notebook | Description |
|----------|-------------|
| 01_bronze_ingestion | Raw data ingestion into Delta Lake |
| 02_silver_cleaning | Data cleaning & validation |
| 03_gold_analytics | 6 analytical queries & aggregations |

## 🔍 Analytical Questions Answered
1. Top 10 most viewed Wikipedia articles
2. Most common entry pages (via search)
3. Most common exit pages
4. Top two-step navigation paths (A→B→C)
5. Traffic distribution across articles
6. Click type breakdown (link vs other)

## 📈 Key Results
- **39 million+** records processed
- **25 million** clean records after filtering
- **2.3 billion** total clicks analyzed
- Top article: **Main_Page** (57K views/hour)
- Most common path: **One_Direction → Liam_Payne → Cheryl**

## 🔗 Live Dashboard
[View Wikipedia Analytics Dashboard](https://dbc-7c7ce75e-49ea.cloud.databricks.com/dashboardsv3/01f13fa6c3181ebe8647da2950c2c76f/published?o=7474647038996372)

## 📁 Project Structure
wikipedia-clickstream-analytics/
├── 01_bronze_ingestion.ipynb
├── 02_silver_cleaning.ipynb
├── 03_gold_analytics.ipynb
└── README.md
