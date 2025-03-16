# BI Web Scraping & Visualization Project

This project implements a complete Business Intelligence (BI) pipeline that extracts data from Worldometer through web scraping, stores it in a Microsoft SQL Server database, transforms it using SQL Server Integration Services (SSIS), and finally visualizes it with Power BI.

## Project Architecture

![Project Architecture Diagram](https://github.com/ayoub-anhal/BI_Web-Scraping_Visualisation/blob/main/PLAN/Diagramme%20Web-Scraping.png)

## 🔗 Workflow Overview

1. **Web Scraping (Data Extraction)**
   * Source: Worldometer
   * Tools: `Python`, `Selenium`, `ChromeDriver`
   * Script: `Web_Scraping.ipynb` → This notebook extracts data from Worldometer and automatically stores it into a Microsoft SQL Server database.

2. **Data Storage**
   * Database: **Microsoft SQL Server** → The raw data collected via scraping is saved directly into SQL Server tables.

3. **Data Transformation (ETL Process)**
   * Tool: **SQL Server Integration Services (SSIS)** → The ETL process is handled via SSIS to clean, organize, and prepare the data for reporting.

4. **Data Visualization**
   * Tool: **Power BI** → The transformed data is visualized interactively using Power BI dashboards.

## 🗂️ Technologies Used

* Python + Selenium (for web scraping)
* Microsoft SQL Server (for data storage)
* SSIS (for data transformation)
* Power BI (for reporting)

## 🚀 How to Run the Project

1. Open and run the `Web_Scraping.ipynb` notebook to start scraping and automatically insert data into SQL Server.
2. Execute the SSIS package to transform and clean the data.
3. Open Power BI and connect it to the SQL Server to create your dashboards.

## Dashboard Visualization

![Power BI Dashboard](https://github.com/ayoub-anhal/BI_Web-Scraping_Visualisation/blob/main/PLAN/DAHS_PHOTO.png)

## Prerequisites

* Python 3.x with the following libraries:
  * Selenium
  * Pandas
  * PyODBC or SQL Server driver
* Microsoft SQL Server
* SQL Server Integration Services (SSIS)
* Power BI Desktop

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/ayoub-anhal/BI_Web-Scraping_Visualisation.git
   cd BI_Web-Scraping_Visualisation
   ```

2. Install required Python packages:
   ```bash
   pip install selenium pandas pyodbc
   ```

3. Download and install ChromeDriver compatible with your Chrome browser version.

4. Configure SQL Server connection in the `Web_Scraping.ipynb` notebook.

## Project Structure

```
BI_Web-Scraping_Visualisation/
├── Web_Scraping.ipynb       # Python notebook for web scraping
├── SSIS/                    # SSIS package files
├── PowerBI/                 # Power BI report files
└── PLAN/                    # Documentation and diagrams
    ├── Diagramme Web-Scraping.png
    └── DAHS_PHOTO.png
```

## License

[MIT License](LICENSE)

## Contact

Ayoub Anhal - [GitHub Profile](https://github.com/ayoub-anhal)
