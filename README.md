# **Building a Scalable and Real-Time Earthquake Data Engineering Pipeline on Azure**

## **Project Overview**
This project focuses on designing and implementing a comprehensive data engineering pipeline to process and analyze real-time earthquake data. By leveraging Azure’s robust cloud services, the solution provides meaningful insights into global seismic activity through an interactive Power BI dashboard.

The pipeline automates data ingestion, transformation, and visualization, enabling stakeholders to access up-to-date, actionable insights for decision-making, research, and emergency planning.

---

## **Business Requirement**
The project was initiated to address the need for real-time insights into global seismic activity. Stakeholders required a system that could:

- Continuously ingest and process real-time earthquake data from external APIs.
- Provide meaningful insights into trends such as earthquake frequency, intensity, and geographic distribution.
- Deliver data in a user-friendly, visually engaging dashboard that could be easily updated and shared.

This solution bridges the gap in real-time earthquake monitoring, helping stakeholders better understand and respond to seismic activities.

---

## **Solution Overview**
To meet the business requirements, the following solution was implemented:

1. **Data Ingestion**: Automated collection of earthquake data from APIs using Azure Data Factory.
2. **Data Transformation**: Scalable transformations with Azure Databricks (PySpark) to ensure data is clean, structured, and ready for analysis.
3. **Data Storage**: Centralized storage in Azure Data Lake and Azure Synapse Analytics for high-performance querying.
4. **Visualization**: Development of a Power BI dashboard to visualize key metrics, including earthquake intensity, frequency, and location trends.
5. **Automation**: Scheduled daily updates to ensure stakeholders always have access to the latest data.

---

## **Technology Stack**
The project uses the following technologies:

- **Data Ingestion**: Azure Data Factory
- **Data Transformation**: Azure Databricks (PySpark)
- **Data Storage**: Azure Data Lake, Azure Synapse Analytics
- **Visualization**: Power BI
- **Cloud Platform**: Microsoft Azure
- **Development Tools**: Python, PySpark, Power BI Desktop

---

## Setup Instructions

### Prerequisites

- An Azure account with sufficient credits.
- Access to real-time earthquake data via an external API.

---

### Step 1: Azure Environment Setup

1. **Create Resource Group**: Set up a new resource group in Azure.
2. **Provision Services**:
   - Create an Azure Data Factory instance for data ingestion.
   - Set up Azure Data Lake Storage with `raw`, `processed`, and `curated` containers.
   - Create an Azure Databricks workspace for data transformation.
   - Set up an Azure Synapse Analytics workspace for querying and reporting.
   - Configure Azure Key Vault for secure management of API keys and connection strings.

---

### Step 2: Data Ingestion

1. **API Integration**: Obtain API access credentials for the earthquake data provider.
2. **Set up Data Factory Pipelines**:
   - Create pipelines to ingest real-time data from the API and store it in the `raw` container in ADLS.

---

### Step 3: Data Transformation

1. **Mount Data Lake in Databricks**:
   - Configure Databricks to access ADLS containers.
2. **Transform Data**:
   - Use Databricks notebooks to clean, enrich, and aggregate the data, moving it from `raw` to `processed` and then to `curated`.

---

### Step 4: Data Loading and Reporting

1. **Load Data into Synapse**:
   - Set up a Synapse SQL pool and load the curated data for analysis and visualization.
2. **Create Power BI Dashboard**:
   - Connect Power BI to Synapse Analytics.
   - Develop visualizations showcasing earthquake trends such as frequency, intensity, and geographic distribution.

---

### Step 5: Automation and Monitoring

1. **Schedule Pipelines**:
   - Use Azure Data Factory to schedule the ingestion and transformation pipelines to run daily.
2. **Monitor Pipeline Runs**:
   - Use ADF and Synapse monitoring tools to track pipeline execution and resolve issues.

---

### Step 6: Security and Governance

1. **Manage Access**:
   - Set up role-based access control (RBAC) using Azure Entra ID (formerly Azure Active Directory).
   - Ensure sensitive data is encrypted and securely managed.

---

### Step 7: End-to-End Testing

1. **Trigger and Test Pipelines**:
   - Simulate API data ingestion and verify the end-to-end pipeline functionality.
   - Ensure the Power BI dashboard reflects accurate and updated information.

