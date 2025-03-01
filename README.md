# Uber Dashboard Project

![Python](https://img.shields.io/badge/Python-3.9-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Dataframe-orange.svg)
![GCP](https://img.shields.io/badge/GCP-Cloud%20Platform-yellow.svg)
![BigQuery](https://img.shields.io/badge/BigQuery-Data%20Warehouse-blue.svg)
![Looker Studio](https://img.shields.io/badge/Looker%20Studio-Dashboard-red.svg)
![MAGE AI](https://img.shields.io/badge/MAGE%20AI-Pipeline%20Tool-purple.svg)
![GitHub](https://img.shields.io/badge/GitHub-Version%20Control-black.svg)

## Overview
This project focuses on building an Uber ride analytics dashboard using Google Cloud Platform (GCP). The data is stored in GCP Bucket Storage, processed through an API call on **MAGE AI**, and then transferred to **BigQuery** for further transformations. The centralized table is then used to create an interactive dashboard in **Looker Studio**.

## Workflow
1. **Data Upload**: Raw Uber ride data is uploaded to **GCP Bucket Storage**.
2. **API Integration**: The data is fetched via an **API call** to **MAGE AI pipeline** on a Compute Instance.
3. **ETL Processing**: 
   - **Python** and **Pandas** are used for cleaning and transformation.
   - The processed data is stored in **BigQuery**.
4. **Data Centralization**: BigQuery processes and stores the transformed data in a **centralized table**.
5. **Dashboard Creation**: The centralized table is visualized using **Looker Studio** to generate insights.

## Technologies Used
- **Google Cloud Platform (GCP)**
  - Cloud Storage
  - Compute Engine
  - BigQuery
- **MAGE AI** (Pipeline Tool)
- **Python & Pandas** (For ETL)
- **Looker Studio** (For Dashboard)
- **GitHub** (Version Control)

## Dashboard Link
[🚀 Click here to view the dashboard](https://lookerstudio.google.com/reporting/df205327-8c5e-4d80-99b7-9ecf848a2ed4)

## Project Images
![Placeholder for ETL Process](/Untitled%20Diagram.drawio%20(1).png)
![Placeholder for Dashboard](/Uber_Dashboard_by_Jugal_Patel%20(2)_page-0001.jpg)
![Placeholder for Data Model used](/data_model.jpeg)

## Setup & Execution
1. Upload data to GCP Bucket Storage.
2. Run and setup Mage and python libraries on your GCP VM instance.
3. Run the following provided code in the respected execution block on the Pipeline, along with configuring the io-config.yaml file with your credentials.
4. Run the ETL Pipeline, after running the pipeline you should be able to see your respected data model tables in BigQuery Studio. 
5. Run the provided SQL script to form a central fact table for the looker studio dashboard.
6. Open the looker studio and connect to you BigQuery Project, and that's it, you did it !
