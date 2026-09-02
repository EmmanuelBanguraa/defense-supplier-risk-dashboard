# Defense Supplier Risk Dashboard (FOCI Scoring)

A Python/pandas project that scores fictional defense suppliers for 
Foreign Ownership, Control, or Influence (FOCI) risk — a core concept 
in supply chain risk management (SCRM) for defense contractors.

## What it does
- Generates a dataset of 40 fictional suppliers with realistic attributes 
  (country, industry, risk score, foreign ownership, single-source status)
- Applies a custom risk-scoring function that weighs FOCI-relevant factors:
  foreign ownership and single-source dependency both increase a supplier's 
  risk score
- Classifies each supplier as HIGH / MEDIUM / LOW risk
- Outputs a scored CSV ready for further analysis or reporting

## Results
Out of 40 suppliers: 22 HIGH RISK, 8 MEDIUM RISK, 10 LOW RISK

## Tools used
Python, pandas, Google Colab
