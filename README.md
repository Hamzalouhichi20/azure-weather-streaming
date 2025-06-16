
# 🌦️ Real-Time Weather Report System using Weather API & Microsoft Azure

## 📌 Project Description
This project implements a real-time weather data pipeline using a public weather API and Microsoft Azure services. It demonstrates how to automate data ingestion, processing, and visualization using Azure Databricks, Azure Functions, Event Hub, and Microsoft Fabric (Eventhouse + Power BI).

---

## 🧩 Architecture Overview
![Untitled Diagram drawio (1)](https://github.com/user-attachments/assets/abba4505-862b-491d-829c-2ce8561323f6)

### 📊 Visual Diagram

```
Weather API
   ↓ (Azure Function or Databricks trigger)
Azure Event Hub
   ↓
Databricks (processes and cleans data)
   ↓
Microsoft Fabric (Eventstream → Eventhouse)
   ↓
Power BI Dashboard
```

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

## 📸 Screenshots

### Azure Resources
![Azure Resources](Screenshot%202025-06-16%20141245.png)

### Weather Data Preview
![Weather Data Preview](Screenshot%202025-06-14%20222424.png)

### Eventstream Pipeline
![Event Stream Pipeline](Screenshot%202025-06-14%20222007.png)

---

## 🛠️ Tech Stack

- **Azure Event Hub**
- **Azure Functions**
- **Azure Databricks**
- **Azure Key Vault**
- **Microsoft Fabric**
- **Power BI**
- **Python**, **Spark**, **KQL**, **JSON**

---

## 📅 Status
✅ Project completed and working in real-time with scheduled API calls, streaming data, and Power BI dashboard.
