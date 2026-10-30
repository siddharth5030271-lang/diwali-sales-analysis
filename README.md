# Diwali Sales Analysis

Exploratory data analysis (EDA) of Diwali sales records using Python to investigate customer demographics, geographic patterns, occupations, and product-category performance.

## Project objective

Identify descriptive patterns in recorded sales and order data that could help a business decide where to investigate customer segments and product performance further.

## Tools

* Python
* Pandas and NumPy
* Matplotlib and Seaborn
* Jupyter Notebook

## Repository structure

```text
diwali-sales-analysis/
├── data/
│   └── diwali\_sales\_data.csv
├── images/
│   └── key\_findings.png
├── notebooks/
│   └── Diwali\_Sales\_Analysis.ipynb
├── .gitignore
├── README.md
└── requirements.txt
```

## How to run

1. Install Python 3.10 or newer.
2. Clone or download this repository.
3. Open a terminal in the repository folder.
4. Create and activate a virtual environment (recommended).
5. Install the dependencies:

```bash
   python -m pip install -r requirements.txt
   ```

6. Start Jupyter:

```bash
   jupyter notebook
   ```

7. Open `notebooks/Diwali\_Sales\_Analysis.ipynb` and run all cells from top to bottom.

The notebook supports running Jupyter from either the repository root or the `notebooks/` directory.

## Data handling

The included CSV omits direct customer identifiers (`User\_ID` and `Cust\_name`) and empty/unneeded columns (`Status` and `unnamed1`). The original file had 11,251 rows and 15 columns; 12 rows had missing `Amount` values. Those rows are excluded only from sales-amount calculations, not from analyses that do not require `Amount`.

**Dataset provenance:** The original source link and data dictionary were not provided with the project. Before making this repository public, confirm that you have permission to redistribute the dataset and add the original source and its license here. If redistribution is not permitted, remove the CSV from the repository and document how users can obtain it lawfully.

## Questions explored

* How do customer-record counts and recorded sales amounts vary by gender?
* Which age groups contribute the highest recorded sales amount?
* Which states rank highest by summed orders and recorded sales amount?
* How does recorded sales amount vary by occupation and marital-status code?
* Which product categories and product IDs rank highest in this dataset?

## Key findings

The current dataset indicates that:

* Gender code `F` has the largest total recorded sales amount.
* Age group `26-35` has the largest total recorded sales amount.
* Uttar Pradesh ranks first by recorded sales amount among states.
* `Food` is the highest-ranked product category by recorded sales amount.
* `IT Sector` is the highest-ranked occupation by recorded sales amount.

These are descriptive findings for the supplied data. They do not establish why the differences exist or prove that the same patterns will hold in other periods.

## Business interpretation

The results can help prioritize follow-up questions about customer segments, geographic performance, and product categories. Before using them for business decisions, confirm field definitions, currency units, and the dataset's collection period. Compare order counts with sales amounts and investigate whether differences are driven by order volume or average order value.

## Limitations and next steps

* Dataset source, license, and data dictionary need to be confirmed.
* The meaning of numeric `Marital\_Status` codes should be verified.
* Analysis is descriptive and does not establish causality.
* Potential extensions: average order value, cross-tabulation of state and category, statistical validation, and a Power BI dashboard.

## Author

Siddharth S Gaikwad
https://www.linkedin.com/in/siddharth-gaikwad-229232242/

