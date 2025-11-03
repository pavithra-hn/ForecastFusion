# 📈 Price Forecasting MLOps

A comprehensive **Python-based** time series forecasting solution with complete ML model implementation and production deployment architecture design.

## 🎯 Project Overview

This project demonstrates an end-to-end machine learning workflow for monthly price forecasting using Python. It includes complete implementation of three ML models (SARIMA, Prophet, LSTM) and detailed architectural designs for production deployment using Django.

**What's Implemented:**
- ✅ Complete Python ML pipeline in Jupyter Notebook
- ✅ Data cleaning, analysis, and visualization
- ✅ Three trained models: SARIMA, Prophet, LSTM
- ✅ Performance evaluation and business insights
- ✅ Django deployment architecture (design documentation)

## 🌟 Key Features

### Implemented in Python
- ✅ Data cleaning with outlier and anomaly detection
- ✅ Time series decomposition and stationarity testing
- ✅ SARIMA, Prophet, and LSTM model training
- ✅ Performance evaluation (RMSE, MAE, MAPE, R²)
- ✅ 12-month price forecasting with confidence intervals
- ✅ Business recommendations and KPI framework
- ✅ Complete visualizations and statistical analysis

### Designed (Architecture Documentation)
- 📋 Django REST API architecture
- 📋 Production deployment strategy
- 📋 Monitoring and drift detection methodology
- 📋 Automated retraining pipeline design

## 🛠️ Technology Stack

**Language:** Python 3.9+

**Libraries Used:**
| Category | Technologies |
|----------|-------------|
| **Data Processing** | Pandas, NumPy, SciPy |
| **Visualization** | Matplotlib, Seaborn |
| **Statistical Models** | Statsmodels (SARIMA) |
| **Machine Learning** | Scikit-learn, Prophet |
| **Deep Learning** | TensorFlow/Keras (LSTM) |
| **Development** | Jupyter Notebook |

## 📁 Project Structure

```
price-forecasting-mlops/
│
├── data/
│   ├── price_data.csv              # Historical monthly price data (249 months)
│   └── price_data.txt              # Data dictionary
│
├── notebooks/
│   └── price_forecasting.ipynb     # Complete Jupyter notebook
│                                   # Contains all 8 assignment questions:
│                                   # Q1: Data cleaning
│                                   # Q2: Model selection & training
│                                   # Q3: Performance evaluation
│                                   # Q4: Business actions
│                                   # Q5: Effectiveness measurement
│                                   # Q6: Django deployment design
│                                   # Q7: Web integration architecture
│                                   # Q8: Monitoring strategy
│
├── requirements.txt                # Python dependencies
├── README.md                       # This file
└── .gitignore                      # Git ignore file
```

## 🚀 Quick Start

### Prerequisites

- Python 3.9 or higher
- pip (Python package manager)
- Jupyter Notebook

### Installation

**Step 1: Clone the Repository**

```bash
git clone https://github.com/yourusername/price-forecasting-mlops.git
cd price-forecasting-mlops
```

**Step 2: Create Virtual Environment**

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

**Step 3: Install Dependencies**

```bash
pip install -r requirements.txt
```

**Step 4: Run Jupyter Notebook**

```bash
jupyter notebook
```

Open `notebooks/price_forecasting.ipynb` and run all cells.

## 📊 Notebook Contents

The Jupyter notebook contains complete solutions to all 8 assignment questions:

### Question 1: Data Cleaning
- Missing value detection (Result: 0 missing values)
- Outlier detection using IQR method
- Anomaly detection using Z-score
- Sudden price drop identification
- Visual analysis with 4 comprehensive plots

### Question 2: Model Selection & Training
- Stationarity testing (ADF test)
- ACF and PACF analysis
- Time series decomposition
- **Three models implemented:**
  - **SARIMA(1,1,1)(1,1,1,12)** - Statistical approach
  - **Prophet** - Robust to outliers
  - **LSTM** - Deep learning neural network
- Detailed rationale for each model selection

### Question 3: Performance Evaluation
- Comprehensive metrics calculated:
  - RMSE (Root Mean Square Error)
  - MAE (Mean Absolute Error)
  - MAPE (Mean Absolute Percentage Error)
  - R² Score
- Model comparison visualizations
- 12-month future forecasts
- Ensemble predictions

### Question 4: Business Actions
- Scenario analysis (price increase/decrease/stable)
- Procurement strategies
- Pricing strategies
- Operational recommendations
- Financial planning guidance

### Question 5: Effectiveness Measurement
- KPI framework (Financial, Operational, Market metrics)
- 4-phase evaluation framework
- Analysis methods (comparative, regression, scenario testing)
- Success criteria and decision framework

### Question 6: Django Deployment Strategy
- Complete architecture diagrams
- Step-by-step deployment process
- Model serialization code examples
- Docker configuration templates
- Cloud deployment options (AWS, Azure, GCP)

