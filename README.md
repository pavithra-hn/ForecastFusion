# 📈 Price Forecasting MLOps  

An end-to-end **MLOps system** for time series price forecasting with automated retraining, monitoring, and cloud-ready deployment.


## 🎯 Overview  
**Price Forecasting MLOps** is a production-grade forecasting system combining **SARIMA**, **Prophet**, and **LSTM** models.  
It supports **real-time predictions**, **drift detection**, **automated model retraining**, and **Dockerized cloud deployment** via a **Django REST API**.

## 🌟 Key Features  
- Multi-model forecasting: **SARIMA**, **Prophet**, **LSTM**  
- **REST API** & **WebSocket** for real-time predictions  
- Automated retraining on **data drift**  
- Monitoring: RMSE, MAE, MAPE, R² with alert system  
- **Docker-based deployment** (Django, Redis, PostgreSQL)  
- Business insights and KPI tracking  


## 🛠️ Tech Stack  
**Machine Learning:** Prophet, LSTM (TensorFlow), SARIMA (Statsmodels)  
**Backend:** Django REST Framework, Celery, Channels  
**Database:** PostgreSQL, Redis  
**Deployment:** Docker, Nginx, Gunicorn  
**Monitoring:** Custom scripts / Prometheus + Grafana (optional)  

## 🗂️ Project Structure

price-forecasting-mlops/
│
├── notebooks/ # Exploratory analysis & training notebook
├── forecasting_app/ # Core Django app
│ ├── ml_models/ # Model training, loading & prediction
│ ├── monitoring/ # Drift detection & performance tracking
│ ├── services/ # Prediction service
│ └── views.py # REST API endpoints
│
├── docker/ # Docker configurations & Compose setup
├── requirements.txt # Dependencies
├── README.md # Documentation
└── .env.example # Environment variable template

## 🚀 Quick Start  

### Prerequisites  
- Python 3.9+  
- Docker & Docker Compose  
- PostgreSQL 13+  
- Redis 6+  

### Installation  
git clone https://github.com/yourusername/price-forecasting-mlops.git
cd price-forecasting-mlops
pip install -r requirements.txt
cp .env.example .env
python manage.py migrate
python manage.py runserver
docker-compose up -d
