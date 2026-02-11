# Customer Churn Predictor

A practical pipeline to predict customer churn and produce simple SHAP-based explanations.
--------------------
## What’s included
- `src/preprocess.py` — clean raw customer CSV and encode features
- `src/train.py` — train an XGBoost classifier and save model + metadata
- `src/explain.py` — produce SHAP explanations for individual customers
- `requirements.txt` — library list
====
## Data expectations
Input CSV should include a column `churn` with values 0 or 1. Additional columns can be numeric or categorical (e.g., tenure, monthly_charges, contract_type).

Optional columns:
- `customer_id` (kept if present)

## Quickstart
---

1. Create environment and install:
```bash
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate
pip install -r requirements.txt
---
