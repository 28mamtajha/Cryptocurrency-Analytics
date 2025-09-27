# 🚀 Project Overview  

This project builds an **end-to-end automated analytics pipeline** for cryptocurrency exchange data.  
It integrates **Apache Airflow, dbt, Snowflake, and Apache Superset** (all containerized with Docker)  
to enable scalable and near real-time crypto analytics.  

The pipeline extracts and processes historical and streaming data from **CoinAPI**, transforms it into  
structured analytical models, and provides visual insights into crypto market trends such as  
**Simple Moving Average (SMA), Relative Strength Index (RSI), and Price Momentum**.  

---

# 💼 Business Problem / Use Case  

Cryptocurrency markets are highly **volatile**, with prices changing rapidly across different exchanges.  
Traditional methods often fail due to:  

- ⚡ **High-frequency streaming data** that is difficult to process in real-time  
- 📊 Lack of **technical indicators** (SMA, RSI, momentum) for trading insights  
- 🔒 **Security concerns** with API keys & credentials in pipelines  

**Our Solution**:  

✅ Automated **ETL/ELT pipeline** using Airflow + dbt  
✅ Centralized **Snowflake warehouse** for structured crypto data  
✅ **Superset dashboards** for visual insights and decision-making  
✅ **Scalable & containerized** design with Docker  

**Use Case Example:**  
- Traders identify **buy/sell signals** (e.g., RSI < 30 → oversold, potential buy).  
- Analysts track **crypto market momentum** and volatility across trading pairs.  
- Engineers extend the pipeline for **new exchanges or tokens** with minimal effort.  

---

# 🔗 System Architecture  

<p align="center">
  <img src="system_architecture.png" width="600" alt="System Architecture Diagram"/>
</p>  

**Workflow**:  
1. **CoinAPI** → extracts crypto trading pairs (ETH/BTC, ADA/USDT, etc.)  
2. **Airflow DAGs** → orchestrate ETL into Snowflake  
3. **dbt models** → transform raw data into analytics tables (SMA, RSI, momentum)  
4. **Superset dashboards** → visualize insights in real-time  

---

# 📊 Key Features  

- **ETL with Airflow** → Extracts, transforms, and loads data into Snowflake  
- **ELT with dbt** → Builds staging models and calculates indicators  
- **Data Warehouse (Snowflake)** → Ensures SQL-based structured storage  
- **Visualization (Superset)** → Dashboards with RSI trends, SMA composition, momentum vs trade count  
- **Security** → API keys & credentials stored securely via Airflow Connections & Variables  
- **Scalability** → Entire environment containerized with Docker  

---

# 🛠️ Languages & Tools  

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white&style=for-the-badge" />
  <img src="https://img.shields.io/badge/SQL-336791?logo=postgresql&logoColor=white&style=for-the-badge" />
  <img src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white&style=for-the-badge" />
  <img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?logo=apache-airflow&logoColor=white&style=for-the-badge" />
  <img src="https://img.shields.io/badge/dbt-FF694B?logo=dbt&logoColor=white&style=for-the-badge" />
  <img src="https://img.shields.io/badge/YAML-CB171E?logo=yaml&logoColor=white&style=for-the-badge" />
  <img src="https://img.shields.io/badge/Apache%20Superset-1F92D1?logo=apache-superset&logoColor=white&style=for-the-badge" />
  <img src="https://img.shields.io/badge/Snowflake-29B5E8?logo=snowflake&logoColor=white&style=for-the-badge" />
  <img src="https://img.shields.io/badge/Data%20Pipeline-FF6F00?logo=databricks&logoColor=white&style=for-the-badge" />
</p>  

---

# 📈 Example Visualizations  

- 📉 **RSI Over Time** → track overbought/oversold signals  
- 🥧 **SMA Composition** → distribution of moving averages across trading pairs  
- 📊 **Momentum vs Trade Count** → identify phases of heavy trading activity  

---

# 📂 Repository  

📌 [Cryptocurrency-Analytics](https://github.com/28mamtajha/Cryptocurrency-Analytics)  

