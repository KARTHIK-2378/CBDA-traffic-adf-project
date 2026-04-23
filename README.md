#  Traffic Data ETL Pipeline using Azure Data Factory

##  Project Overview

This project demonstrates an end-to-end **ETL (Extract, Transform, Load)** pipeline using **Azure Data Factory**. Traffic data in CSV format is ingested from Azure Blob Storage, processed, and used for analytics and visualization.

---

##  Architecture

```
CSV File
   ↓
Azure Blob Storage (raw)
   ↓
Azure Data Factory (Copy Data Pipeline)
   ↓
Azure Blob Storage (processed)
   ↓
Power BI Dashboard
```

---

##  Technologies Used

* Azure Data Factory (ADF)
* Azure Blob Storage
* Power BI
* CSV Data Source

---

##  Resource Setup

* Resource Group: `traffic-etl-rg`
* Data Factory: `traffic-adf`
* Storage Account: `trafficdatalake`

---

##  Pipeline Details

* Pipeline Name: `PL_Traffic_ETL`
* Activity Used: **Copy Data**
* Source Dataset: `DS_TrafficCSV`
* Sink Dataset: `DS_TrafficProcessed`

---

##  Data Flow

* **Input Folder:** `raw/`
* **Output Folder:** `processed/`

Example:

```
raw/traffic_data.csv → processed/traffic_processed.csv
```

---

##  Power BI Dashboard

The processed data is visualized using Power BI:

* Vehicle count by year
* Junction-wise analysis
* Traffic trends over time

---

##  How to Run the Project

### Step 1: Upload Data

Upload CSV file to:

```
Blob Storage → raw folder
```

### Step 2: Create Dataset

* Create dataset for CSV in ADF
* Link it to Blob Storage

### Step 3: Run Pipeline

```
Author → Pipelines → PL_Traffic_ETL → Debug/Trigger
```

### Step 4: Verify Output

Check:

```
Blob Storage → processed folder
```

### Step 5: Visualize

Load processed data into Power BI and build visuals.

---

##  Screenshots

(Add your screenshots here)

* Azure Data Factory Pipeline
* Blob Storage (raw & processed)
* Power BI Dashboard

---

##  Key Learnings

* Building ETL pipelines in Azure Data Factory
* Working with Blob Storage datasets
* Data transformation using Copy Activity
* Integrating ADF output with Power BI

---

##  Future Enhancements

* Add Data Flow transformations
* Connect to Azure SQL Database
* Automate pipeline using triggers

---

##  Screenshots
<img width="1919" height="871" alt="Screenshot 2026-04-23 110839" src="https://github.com/user-attachments/assets/c28df63e-3215-4f43-b443-c89d9622e4f3" />
<img width="1914" height="888" alt="Screenshot 2026-04-23 110853" src="https://github.com/user-attachments/assets/8873d040-d594-4f76-993f-f54130ff7216" />
<img width="1914" height="883" alt="Screenshot 2026-04-23 110953" src="https://github.com/user-attachments/assets/8af68bee-a46e-4e55-9d97-a7e8b07bb9c4" />
<img width="1919" height="967" alt="Screenshot 2026-04-23 111053" src="https://github.com/user-attachments/assets/2bf247b0-d60b-490b-aea6-d27c603a1d66" />
<img width="1919" height="769" alt="Screenshot 2026-04-23 111143" src="https://github.com/user-attachments/assets/3396f4f8-8f17-4155-b2fb-20251a7b5762" />




