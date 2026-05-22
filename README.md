# USDA Biotech Crops Adoption Dashboard — 2025

An interactive data dashboard visualising the adoption of genetically engineered (GE) crop varieties across the United States, based on USDA survey data.

[![Live Dashboard](https://img.shields.io/badge/Dashboard-Live-2E7D32?style=for-the-badge&logo=github)](https://mayodeji25-alt.github.io/usda-biotech-crops-dashboard/)
![Data Year](https://img.shields.io/badge/Data%20Year-2025-1B4332?style=for-the-badge)
![Crops](https://img.shields.io/badge/Crops-Corn%20%7C%20Cotton%20%7C%20Soybean-F57C00?style=for-the-badge)

---

## Overview

This dashboard summarises the adoption of herbicide-tolerant (HT) and insect-resistant (Bt) varieties of **corn**, **upland cotton**, and **soybeans** across major U.S. growing states. Data was collected by USDA's National Agricultural Statistics Service (NASS) in the **June Agricultural Survey 2025** and published in the annual [NASS Acreage report](https://esmis.nal.usda.gov/publication/acreage).

> USDA Economic Research Service does not modify the data published in the annual NASS Acreage report.

---

## Key Findings — 2025

| Crop | All GE Varieties | Dominant Trait |
|------|-----------------|---------------|
| 🌽 Corn | **94%** of planted acres | Stacked (Bt + HT) — 84% |
| 🩵 Upland Cotton | **97%** of planted acres | Stacked (Bt + HT) — 87% |
| 🟢 Soybean | **96%** of planted acres | Herbicide-Tolerant (HT) — 96% |

### Insights

- **Stacked gene varieties dominate corn and cotton**: The vast majority of corn (84%) and cotton (87%) farmers use varieties engineered with both herbicide tolerance *and* insect resistance simultaneously, rather than single-trait seed.
- **Cotton adoption is near-universal in the South**: Alabama, Arkansas, Georgia, Louisiana, Missouri, and Tennessee all reported 99% GE cotton adoption in 2025.
- **Soybeans have reached saturation**: At 96% nationwide, HT soybeans are the most uniformly adopted GE crop. No commercial Bt soybean variety is deployed in the U.S., making HT essentially synonymous with GE for this crop.
- **Corn shows the widest state variation**: Ranging from 88% (Indiana) to 97% (South Dakota), corn has more variance than cotton or soybeans across states.

---

## Dashboard Contents

### `index.html` — Interactive Web Dashboard
A fully self-contained HTML/JavaScript dashboard built with [Chart.js](https://www.chartjs.org/). No server required — open locally or host on GitHub Pages.

**Charts included:**
- KPI summary cards (national adoption rates)
- Doughnut charts — trait composition per crop (Bt only / HT only / Stacked / Non-GE)
- Grouped bar chart — trait-type comparison across all three crops
- Horizontal ranked bar charts — All GE adoption by state for each crop (colour-coded by adoption tier)
- Stacked bar charts — trait breakdown by state for corn and cotton

### `USDA_Biotech_Crops_Dashboard_2025.xlsx` — Excel Workbook
A multi-sheet Excel workbook with:
- Executive dashboard with KPI cards and summary tables
- Per-crop detail sheets (Corn, Cotton, Soybean) with state-level data tables
- Embedded bar and pie charts
- Raw data sheet for full traceability

### `biotech-crops-all-tables-2025.csv` — Source Data
The original USDA NASS dataset (place in repo root if you wish to include it).

---

## Data Definitions

| Term | Definition |
|------|-----------|
| **GE** | Genetically Engineered — crops with DNA altered via biotechnology |
| **HT** | Herbicide-Tolerant — engineered to survive specific herbicide applications |
| **Bt** | Insect-Resistant — carries genes from *Bacillus thuringiensis* bacteria to produce insect-repelling proteins |
| **Stacked** | Varieties combining both HT and Bt traits in a single seed |
| **All GE** | Sum of all GE variety types (Bt only + HT only + Stacked) |

---

## Data Source

- **Primary source**: [USDA NASS Acreage Report 2025](https://esmis.nal.usda.gov/publication/acreage)
- **Survey**: June Agricultural Survey, National Agricultural Statistics Service
- **Publisher**: USDA Economic Research Service (ERS)
- **Coverage**: United States — major corn, cotton, and soybean producing states
- **Years available in original dataset**: 2000–2025

> USDA does not collect or disseminate information about global GE seed use. For global estimates, see the [ISAAA Global Status of Commercialized Biotech/GM Crops](https://www.isaaa.org/) reports.

---

## Repository Structure

```
usda-biotech-crops-dashboard/
├── index.html                              # Interactive web dashboard
├── USDA_Biotech_Crops_Dashboard_2025.xlsx  # Excel workbook
├── biotech-crops-all-tables-2025.csv       # Source data (USDA NASS)
└── README.md                               # This file
```

---

## License

Data is public domain (U.S. Government work — USDA NASS). Dashboard code and visualisation are released under the [MIT License](LICENSE).

---

*Dashboard generated May 2025. Data reflects USDA NASS June Agricultural Survey 2025 results.*
