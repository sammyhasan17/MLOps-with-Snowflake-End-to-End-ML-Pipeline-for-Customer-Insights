# 🚀 MLOps with Snowflake: End-to-End ML Pipeline for Customer Insights

**My Original Notebook in Snowflake:**  
[notebook 1 on Snowflake](https://app.snowflake.com/us-east-1/rlc50566/#/notebooks/HOL_DB.HOL_SCHEMA.%22notebook%201%22)

---

## 💡 Project Overview

Built an **end-to-end, cloud-native machine learning pipeline in Snowflake** for multilingual sentiment analysis and customer purchase prediction, leveraging distributed compute and modern NLP models (Hugging Face BART).


## Context

- E-commerce furniture retailer with multilingual product reviews (EN/ES/PT/FR).  
- **Objective:** Transform unstructured customer feedback into actionable insights and predict purchase likelihood to increase sales and reduce churn.  
- **Requirement:** Keep all data and processing inside Snowflake for governance, security, and scalability.

## Action

- Unified review, clickstream, and transaction data in Snowflake via **Snowpark**.  
- Applied **multilingual NLP** (Cortex AI + Hugging Face BART) for sentiment and topic detection, distributed with **Ray Data**.  
- Built **XGBoost** purchase propensity model using sentiment, product attributes, and behavioral signals.  
- Automated the pipeline with **remote ML jobs** and **DAG scheduling** for daily retraining and scoring.

## Results (Business Impact)

- uplift in marketing conversion by targeting high-propensity customers.  
- reduction in churn via proactive engagement with at-risk customers.  
- faster issue resolution for low-sentiment SKUs, improving brand trust.   
- Scalable to new regions and product lines without additional infrastructure.

---

## 🔗 Features & Architecture

### 1. Multilingual Review Ingestion
- Pull customer reviews from Snowflake stages
- Parallel processing with **Ray Data**

### 2. AI-Powered Text Analysis
- **Cortex AI** and **Hugging Face BART** for:
  - 🌍 **Sentiment Analysis** (multi-language)
  - 🧠 **Transformer-based Review Classification** (Ray for batch inference)

### 3. Predictive Modeling
- **XGBoost** to predict purchase decisions:
  - Uses review text features, ratings, sentiment, page load times, and more

### 4. Full Snowflake Integration
- **Snowpark**: Unified DataFrame & SQL access
- **Ray**: Distributed model training/inference  
- **Compute Pools**: Python execution at scale  
- **Warehouses**: Scalable SQL queries  
- **Cluster scaling** for fast compute

### 5. Automated MLOps
- **Remote ML jobs** for data and model updates
- **Model Registry** for logging & explainability
- **DAG tasks** for daily retraining, scheduling, and monitoring

---

## ⚡️ Why Use This Pipeline?

- **Cut manual work**—auto-ingest, analyze, and predict from all customer feedback  
- **See actionable insights instantly**  
- **Boost revenue** by targeting likely buyers and solving product issues faster  
- **Modern, scalable, fully cloud-native—**run everything inside Snowflake!

---

## 🧩 More on End-to-End ML in Snowflake

> Dive deeper into how Snowflake enables **ML workflows**:  
> [Snowflake ML](https://www.snowflake.com/en/product/features/end-to-end-ml-workflows/?utm_source=on24&utm_medium=referral&utm_campaign=0n24-webinars-resource-box)

