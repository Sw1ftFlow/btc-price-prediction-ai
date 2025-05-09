# 🪙 BTC Price Prediction with AI, Databricks & Airflow

This is an end-to-end learning project using **Databricks**, **Airflow**, and **AI/ML models** to predict the price of **Bitcoin (BTC)** based on historical cryptocurrency data from the **CoinGecko API**.

---

## 📌 Project Goals

- Ingest historical BTC data via public API (CoinGecko)
- Build a Lakehouse pipeline in **Databricks** using Delta tables
- Orchestrate the workflow using **Darabricks Workflows**
- Train an AI model (XGBClassifier) to forecast BTC price increase or decrease

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Databricks** | Data engineering, processing & model training |
| **Darabricks Workflows** | Orchestration of data ingestion & model runs |
| **CoinGecko API** | Source of BTC market data |
| **Python** | Core language |

---

## 📈 Data Source

**CoinGecko Market Chart API**

- Endpoint: `https://api.coingecko.com/api/v3/coins/bitcoin/market_chart`
- Frequency: Hourly
- Data: `price`, `market_cap`, `volume`
- Time Period: Last 90 days

---

## 📂 Project Structure

```text
btc-price-prediction-ai/
├── notebooks/
│   ├── 01_ingest_data_coingecko.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_model_training.ipynb
├── workflows/
│   └── btc_price_predictions
├── data/
│   └── (optional sample data files)
├── README.md
├── requirements.txt
└── LICENSE
```

---

## 🚀 How to Run

### 1. Clone the repo

```bash```
```git clone https://github.com/Sw1ftFlow/btc-price-prediction-ai.git```
```cd btc-price-prediction-ai```
### 2. Install requirements
```bash```
pip install -r requirements.txt
### 3. Setup Databricks
- Import notebooks under /notebooks/
- Configure your cluster
- Set up access tokens if needed

### 4. Run Databricks Workflow (Optional)
- Trigger Workflow to ingest data & train models

## 🔮 Example Forecast Plot
<img width="1190" alt="btc_price_prediction_chart" src="https://github.com/user-attachments/assets/f6f3960c-f09c-4c34-8557-781479e3f7b8" />


## 💡 Future Improvements
- Add twitter data and intepret sentiment with llm
- Use exchange APIs for real-time data & order books



