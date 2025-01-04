# **Scalable Earthquake Data Engineering Pipeline on Azure**

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

## **Setup Instructions**
Follow these steps to set up the project:

1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/your-repo/scalable-earthquake-pipeline.git
   cd scalable-earthquake-pipeline
