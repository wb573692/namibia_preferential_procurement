# Namibia Procurement Reform — Reproducibility Package
[![Python 3.9+](https://img.shields.io/badge/python-3.9%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/notebook-Jupyter%20%7C%20Colab-orange.svg)](https://colab.research.google.com/)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Status: Working Draft](https://img.shields.io/badge/status-working%20draft-yellow.svg)]()


---

## Repository Structure

```
namibia_preferential_procurement/
│
├── notebooks/
│   └── preferential_procurement_policy_namibia.ipynb
│
├── data/                                           ← Not included - see Data Access and Download Instructions
│   ├── Namibia2006_manufacturing_clean.dta
│   ├── Namibia2006_residual_clean.dta
│   ├── Namibia2006_retail_and_it_clean.dta
│   ├── Namibia-2014-full-data.dta
│   └── Namibia-2024-full-data.dta
│
├── outputs/
│
├── paper/
│   └── preferential_procurement_policy_namibia.docx
│
└── README.md
```

---

## Data Access and Download Instructions

The World Bank Enterprise Survey microdata are **not included** in this repository due to the World Bank's data use terms. They must be downloaded directly from the WBES portal.

1. Go to [enterprisesurveys.org](https://www.enterprisesurveys.org/en/data)
2. Search for **Namibia** and download the following waves<br>
   2006: `Namibia2006_manufacturing_clean.dta` · `Namibia2006_residual_clean.dta` · `Namibia2006_retail_and_it_clean.dta`<br>
   2014: `Namibia-2014-full-data.dta`<br>
   2024: `Namibia-2024-full-data.dta`<br>
3. Place all five `.dta` files in the `data/` directory.

---

## Dependencies

```
python >= 3.9
pandas >= 1.5
numpy >= 1.23
pyreadstat >= 1.2       # reads .dta Stata files
statsmodels >= 0.14     # OLS, Probit, marginal effects
matplotlib >= 3.6       # event-study plot
jupyter >= 1.0          # notebook runtime
```

---

## License

Code in this repository is released under the [MIT License](LICENSE).  
The World Bank Enterprise Survey data are subject to the [World Bank's own terms of use](https://www.enterprisesurveys.org/en/methodology) and are not redistributed here.