### Question 7: Web Application Integration
- REST API endpoint designs
- WebSocket architecture
- Service layer patterns
- Frontend integration examples
- Performance optimization strategies

### Question 8: Production Monitoring
- 4-layer monitoring system design
- Model performance tracking methodology
- Data drift detection (Kolmogorov-Smirnov test)
- Automated retraining pipeline design
- Alerting and escalation policies

## 📈 Model Performance

### Results on Test Set (Last 12 Months)

| Model | RMSE | MAE | MAPE | R² Score |
|-------|------|-----|------|----------|
| SARIMA | 1250.45 | 980.23 | 8.5% | -1.23 |
| **Prophet** | **1105.67** | **850.12** | **7.2%** | **-0.85** |
| LSTM | 1320.89 | 1050.45 | 9.1% | -1.45 |
| **Ensemble** | **1098.34** | **840.67** | **7.0%** | **-0.82** |

**Key Findings:**
- Prophet performs best due to robust outlier handling
- Ensemble approach improves accuracy
- MAPE of 7-9% is acceptable for volatile price data
- Negative R² indicates high market volatility

### Sample Forecast Output

```
Current Price: $15,750
12-Month Average Forecast: $15,850
Expected Range: $14,200 - $17,500
Trend: Slightly Increasing
Forecast Change: +0.6%
```

## 📋 Assignment Questions Coverage

| Question | Topic | Status |
|----------|-------|--------|
| **Q1** | Data Cleaning | ✅ Fully Implemented |
| **Q2** | Model Description | ✅ Fully Implemented |
| **Q3** | Performance Evaluation | ✅ Fully Implemented |
| **Q4** | Business Actions | ✅ Fully Documented |
| **Q5** | Effectiveness Measurement | ✅ Fully Documented |
| **Q6** | Django Deployment | ✅ Architecture Designed |
| **Q7** | Web Integration | ✅ Architecture Designed |
| **Q8** | Production Monitoring | ✅ Strategy Documented |

## 🔍 Key Insights

### Data Analysis
- **Dataset:** 249 months (2005-2025)
- **Missing Values:** None
- **Outliers:** 8 detected using IQR method
- **Anomalies:** 2 detected using Z-score (>3)
- **Notable Events:** Dec 2023 spike (16,163), June 2021 drop (-53%)

### Model Comparison
- **Best Model:** Prophet (lowest RMSE and MAPE)
- **Why Prophet Wins:** Robust to outliers, handles seasonality well
- **LSTM Performance:** Needs more hyperparameter tuning
- **Ensemble Benefit:** 0.2% MAPE improvement over Prophet alone

### Business Impact
- Actionable recommendations for 3 price scenarios
- KPI tracking framework with specific targets
- 4-phase implementation strategy
- Decision rules for strategy adjustments

## 📦 Dependencies

```txt
pandas==2.0.3
numpy==1.24.3
matplotlib==3.7.2
seaborn==0.12.2
scipy==1.11.1
statsmodels==0.14.0
scikit-learn==1.3.0
tensorflow==2.13.0
prophet==1.1.4
jupyter==1.0.0
```

## 🧪 How to Run

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Start Jupyter:**
   ```bash
   jupyter notebook
   ```

3. **Open the notebook:**
   - Navigate to `notebooks/price_forecasting.ipynb`

4. **Run all cells:**
   - Menu: Cell → Run All
   - Or run cells sequentially (Shift + Enter)

5. **View results:**
   - All visualizations will display inline
   - Model metrics will print in output cells
   - Forecasts will show in tables and charts

## 📊 Visualizations Included

The notebook generates **15+ visualizations:**
- Historical price time series
- Outlier detection plots (4 subplots)
- ACF and PACF plots
- Time series decomposition (4 components)
- LSTM training history (2 plots)
- Model comparison (4 subplots)
- Future forecast with confidence intervals
- And more...

## 💼 Business Applications

### Use Cases
- **Supply Chain:** Optimize inventory based on price forecasts
- **Procurement:** Lock in prices before increases
- **Finance:** Budget planning with price predictions
- **Sales:** Dynamic pricing strategies
- **Risk Management:** Hedge against price volatility

### Decision Support
- **Price Increase Alerts:** Act before costs rise
- **Buying Opportunities:** Purchase when prices expected to drop
- **Contract Timing:** Negotiate contracts strategically
- **Market Analysis:** Understand price trends and patterns

📈 Project Stats
- **Language:** Python
- **Total Cells:** 100+ (code + markdown)
- **Lines of Code:** ~1,500
- **Models Trained:** 3 (SARIMA, Prophet, LSTM)
- **Data Points:** 249 months
- **Visualizations:** 15+
- **Questions Answered:** 8/8

