# Comprehensive-Water-Quality-Assessment-and-Potability-Prediction-using-Multi-parameter-Analysis


 

Analyse water quality parameters to predict potability using machine learning. Includes feature importance analysis, SMOTE for data balancing, and rigorous model evaluation. The goal is building robust predictive models to accurately classify samples, ensuring reliable and safe drinking water assessment.

## 📌 Project Overview
The objective of this machine learning project is to predict whether a given set of water quality parameters meets potability criteria (safe for drinking) based on the provided physical and chemical features.

## 🛠️ Key Features & Methodology
* **Data Balancing:** Implemented SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance for stable model training.
* **Hyperparameter Tuning:** Applied `RandomizedSearchCV` for optimal parameter selection and to prevent over/underfitting.
* **Feature Importance Analysis:** Utilized tree-based evaluations to extract and rank the most influential indicators of potable water.

## 📊 Dataset Details
* **Data Shape:** 2,650 rows and 10 columns.
* **Target Variable:** `Potability` (0 = Non-Potable, 1 = Potable).
* **Feature Importance Rankings (Top Contributors):**
  1. Chloramines (0.14)
  2. pH (0.13)
  3. Solids (0.12) / Sulfate (0.12)
  4. Hardness (0.11)
  5. Turbidity (0.09) / Trihalomethanes (0.09)
  6. Conductivity (0.08) / Organic Carbon (0.08)

## 📈 Model Performance Summary
* **Random Forest:** **0.88 Accuracy** (Most reliable, robust predictions with balanced precision/recall).
* **Decision Tree:** **0.77 Accuracy** (Clear, highly interpretable decision structure).
* **Naive Bayes:** **0.65 Accuracy** (Quick baseline execution, excels in specific class recall).

## 🗂️ Repository Structure
```text
├── data/
│   └── water_potability.csv        # Dataset containing 2,650 water samples
├── notebooks/
│   └── water_quality_analysis.ipynb # Jupyter Notebook containing complete pipeline & EDA
├── presentation/
│   └── Water_Quality_Assessment.pptx # Project presentation slide deck
├── main.py                         # Python script for model training and evaluation
├── requirements.txt                # List of required library dependencies
└── README.md                       # Project documentation
```

## ⚙️ Installation & Setup
1. Clone the repository:

   git clone https://github.com/Ruchithaml/Comprehensive-Water-Quality-Assessment-and-Potability-Prediction-using-Multi-parameter-Analysis

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage
Open the Jupyter notebook inside the `notebooks/` directory to explore the complete EDA, correlation matrices, and model pipelines. Alternatively, run the primary modeling script:
```bash
python main.py
```

