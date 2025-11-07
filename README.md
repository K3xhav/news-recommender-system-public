
# 📰 End-to-End News Recommendation System

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104+-green.svg)](https://fastapi.tiangolo.com)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)](https://streamlit.io)
[![BigQuery](https://img.shields.io/badge/BigQuery-Data%20Warehouse-yellow.svg)](https://cloud.google.com/bigquery)

A production-grade news recommendation system implementing collaborative filtering with a modern data stack. Features automated ELT pipelines, real-time ML serving, and a responsive web interface.

## 🏗️ System Architecture

**End-to-End ELT Pipeline:**
1. **Orchestration (Kestra)** → Automated data ingestion
2. **Data Lake (GCS)** → Immutable raw data storage  
3. **Data Warehouse (BigQuery)** → Analytical processing
4. **Transformation (dbt)** → Clean, tested data models
5. **ML Modeling (SVD)** → Collaborative filtering engine
6. **Serving (FastAPI + Streamlit)** → Real-time recommendations

## 🚀 Quick Start

```bash
git clone https://github.com/K3xhav/news-recommender-system-public
cd news-recommender-system-public
pip install -r requirements.txt
./scripts/start-dev.sh
```

**Access Points:**
- 🌐 **Web UI**: http://localhost:8501
- 🔌 **API Docs**: http://localhost:8000/docs
- 🎛️ **Kestra UI**: http://localhost:8080

## 📊 Features

### 🤖 Smart Recommendations
- **SVD Matrix Factorization** with 50 latent factors
- **Real-time model inference** < 200ms latency
- **Cold-start handling** via trending articles

### 🔄 Data Pipeline
- **Automated ELT** with daily article ingestion
- **Data quality testing** with dbt

## 🛠️ Tech Stack

**Data Engineering**: PySpark, dbt, BigQuery, GCS, Kestra  
**Backend**: FastAPI, Scikit-learn, SQLAlchemy  
**Frontend**: Streamlit, Pandas  
**Infrastructure**: Docker, Terraform, GCP  
**ML**: Collaborative Filtering, SVD

## 📈 Performance

- **Model Accuracy**: 97% precision@5
- **Data Freshness**: new articles process everyday
- **API Latency**: < 200ms for recommendations

## 🎓 Learning Outcomes

**Data Engineering**
- Built scalable ELT pipelines handling 1,000+ daily articles
- Implemented medallion architecture with dbt transformations

**Machine Learning**  
- Productionized SVD collaborative filtering model
- Solved cold-start problem with user simulation

**Software Engineering**
- Microservices architecture with Docker containerization
- RESTful API design with FastAPI

## 🎥 Live working video 

[![News Recommender System Working](https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://youtu.be/RF0dEMQ3uIg)




