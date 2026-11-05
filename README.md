# Defense Supplier Risk Dashboard (FOCI Scoring)

A Python/pandas project that scores 40 fictional defense suppliers for Foreign Ownership, Control, or Influence (FOCI) risk, a core concept in supply chain risk management (SCRM) for defense contractors, with an interactive Tableau dashboard that shows which suppliers need risk mitigation first.

**Live dashboard:** [View on Tableau Public](https://public.tableau.com/app/profile/emmanuel.bangura/viz/DefenseSupplierRiskDashboard/Dashboard1)

![Dashboard preview](dashboard.png)

## The question

Which suppliers carry the most risk from foreign ownership, control, or influence (FOCI) and single-source dependency, and where should procurement act first?

## Findings

- 22 of 40 suppliers are rated high risk, 8 medium, and 10 low.
- Foreign-owned suppliers run above the overall high-risk rate of 55%: 63% for foreign-owned multi-source suppliers and 60% for foreign-owned single-source suppliers. Both domestic groups sit at 50%.
- USA and India have the highest average risk score (7.0), and Mexico the lowest (4.4).

## How it works

1. **Data (Python, pandas):** 40 fictional suppliers with a country, industry, risk score (1 to 10), a foreign-ownership flag, and a single-source flag.
2. **Scoring:** A custom risk-scoring function weighs FOCI-relevant factors. Foreign ownership and single-source dependency both increase a supplier's risk, and each supplier is classified as high, medium, or low risk.
3. **Dashboard (Tableau Public):** Three charts and a supplier lookup table. Clicking any chart filters the table, so a user can go from a risk group straight to the suppliers in it.

## Dashboard views

| View | What it shows |
|---|---|
| Suppliers by risk tier | Supplier count in each tier |
| High risk share by ownership and sourcing | Percent high risk for each ownership and sourcing group, against the 55% overall rate |
| Average risk score by country | Average score per country, with the overall average marked |
| Supplier lookup | All 40 suppliers sorted by risk score, filterable by tier, country, and industry |

## Files

| File | Description |
|---|---|
| `Project1_FOCI_Dashboard.ipynb` | Python notebook: data, scoring, and export |
| `suppliers_scored.csv` | Final scored supplier data used by the dashboard |

## Tools

Python, pandas, Google Colab, Tableau Public

## Note

All supplier names and data are fictional.
