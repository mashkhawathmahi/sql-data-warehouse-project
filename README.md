# Data Warehouse and Analytics Project

An end-to-end data warehousing and analytics solution built with SQL Server, covering everything from raw data ingestion to business-ready reporting. This is my own implementation of the project, built as a portfolio piece to demonstrate data engineering and analytics skills.

> **Credit:** This project is based on the open-source *SQL Data Warehouse Project* by [Baraa Khatib Salkini (Data With Baraa)](https://github.com/DataWithBaraa/sql-data-warehouse-project), released under the MIT License. The architecture and dataset follow the original tutorial; the implementation, documentation, and extensions in this repository are my own.

---

## 🏗️ Data Architecture

The warehouse follows the **Medallion Architecture** with Bronze, Silver, and Gold layers:

![Data Architecture](docs/data_architecture.png)

1. **Bronze Layer**: Raw data stored as-is from the source systems. Ingested from CSV files into SQL Server.
2. **Silver Layer**: Data cleansing, standardization, and normalization to prepare data for analysis.
3. **Gold Layer**: Business-ready data modeled as a star schema for reporting and analytics.

---

## 📖 Project Overview

1. **Data Architecture**: Designing a modern data warehouse using the Medallion Architecture.
2. **ETL Pipelines**: Extracting, transforming, and loading data from the ERP and CRM source systems.
3. **Data Modeling**: Building fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: SQL-based reports delivering insights on customer behavior, product performance, and sales trends.

**Skills demonstrated:** SQL Development · Data Architecture · Data Engineering · ETL Development · Data Modeling · Data Analytics

---

## 🛠️ Tools & Technologies

- **SQL Server Express**: database engine
- **SQL Server Management Studio (SSMS)**: database management and querying
- **Git & GitHub**: version control
- **Draw.io**: architecture, data flow, and data model diagrams
- **Notion**: project planning
- **Datasets**: ERP and CRM CSV files in [`datasets/`](datasets/)

---

## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

**Objective:** Build a modern data warehouse in SQL Server that consolidates sales data to support analytical reporting and decision-making.

- **Data Sources**: Two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Identify and resolve data quality issues before analysis.
- **Integration**: Combine both sources into a single, analytics-friendly data model.
- **Scope**: Latest dataset only; no historization required.
- **Documentation**: Clear documentation of the data model for business and analytics stakeholders.

### Analytics & Reporting (Data Analysis)

**Objective:** Develop SQL-based analytics covering:

- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

See [docs/requirements.md](docs/requirements.md) for details.

---

## 📂 Repository Structure

```
data-warehouse-project/
│
├── datasets/                     # Raw ERP and CRM CSV files
│
├── docs/                         # Documentation and diagrams
│   ├── etl.drawio                # ETL techniques and methods
│   ├── data_architecture.drawio  # Overall architecture
│   ├── data_flow.drawio          # Data flow diagram
│   ├── data_models.drawio        # Star schema data model
│   ├── data_catalog.md           # Field descriptions and metadata
│   └── naming-conventions.md     # Naming guidelines
│
├── scripts/                      # SQL scripts
│   ├── bronze/                   # Raw data extraction and loading
│   ├── silver/                   # Cleansing and transformation
│   └── gold/                     # Analytical models (star schema)
│
├── tests/                        # Data quality checks and test scripts
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## ▶️ How to Run

1. Install SQL Server Express and SSMS.
2. Clone this repository and place the CSV files in `datasets/`.
3. Run the scripts in order:
   1. `scripts/bronze/` to create the database, schemas, and raw tables, then load the CSVs
   2. `scripts/silver/` to clean and standardize the data
   3. `scripts/gold/` to create the star-schema views
4. Run the checks in `tests/` to validate data quality.
5. Run the analytics queries to generate reports.

> Update the file paths in the bronze load scripts to match where the CSVs live on your machine.

---

## 💡 Key Insights & Findings

_Add 3–5 headline findings from your analysis here (e.g. top-performing product categories, customer segments, sales trends)._

---

## 🔧 What I Added / Changed

_List anything that makes this version yours: extra data quality checks, additional reports, different naming choices, performance improvements, dashboards, etc._

---

## 🛡️ License

This project is licensed under the [MIT License](LICENSE). The original work by Baraa Khatib Salkini is also MIT licensed; please keep the attribution above.

---

## 🌟 About Me

Hi, I'm **Mahi**, a data analyst with a BBA in Business and Technology Management from the Islamic University of Technology (IUT), Bangladesh. I work with operational analytics, funnel management, and data-driven decision-making in the financial services space.

- LinkedIn: _add your link_
- GitHub: _add your link_
- Email: _add your email_
