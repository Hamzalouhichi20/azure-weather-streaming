
# 🌦️ Real-Time Weather Report System using Weather API & Microsoft Azure

## 📌 Project Description
This project implements a real-time weather data pipeline using a public weather API and Microsoft Azure services. It demonstrates how to automate data ingestion, processing, and visualization using Azure Databricks, Azure Functions, Event Hub, and Microsoft Fabric (Eventhouse + Power BI).

---

## 🚀 Steps Completed

### 1. 🏗️ Resource Setup
- Created a **Resource Group** in Azure
- Deployed services: Event Hub, Databricks, Key Vault, Function App, Storage Account, Fabric Capacity

### 2. ⚙️ Data Ingestion
- Used **Azure Function App (Timer Trigger)** to pull data from the **Weather API**
- Sent structured JSON events into **Azure Event Hub**

### 3. 🧼 Data Processing
- Set up a **Databricks Cluster**
- Created a **notebook** to:
  - Parse and flatten API data
  - Send events to Event Hub
- Secured credentials via **Key Vault + Secret Scope**

### 4. 🔐 Security
- Used **RBAC** and **Managed Identity** for Function App access to Key Vault
- Created and linked **secrets** (API keys, connection strings)

### 5. 🔁 Eventstream & Fabric Integration
- Created a **Real-Time Eventstream Pipeline** in Fabric
- Routed data to an **Eventhouse (KQL DB)**
- Connected to **Power BI** for visualization

### 6. 📊 Dashboard
- Built a **Power BI dashboard** from the Eventhouse in Fabric

---
### Azure Resources
![Screenshot 2025-06-16 141245](https://github.com/user-attachments/assets/fc6fd986-f5b0-4609-adc3-4dce889ee48f)

### Weather Data Preview
![Screenshot 2025-06-14 222424](https://github.com/user-attachments/assets/0974f5cb-3092-405e-b413-97e138462518)

### Eventstream Pipeline
![Screenshot 2025-06-14 222007](https://github.com/user-attachments/assets/783fb7a7-30d6-4b83-a604-b669f94e6484)

---

## 🛠️ Tech Stack

- **Azure Event Hub**
- **Azure Functions**
- **Azure Databricks**
- **Azure Key Vault**
- **Microsoft Fabric**
- **Power BI**
- **Python**, **Spark**, **KQL**, **JSON**

