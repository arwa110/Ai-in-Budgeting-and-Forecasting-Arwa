# AI in Budgeting and Forecasting

**Bachelor Thesis** — Arwa Abdelmohsen Mohamed (58-25055)  
**Supervisor:** Dr. Ayman Alserafi  
**Faculty of Management Technology — Business Informatics**  
**German University in Cairo (GUC) — May 2026**

## Abstract

This thesis examines the application of Explainable Artificial Intelligence (XAI) in budgeting and forecasting modelling with a focus on achieving transparency without compromising forecast accuracy. A Design Science Research approach was used to design the AI-based budgeting and forecasting model. The integration of two XAI models, SHAP and LIME, was performed within the forecasting process. The designed artefact consists of two business processes, user stories, use case diagrams, BPMN models, wireframes, business rules, and test cases. The design was evaluated by means of an interview study involving a finance and a technical expert. The results suggest that a systematic incorporation of XAI technology within the budgeting process would facilitate bridging the interpretability gap.

## Research Question

> "How can XAI be effectively integrated into budgeting and forecasting processes to ensure transparency and trust while maintaining predictive accuracy and supporting organisational decision-making?"

## Repository Structure

```
├── dataset/            NYC Capital Construction Budget data
├── diagrams/           Draw.io source files for use case and BPMN diagrams
├── documentation/      Features report (docx)
├── project-code/       Google Colab notebook (.ipynb)
├── wireframes/         HTML source files for original and updated wireframes
└── README.md
```

### dataset/
Contains the NYC Capital Construction Budget dataset or a link to it. The dataset has 11,493 capital project records with 51 attributes covering planned commitments, adopted budgets, allocated funds, actual spending, project types, managing agencies, and project dates.

### diagrams/
Contains the editable Draw.io (.drawio) source files for the use case diagrams and BPMN diagrams used in both business processes. These can be opened and edited at [app.diagrams.net](https://app.diagrams.net/).

### documentation/
Contains the features report documenting the system design including business processes, user stories, use case diagrams, BPMN diagrams, business rules, wireframes, and test cases.

### project-code/
Contains the Google Colab notebook (.ipynb) that demonstrates the AI and XAI pipeline. The notebook applies three classification models (Logistic Regression, Random Forest, XGBoost) on the NYC Capital Construction Budget dataset, then uses SHAP for global feature importance and LIME for local prediction explanations.

### wireframes/
Contains the HTML source files for the wireframe prototypes built using Lovable, covering both the original wireframes (20 screens) and the updated wireframes after expert evaluation (18 screens).

## Setup & How to Run

### Prerequisites
- A Google account (to run the notebook on Google Colab)
- Python 3.x (if running locally)

### Required Libraries
```
pandas
numpy
matplotlib
seaborn
scikit-learn
shap
lime
```

### Steps to Run

1. Open the notebook in Google Colab:  
   [Open Notebook](https://colab.research.google.com/drive/1bfoWrtwdI5woyCa1wPJOmZCVadJ0hZ9v?usp=sharing)

2. Run all cells sequentially (Runtime → Run all)

3. The dataset loads automatically from the NYC Open Data portal — no manual download needed

4. The notebook will:
   - Load and preprocess the dataset
   - Perform feature engineering and feature selection
   - Train three classification models (Logistic Regression, Random Forest, XGBoost)
   - Apply SHAP to the Random Forest model for global feature importance
   - Apply LIME to explain individual budget predictions

## Dataset

**NYC Capital Construction Budget**  
- 11,493 capital project records  
- 51 attributes  
- Classification target: On Budget / Over Budget / Under Budget  
- Source: [NYC Open Data Portal](https://data.cityofnewyork.us/City-Government/Capital-Projects-Database-CPDB-Projects/fi59-268w/about_data)

## Links

| Resource | Link |
|----------|------|
| Wireframes | [https://chum-page-builder.lovable.app/](https://chum-page-builder.lovable.app/) |
| Colab Notebook | [Open in Colab](https://colab.research.google.com/drive/1bfoWrtwdI5woyCa1wPJOmZCVadJ0hZ9v?usp=sharing) |
| Dataset | [NYC Open Data](https://data.cityofnewyork.us/City-Government/Capital-Projects-Database-CPDB-Projects/fi59-268w/about_data) |
