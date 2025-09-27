**Overview**

This project builds an end-to-end automated analytics pipeline for cryptocurrency exchange data. It integrates Apache Airflow, dbt, Snowflake, and Apache Superset (all containerized with Docker) to enable scalable and near real-time crypto analytics.

The pipeline extracts and processes historical and streaming data from CoinAPI, transforms it into structured analytical models, and provides visual insights into crypto market trends such as Simple Moving Average (SMA), Relative Strength Index (RSI), and Price Momentum.

**Tech Stack**

Data Source: CoinAPI
Orchestration: Apache Airflow
Transformation & Modeling: dbt (Data Build Tool)
Data Warehouse: Snowflake
Visualization: Apache Superset
Containerization: Docker

**Pipeline Architecture**

**ETL with Airflow**

Extracts data from CoinAPI

Transforms raw API responses

Loads cleaned data into Snowflake

**ELT with dbt in Airflow**
Staging and modeling of crypto data

Calculates key metrics:

SMA (7-day moving average)

RSI (7-day relative strength index)

Price Momentum

**Visualization with Superset**
Interactive dashboards for time-series trends, SMA composition, and trade momentum analysis.

**Data Models**

Raw Table: user_db_camel.raw.crypto_currencies – stores raw trading data

Analytics Models:

crypto_sma – 7-day SMA

crypto_rsi – RSI calculations

crypto_price_momentum – momentum direction classification

crypto_abstract_metrics – final consolidated metrics table used for visualization

**Features**

Automated scheduling and orchestration via Airflow DAGs
Secure storage of API keys & credentials with Airflow Connections/Variables
Transactional integrity & idempotent inserts for reliability
Testing with dbt to ensure data quality and model consistency
Snapshots for historical versioning of both raw and abstract metrics

**Example Visualizations**

RSI Over Time – track overbought/oversold signals

SMA Composition – distribution of moving averages across trading pairs

Momentum vs. Trade Count – identify active trading phases
