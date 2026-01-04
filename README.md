# Data_Mining_Dengue
# Dengue Risk Prediction and Governance Response Framework

## Overview
This repository contains the implementation of a two-layer
data-driven framework for dengue early warning and policy
response evaluation in Bangladesh.

Layer 1 predicts dengue risk using climate, environmental,
and epidemiological indicators.

Layer 2 evaluates whether city corporation actions align
with predicted dengue risk.

## Dataset
We use the following dataset for Layer 1:

Hasan, Mehadi; Ifti, Eshraque Jabid; Ifty, Fihab (2025),
"Monthly Division-Level Dengue Cases & Mortality with Climate
and Environmental Indicators in Bangladesh (2020–2025)",
Mendeley Data, V2.
DOI: 10.17632/cgwjshkx5k.2

City corporation action data were manually curated from
official reports and media sources.

## Layer 1: Dengue Risk Prediction
- Models used:
  - Logistic Regression
  - Random Forest
  - XGBoost
- Evaluation metric: Accuracy, Precision, Recall, F1-score
- Selected model: Random Forest (best balance between accuracy
  and generalization)

## Layer 2: Governance Response Evaluation
- Action scores are computed based on mosquito control,
  cleanliness drives, and emergency interventions.
- Response Adequacy Score = Action_Score / Predicted_Risk
- Governance responses are categorized as:
  - Reactive
  - Moderate
  - Proactive

```bash
pip install -r requirements.txt
