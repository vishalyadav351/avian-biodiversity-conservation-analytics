# 🦅 Avian Diversity & Habitat Dynamics Analysis
**End-to-End Data Pipeline, Relational Modeling & Interactive Power BI Dashboard**

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-3.x-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-Desktop-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📌 Executive Summary
This project analyzes multi-year avian monitoring datasets across 11 National Park units, covering both Forest and Grassland habitats. The objective is to consolidate disparate monitoring records, evaluate environmental impacts (temperature, humidity, weather conditions) on bird activity, and identify critical conservation priority zones for at-risk species.

---

## 📊 Core Analytical Highlights

| Dimension | Metric / Finding | Strategic Impact |
| :--- | :--- | :--- |
| **Total Observations** | **17,077 Sightings** | Harmonized across 21 raw Excel catalog sheets |
| **Species Diversity** | **127 Unique Species** | Comprehensive avian biodiversity record |
| **Habitat Balance** | **8,546 Forest \| 8,531 Grassland** | Balanced ~50/50 ecological distribution |
| **PIF Watchlist Species** | **378 Sightings across 8 Species** | Identified vulnerable populations (e.g., *Wood Thrush*) |
| **Regional Stewardship** | **3,985 Sightings** | Priority species requiring habitat preservation |
| **Detection Method** | **~81.5% Acoustic Detection** | Identified primarily through Singing & Calling |
| **Mean Environment** | **22.57°C Temp \| 73.69% Humidity** | Optimal baseline window for field observation |

---

## 🛠️ Tech Stack & Architecture

```text
[ Raw Excel Sheets (21) ] ──> [ Python / Pandas ETL ] ──> [ Cleaned_Bird_Data.csv ]
                                                                 │
                                                                 ├──> [ SQLite Database (bird_database.db) ]
                                                                 └──> [ Power BI Dashboard (4 Pages) ]
Data Engineering & Cleaning: Python (pandas, numpy, openpyxl)  Database Architecture: SQLite (sqlite3), SQL queries & schema validation  Visualization & Analytics: Microsoft Power BI Desktop, DAX, Custom Dark Glass UI Theme  📑 Power BI Dashboard Structure (4 Pages)Page 1: Overview & DiversityHigh-level KPI metrics (Total Sightings, Unique Species, Habitat breakdown).  Top 10 Sighted Bird Species & Park-wise distribution share.  Longitudinal annual observation trends by habitat type.  Page 2: Habitat & EnvironmentDetection method breakdown (Singing, Calling, Visual).  Temperature vs. Sighting volume curve & Sky condition distribution.  Distance-from-observer patterns across Forest vs. Grassland[cite: 3].Page 3: Conservation & Watchlist InsightsPriority at-risk species tracking (Wood Thrush, Prairie Warbler, Worm-eating Warbler)[cite: 3].National Park conservation hotspots (PRWI, CATO, CHOH)[cite: 3].Interactive raw inspection data grid with dynamic cross-filtering[cite: 3].Page 4: Project Overview & MetadataExecutive project brief, author metadata, and architectural workflow[cite: 3].📁 Repository StructurePlaintext├── data/
│   ├── Cleaned_Bird_Data.csv          # Master harmonized dataset
│   └── bird_database.db               # Relational SQLite database
├── scripts/
│   ├── clean_data.py                  # Automated multi-sheet ingestion & ETL script
│   ├── save_to_sql.py                 # SQLite export & schema validation script
│   └── eda_analysis.py                # Exploratory statistical analysis script
├── dashboard/
│   ├── Bird_Observation_Analysis.pbix  # Interactive 4-Page Power BI report
│   └── theme.json                     # Apex Wildlife Dark Glass custom theme
├── docs/
│   └── Bird_Observation_Analysis_Report.pdf  # Comprehensive Analytical Project Report
└── README.md
🚀 How to Run Locally1. Clone the RepositoryBashgit clone [https://github.com/](https://github.com/)<your-username>/avian-biodiversity-conservation-analytics.git
cd avian-biodiversity-conservation-analytics
2. Run the Data PipelineBash# Clean & merge raw datasets
python scripts/clean_data.py

# Export to SQLite database
python scripts/save_to_sql.py
3. Open the DashboardLaunch Microsoft Power BI Desktop.Open dashboard/Bird_Observation_Analysis.pbix[cite: 3].💡 Key Strategic RecommendationsPrioritize Acoustic Survey Windows: Over 80% of bird detections occur via vocalizations; surveys conducted during high wind or environmental disturbance suffer significant yield drops[cite: 3].Target High-Priority Hotspots: Conservation funding and forest fragmentation mitigation should target Prince William Forest Park (PRWI) and Catoctin Mountain Park (CATO) due to dense Watchlist species populations[cite: 3].👤 AuthorDeveloper: Vishal YadavDomain: Conservation Informatics & Data Analytics[cite: 3]
---

