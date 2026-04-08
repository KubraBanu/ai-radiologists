# AI & Radiologists — Analyzing How AI Influences Diagnostic Efficiency

**Course:** BAN 5573 — Visual Analytics & Business Intelligence  
**Institution:** Clark University School of Business  
**Term:** Spring 2025  
**Team:** Kubra Banu, Joash Kawal, Aman, Manikar Goud Rasamalla

---

## Overview

This project investigates how Artificial Intelligence influences the **efficiency, speed, and accuracy** of radiologists when interpreting chest X-rays (CXR). With radiologists interpreting hundreds of X-rays daily and a global shortage of specialists, the need for AI-assisted tools is critical — this study analyzes that potential through NLP, machine learning classification, and sentiment analysis on radiology reports.

---

## Problem Statement

- Manual interpretation of chest X-rays is slow, error-prone, and not scalable
- Radiologists need tools to quickly answer: *"Is this report critical?"*
- AI can automate classification of reports and surface urgent cases faster

---

## Objectives

1. Automated classification of radiology reports using machine learning
2. Sentiment analysis on clinical reports for urgency comprehension
3. Improving radiologists' decision-making accuracy and speed through visual analytics

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| **KNIME** | Visual analytics workflow & ML pipeline |
| **Power BI** | Interactive dashboard for insights |
| **Python** | Data processing, NLP, ML modeling |
| **Tableau** | Supplementary visualizations |
| **NLP (NegBio / CheXpert)** | Extracting structured labels from radiology text |
| **SVM, Logistic Regression** | Classification models |

---

## Dataset

- **MIMIC-CXR** — Over 370,000 chest radiology reports from ICU and inpatient cases
- De-identified clinical data with multi-label findings (Cardiomegaly, Pleural Effusion, Consolidation, Pneumothorax, No Finding, etc.)
- NLP-extracted labels using NegBio and CheXpert labeling tools

---

## Methodology

1. **Data Preprocessing** — Cleaned and structured radiology reports from MIMIC-CXR
2. **NLP Labeling** — Applied NegBio and CheXpert to extract condition labels from unstructured text
3. **Sentiment Analysis** — Classified report tone (critical / normal) to flag urgent cases
4. **ML Classification** — Trained SVM and Logistic Regression models on TF-IDF features
5. **Visual Analytics** — Built KNIME workflow and Power BI dashboard for real-time insights
6. **Model Evaluation** — Assessed using ROC AUC, accuracy, precision, and recall

---

## Key Findings

- AI-assisted classification significantly reduces time to flag critical reports
- NLP-based sentiment analysis successfully identifies urgent vs. routine cases
- Models achieve strong AUC scores; SVM outperforms on high-dimensional TF-IDF features
- Visual dashboards enable radiologists to prioritize workload more effectively

---

## Files

| File | Description |
|------|-------------|
| `Final_code_Radiology.ipynb` | Main Python notebook — NLP, ML models, evaluation |
| `Final-Workflow-Radiology.knwf` | KNIME analytics workflow |
| `Final-Dashboard-Visual-Radiology.pbix` | Power BI dashboard |
| `Final-Project-Report-Visual-Radiology.pdf` | Full project report |
| `Visual-Analytics-Presentation-Radiology.pptx` | Presentation slides |
| `Final_reports_with_conditions_and_sentiment.csv` | Processed dataset with labels & sentiment |

---

## Results Summary

- Automated classification pipeline reduces manual triage time
- Sentiment scoring helps flag critical reports for immediate review
- Power BI dashboard provides real-time visibility into report urgency distribution

---

## References

- Johnson et al. — MIMIC-CXR Dataset
- Rajpurkar et al. — CheXNet deep learning model
- Irvin et al. — CheXpert labeling tool
- Peng et al. — NegBio NLP tool
- Gichoya et al. — AI bias in chest X-rays
- Niehoff et al. — Siemens AI-Rad Companion evaluation (2023)
