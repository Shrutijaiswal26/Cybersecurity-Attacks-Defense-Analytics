<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter"/>
  <img src="https://img.shields.io/badge/Machine%20Learning-scikit--learn-green?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="ML"/>
  <img src="https://img.shields.io/badge/XGBoost-Classifier-red?style=for-the-badge&logo=xgboost&logoColor=white" alt="XGBoost"/>
  <img src="https://img.shields.io/badge/Plotly-Interactive-purple?style=for-the-badge&logo=plotly&logoColor=white" alt="Plotly"/>
  <img src="https://img.shields.io/badge/SHAP-Explainability-yellow?style=for-the-badge&logoColor=white" alt="SHAP"/>
  <img src="https://img.shields.io/badge/License-MIT-brightgreen?style=for-the-badge" alt="License"/>
</p>

---

# AI-Powered Cyber Threat Intelligence, Vulnerability Analytics, Malicious Infrastructure Detection, and Machine Learning Security Intelligence Platform

### Comprehensive Analysis of Threat Intelligence Indicators, Vulnerability Intelligence, Malicious Domains, and Malicious IP Infrastructure Using Data Analytics, Cybersecurity Intelligence, and Machine Learning

---

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Notebook Sections](#notebook-sections)
- [Technology Stack](#technology-stack)
- [Visualization Gallery](#visualization-gallery)
- [Machine Learning Pipeline](#machine-learning-pipeline)
- [Key Findings](#key-findings)
- [Use Cases](#use-cases)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Project Overview

This project presents an enterprise-grade Jupyter Notebook designed as a complete **Cyber Threat Intelligence (CTI)**, **Security Analytics**, **Threat Hunting**, **Vulnerability Intelligence**, **Machine Learning**, and **Executive Reporting** platform. The notebook analyzes the [AI Cybersecurity Threat Dataset 2026](https://www.kaggle.com/datasets/chuneeb/ai-cybersecurity-threat-dataset-2026) from Kaggle, providing deep insights into the modern cyber threat landscape.

The analysis pipeline transforms raw cybersecurity data into actionable intelligence through:

- **Threat Intelligence Analysis** -- Decomposition of AlienVault OTX threat pulses, MITRE ATT&CK technique mapping, and malware family classification
- **Vulnerability Intelligence** -- Systematic analysis of CVE/KEV vulnerability records, vendor exposure assessment, and weakness taxonomy mapping
- **Malicious Infrastructure Detection** -- Domain reputation scoring, TLD risk profiling, IP geolocation analysis, and Tor exit node identification
- **Machine Learning Security Models** -- Classification, clustering, and anomaly detection models for automated threat severity prediction
- **Model Explainability** -- SHAP-based interpretability analysis ensuring transparent and auditable ML-driven security decisions
- **Executive Dashboards** -- 30+ interactive and static visualization types delivering intelligence at every organizational level

---

## Dataset Description

The analysis utilizes four complementary cybersecurity datasets sourced from Kaggle:

| Dataset | File | Records | Features | Source |
|---------|------|---------|----------|--------|
| **OTX Threat Intelligence** | `1_otx_threat_intel.csv` | ~2,300+ | 14 | AlienVault OTX |
| **CVE Vulnerabilities** | `2_cve_vulnerabilities.csv` | ~1,500+ | 10 | CISA KEV Catalog |
| **Malicious Domains** | `3_malicious_domains.csv` | ~500+ | 20 | VirusTotal |
| **Malicious IPs** | `4_malicious_ips.csv` | ~700+ | 20 | VirusTotal |

### Dataset Features

**OTX Threat Intelligence**: Pulse ID, Title, Description, Author, Created/Modified timestamps, TLP classification, Tags, Malware Families, MITRE ATT&CK IDs, Targeted Industries, Targeted Countries, Indicator Count, Subscriber Count

**CVE Vulnerabilities**: CVE ID, Vendor/Project, Product, Vulnerability Name, Date Added, Short Description, Required Action, Due Date, Ransomware Campaign Association, CWE Weakness Types

**Malicious Domains**: Domain name, TLD, Domain Length, Character Analysis, Registrar, WHOIS dates, Reputation Score, Community Votes (Malicious/Suspicious/Harmless/Undetected), Threat Severity, Categories, Popularity Rank, Analysis metadata

**Malicious IPs**: IP address, Country, Continent, ASN, Network Owner, CIDR Block, Community Votes, Reputation Score, Threat Label/Category, Regional Registry, Tor Node status, Threat Severity

---

## Project Structure

```
.
|-- cybersecurity_threat_intelligence.ipynb   # Main analysis notebook (30 sections)
|-- 1_otx_threat_intel.csv                    # OTX threat intelligence data
|-- 2_cve_vulnerabilities.csv                 # CVE vulnerability records
|-- 3_malicious_domains.csv                   # Malicious domain intelligence
|-- 4_malicious_ips.csv                       # Malicious IP infrastructure data
|-- generate_notebook.py                      # Notebook generator script
|-- README.md                                 # Project documentation
```

---

## Installation

### Prerequisites

- Python 3.10 or higher
- Jupyter Notebook or JupyterLab

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/ai-cybersecurity-threat-intelligence.git
cd ai-cybersecurity-threat-intelligence
```

2. **Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn xgboost lightgbm catboost shap networkx kaleido
```

3. **Download the dataset**

Download the dataset from [Kaggle](https://www.kaggle.com/datasets/chuneeb/ai-cybersecurity-threat-dataset-2026) and place all four CSV files in the project root directory.

4. **Launch the notebook**
```bash
jupyter notebook cybersecurity_threat_intelligence.ipynb
```

---

## Usage

Open the notebook and execute cells sequentially. The notebook is designed to run end-to-end with no manual intervention required. All dependencies are installed automatically in the first cell.

```bash
# Quick start
jupyter notebook cybersecurity_threat_intelligence.ipynb
```

For JupyterLab users:
```bash
jupyter lab cybersecurity_threat_intelligence.ipynb
```

---

## Notebook Sections

The notebook contains exactly **30 structured sections**, organized into six analytical phases:

### Phase 1: Foundation and Data Engineering (Sections 1-7)

| Section | Title | Description |
|---------|-------|-------------|
| 1 | Executive Project Overview | Project architecture, security objectives, intelligence objectives, ML objectives |
| 2 | Cyber Threat Intelligence Foundations | CTI concepts, IOC analysis, TTPs, MITRE ATT&CK, threat hunting methodology |
| 3 | Dataset Understanding | Schema analysis, feature inventory, sample records for all four datasets |
| 4 | Data Ingestion Pipeline | Secure ingestion workflow, schema validation, initial profiling |
| 5 | Data Dictionary | Comprehensive feature dictionary with security relevance and intelligence value |
| 6 | Data Quality Assessment | Missing value analysis, duplicate detection, quality scoring |
| 7 | Data Cleaning and Preparation | Null treatment, standardization, type conversion, deduplication |

### Phase 2: Exploratory Intelligence (Sections 8-12)

| Section | Title | Description |
|---------|-------|-------------|
| 8 | Global Exploratory Data Analysis | Summary KPIs, distribution overview, high-level intelligence metrics |
| 9 | OTX Threat Intelligence Analysis | Malware families, ATT&CK techniques, targeted industries and countries |
| 10 | Vulnerability Intelligence Analysis | Vendor/product exposure, CWE taxonomy, ransomware associations, timelines |
| 11 | Malicious Domain Intelligence Analysis | TLD profiling, reputation analysis, registrar patterns, domain age |
| 12 | Malicious IP Intelligence Analysis | Geographic distribution, Tor analysis, ASN/ISP profiling, reputation |

### Phase 3: Statistical Analysis (Sections 13-16)

| Section | Title | Description |
|---------|-------|-------------|
| 13 | Univariate Analysis | Histograms, KDE plots, frequency analysis, density distributions |
| 14 | Bivariate Analysis | Scatter plots, group comparisons, cross-feature analysis |
| 15 | Multivariate Analysis | Pairplots, correlation matrices, feature interaction maps |
| 16 | Statistical Analysis | Distribution testing, chi-square tests, ANOVA, trend analysis |

### Phase 4: Risk and Threat Analytics (Sections 17-19)

| Section | Title | Description |
|---------|-------|-------------|
| 17 | Cyber Risk Analytics | Composite risk scoring, risk heatmaps, risk matrices |
| 18 | Threat Landscape Analysis | Emerging threats, critical indicators, threat concentration |
| 19 | Anomaly Detection Analysis | Isolation Forest, LOF, statistical anomaly detection |

### Phase 5: Machine Learning (Sections 20-27)

| Section | Title | Description |
|---------|-------|-------------|
| 20 | Feature Engineering | Threat density metrics, composite scores, ML-ready datasets |
| 21 | Feature Importance Analysis | Random Forest importance, Mutual Information, Permutation Importance |
| 22 | Machine Learning Pipeline | Preprocessing pipeline, training architecture, validation framework |
| 23 | Classification Models | Logistic Regression, Random Forest, XGBoost, LightGBM, CatBoost |
| 24 | Clustering Analysis | K-Means, DBSCAN, Hierarchical Clustering with cluster profiling |
| 25 | Anomaly Detection Models | Isolation Forest, One-Class SVM, LOF with agreement analysis |
| 26 | Model Evaluation | Confusion matrices, ROC/AUC, Precision-Recall curves, performance dashboard |
| 27 | Model Explainability | SHAP summary, dependence plots, waterfall plots, feature contributions |

### Phase 6: Intelligence and Reporting (Sections 28-30)

| Section | Title | Description |
|---------|-------|-------------|
| 28 | Cybersecurity Intelligence Findings | Key indicators, critical vulnerabilities, SOC and hunting implications |
| 29 | Executive Recommendations | Strategic, operational, technical, detection, and hunting recommendations |
| 30 | Enterprise CTI Dashboard | Complete dashboard with 30+ visualization types and KPI cards |

---

## Technology Stack

### Core Libraries

| Library | Version | Purpose |
|---------|---------|---------|
| `pandas` | 2.x | Data manipulation and analysis |
| `numpy` | 1.x | Numerical computing |
| `matplotlib` | 3.x | Static visualizations and dashboards |
| `seaborn` | 0.13+ | Statistical data visualization |
| `plotly` | 5.x | Interactive visualizations, maps, Sankey diagrams |

### Machine Learning

| Library | Purpose |
|---------|---------|
| `scikit-learn` | Classification, clustering, anomaly detection, preprocessing |
| `xgboost` | Gradient boosting classification |
| `lightgbm` | Light gradient boosting classification |
| `catboost` | Categorical gradient boosting classification |
| `shap` | Model explainability and interpretability |

### Supporting Libraries

| Library | Purpose |
|---------|---------|
| `networkx` | Network graph analysis and visualization |
| `scipy` | Statistical testing (Shapiro-Wilk, Chi-square, Kruskal-Wallis) |
| `kaleido` | Static image export for Plotly charts |

---

## Visualization Gallery

The notebook produces **30+ distinct visualization types** across all sections:

### Statistical Visualizations
- Line Charts, Area Charts, Spline Charts
- Histograms, KDE Plots, Box Plots, Violin Plots
- Strip Plots, Swarm Plots
- Scatter Plots, Bubble Charts

### Comparative Visualizations
- Bar Charts (standard, grouped, stacked, horizontal)
- Pairplots, Correlation Matrices, Pivot Heatmaps

### Hierarchical and Relational
- Treemaps, Sunburst Charts
- Sankey Diagrams, Network Graphs

### Distribution and Composition
- Donut Charts, Pie Charts
- Waterfall Charts, Funnel Charts
- Radar Charts, Polar Charts

### Geospatial and Specialized
- Geographic Choropleth Maps
- Cluster Maps, Risk Matrices
- Timeline Analysis with Range Sliders

### Machine Learning Visualizations
- Confusion Matrices, ROC Curves, Precision-Recall Curves
- SHAP Summary, Dependence, and Waterfall Plots
- Feature Importance Rankings, Elbow Method Plots
- Cluster Scatter Plots (PCA-reduced)

---

## Machine Learning Pipeline

### Classification Task
**Objective**: Predict threat severity (Low/Medium/High) for malicious entities (domains and IPs)

**Models Trained**:
1. Logistic Regression (baseline)
2. Random Forest (ensemble)
3. XGBoost (gradient boosting)
4. LightGBM (light gradient boosting)
5. CatBoost (categorical boosting)

**Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, ROC AUC, Precision-Recall AUC

### Clustering Task
**Objective**: Identify natural groupings in threat infrastructure

**Algorithms**: K-Means, DBSCAN, Agglomerative (Hierarchical) Clustering

### Anomaly Detection
**Objective**: Detect outlier threat entities requiring urgent investigation

**Models**: Isolation Forest, One-Class SVM, Local Outlier Factor (LOF)

### Explainability
**Framework**: SHAP (SHapley Additive exPlanations) for transparent, auditable ML decisions

---

## Key Findings

The analysis reveals critical insights across the cyber threat landscape:

- **Threat Intelligence**: Identification of prevalent malware families, most-targeted industries, and dominant MITRE ATT&CK techniques used by threat actors
- **Vulnerability Landscape**: Vendor exposure analysis highlighting the most affected software products and common weakness types (CWEs)
- **Domain Intelligence**: TLD risk profiling, domain age patterns, and registrar associations with malicious infrastructure
- **IP Infrastructure**: Geographic concentration of malicious IPs, Tor exit node behavior patterns, and ISP/hosting provider risk profiles
- **ML Performance**: Ensemble models (Random Forest, XGBoost, LightGBM) achieve strong classification performance for threat severity prediction
- **Anomaly Detection**: Multi-method anomaly detection identifies high-priority entities for SOC investigation

---

## Use Cases

This notebook is designed for professionals and researchers across multiple domains:

| Audience | Application |
|----------|-------------|
| **Cybersecurity Portfolio** | Demonstrate end-to-end CTI and ML capabilities |
| **Academic Research** | Reference implementation for cybersecurity data science |
| **Threat Intelligence** | Operational IOC analysis and threat landscape reporting |
| **SOC Analytics** | Detection engineering insights and alert prioritization |
| **Security Operations** | Vulnerability management and risk assessment |
| **Security Engineering** | Infrastructure hardening and defensive architecture |
| **Machine Learning Showcase** | Multi-model comparison with explainability |
| **Executive Reporting** | Board-level dashboards and strategic recommendations |

---

## Contributing

Contributions are welcome. Please follow these guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/enhancement`)
3. Commit your changes (`git commit -m 'Add enhancement'`)
4. Push to the branch (`git push origin feature/enhancement`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- **Dataset**: [AI Cybersecurity Threat Dataset 2026](https://www.kaggle.com/datasets/chuneeb/ai-cybersecurity-threat-dataset-2026) by Chuneeb on Kaggle
- **Data Sources**: AlienVault OTX, CISA KEV Catalog, VirusTotal
- **Frameworks**: MITRE ATT&CK, CVSS, CWE

---

<p align="center">
  <strong>Built for cybersecurity professionals, by cybersecurity professionals.</strong>
</p>
