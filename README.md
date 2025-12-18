# 🩺 US County Health Analytics: Public Health Targeting System

## 📋 Executive Summary

**US County Health Analytics** is a comprehensive data-driven framework for identifying, prioritizing, and targeting public health interventions. This system transforms complex health data into actionable intelligence for resource allocation, with direct applicability to global health contexts such as Sub-Saharan Africa.

**Core Impact**: Enables evidence-based targeting of limited health resources to areas of greatest need, maximizing program effectiveness and health outcomes.

---

## 🎯 Key Features

### 📊 **Data Intelligence**
- **796 health indicators** across 3,204 US counties
- **Automated data pipeline** with robust error handling
- **Multi-header CSV processing** for complex datasets
- **Data quality framework** with completeness, consistency, and accuracy checks

### 🔍 **Analytical Frameworks**
- **Health Need Index** - Composite metric (0-100) combining outcomes, access, and social factors
- **County Archetypes** - 4 distinct clusters for tailored interventions
- **Priority Matrix** - 2×2 framework (Access × Poverty) for intervention matching
- **Driver Analysis** - Correlation studies identifying root causes

### 🗺️ **Geographic Targeting**
- **National ranking** of all 3,204 counties by health need
- **State-level analysis** for partnership planning
- **Regional patterns** identification (Northeast, Midwest, South, West)
- **Interactive mapping** with proper red gradient shading

### 📈 **Actionable Outputs**
1. `county_health_priority_ranking.csv` - Complete national ranking
2. `top_100_priority_counties.csv` - Immediate action list
3. `state_level_health_need_summary.csv` - State partnerships guide
4. `us_health_need_map_proper_shading.html` - Interactive stakeholder tool
5. `health_intervention_priority_summary.txt` - Executive briefing

---


---

## 📁 Project Structure

```bash
us-county-health-analytics/
│
├── data/
│   ├── raw/                           # Original CSV files
│   │   └── analytic_data2025_v3.csv   # Main data source
│   ├── processed/                     # Cleaned data
│   │   └── county_health_rankings_2025_cleaned.csv
│   └── backups/                       # Local backups
│
├── notebooks/
│   └── county_health_analysis.ipynb   # Complete analysis notebook
│
├── outputs/
│   ├── rankings/                      # Priority lists
│   │   ├── county_health_priority_ranking.csv
│   │   ├── top_100_priority_counties.csv
│   │   ├── state_level_health_need_summary.csv
│   │   └── regional_health_need_analysis.csv
│   │
│   ├── visualizations/                # Generated charts
│   │   ├── state_health_need.png
│   │   ├── county_archetypes.png
│   │   └── priority_matrix.png
│   │
│   ├── interactive/                   # HTML files
│   │   └── us_health_need_map_proper_shading.html
│   │
│   └── reports/                       # Executive summaries
│       └── health_intervention_priority_summary.txt
│
├── src/                               # Source code modules
│   ├── __init__.py
│   ├── data_loader.py                 # Data loading utilities
│   ├── data_cleaner.py                # Cleaning functions
│   ├── analyzer.py                    # Analytical functions
│   ├── visualizer.py                  # Visualization functions
│   └── reporter.py                    # Reporting functions
│
├── tests/                             # Test suite
│   ├── test_data_loading.py
│   ├── test_analysis.py
│   └── test_visualization.py
│
├── requirements.txt                   # Python dependencies
├── environment.yml                    # Conda environment
├── config.yaml                        # Configuration file
├── Dockerfile                         # Container configuration
├── .gitignore                         # Git ignore rules
├── LICENSE                            # MIT License
└── README.md                          # This file

