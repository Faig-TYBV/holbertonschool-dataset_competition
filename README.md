# Azerbaijan Transport Sector Analysis (1995-2024)

### IDDA Open Data Project

## 📌 Project Overview

This project provides a comprehensive analysis of the transport sector in Azerbaijan over the last three decades. Using open data provided by the **IDDA (Innovation and Digital Development Agency)**, this study explores the economic evolution of different transport modes, identifies structural shifts in the industry, and corrects critical data inconsistencies found in the raw source.

## 🛠 Tools Used

* **Python** (Data Processing)
* **Pandas** (Data Auditing & Cleaning)
* **Plotly** (Interactive Visualizations)
* **Seaborn/Matplotlib** (Statistical Aesthetic Visuals)

## 🔍 Data Quality Audit & Cleaning

One of the most valuable aspects of this project was the **Data Integrity Phase**. During the analysis, several inconsistencies were identified and corrected to ensure accuracy:

1. **Unit Correction:** The `Railway` column was labeled in millions (*mln.manat*) while the rest of the data was in thousands (*min manat*). Cross-referencing with the `Total` column revealed this was a typographical error in the source; all units were standardized to Thousands.
2. **Hierarchy Management:** The dataset includes a hierarchical structure where `Pipeline` is the sum of `Oil` and `Gas`. To avoid **double-counting** and **triple-counting** (adding the total to its own components), a custom calculation logic was applied to extract the "True Total."
3. **Language:** All categories were translated from Azerbaijani to English for international accessibility.

## 💡 Key Insights

* **The Rise of Aviation:** Since 2015, the aviation sector has experienced exponential growth, surpassing traditional sectors like Railways and Pipelines. As of 2024, Air Transport accounts for **over 50%** of the sector's total recorded value.
* **Sector Diversification:** While the early 2000s were dominated by resource-based Pipeline transport, the current trend shows a more diversified logistics economy with a significant increase in Automobile and Air cargo.

## 📊 Visualizations

* **Evolution Area Chart:** An interactive visualization showing the "mountain" of growth from 1995 to 2024.
* **Market Share Analysis:** A breakdown of how each transport mode's importance has shifted over time.

## 🚀 How to View

1. Open the `Analysis.ipynb` to see the code and logic.
2. Open the `Analysis.html` for the interactive version of the charts (best for viewing).

---

*Developed for the IDDA Open Data Competition.*
