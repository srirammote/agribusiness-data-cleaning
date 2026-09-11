# Agribusiness Data Analysis and Machine Learning

## YuvaIntern – Machine Learning Data Analyst (Agribusiness)

This repository contains the complete work for the 4-week virtual internship project focused on agricultural data collection, cleaning, exploratory data analysis, machine learning, and agribusiness recommendations.

## Project Objective

The project uses an Indian crop-yield dataset to:

- Collect and inspect agricultural data.
- Clean and preprocess the dataset.
- Perform exploratory data analysis (EDA).
- Build a machine learning model to predict crop yield.
- Evaluate the model using standard regression metrics.
- Translate analytical and machine learning findings into practical agribusiness recommendations.

## Dataset

The cleaned dataset contains **19,689 records** and **10 columns** covering crop, year, season, state, area, production, rainfall, fertilizer, pesticide usage, and yield.

The final cleaned dataset is available in the repository as `cleaned_crop_yield.csv`.

## Project Structure

```text
agribusiness-data-cleaning/
├── cleaned_crop_yield.csv
├── data/
│   └── README.md
├── week1/
│   ├── README.md
│   └── Week_1_Task_Data_Collection_and_Cleaning.docx
├── week2/
│   ├── README.md
│   └── Week_2_EDA_Internship_Report.docx
├── week3/
│   ├── README.md
│   ├── crop_yield_model.py
│   └── Week_3_Crop_Yield_ML_Report.docx
├── week4/
│   ├── README.md
│   └── Week_4_Agribusiness_Findings_Recommendations_Report.docx
└── README.md
```

## Week 1 – Data Collection and Cleaning

The first week focused on collecting and preparing the agricultural dataset. Data-quality checks included missing values, duplicate records, inconsistent categorical values, invalid numeric values, and potential outliers.

The cleaned dataset was prepared for further analysis and machine learning.

**Deliverable:** `week1/Week_1_Task_Data_Collection_and_Cleaning.docx`

## Week 2 – Exploratory Data Analysis

The second week focused on exploratory analysis of crop yield and its relationship with agricultural variables such as area, production, rainfall, fertilizer, pesticide usage, crop, season, and state.

**Deliverable:** `week2/Week_2_EDA_Internship_Report.docx`

## Week 3 – Machine Learning Model

A **Random Forest Regression** model was developed to predict crop yield.

### Method

- Target variable: `Yield`
- Training/testing split: **80% / 20%**
- Categorical variables: one-hot encoded
- Model: Random Forest Regressor
- Number of trees: **100**
- Random state: **42**

### Model Evaluation

- **MAE:** 7.5773
- **RMSE:** 103.1508
- **R² Score:** 0.9867

The model achieved a high R² score on the test set, indicating that it explained most of the variation in the target variable under the selected train/test setup.

The complete implementation is available in `week3/crop_yield_model.py`.

**Deliverable:** `week3/Week_3_Crop_Yield_ML_Report.docx`

## Week 4 – Findings and Recommendations

The final week translated the analytical and machine learning results into practical agribusiness insights.

Key areas covered include:

- Model performance interpretation.
- Important predictive factors.
- Agricultural and business implications.
- Data-driven recommendations for crop planning and resource management.
- Limitations and possible future improvements.

**Deliverable:** `week4/Week_4_Agribusiness_Findings_Recommendations_Report.docx`

## How to Run the Machine Learning Code

From the repository root, install the required Python libraries:

```bash
pip install pandas scikit-learn numpy
```

Then run:

```bash
python week3/crop_yield_model.py
```

The script loads `cleaned_crop_yield.csv`, trains the Random Forest regression pipeline, generates predictions, and prints MAE, RMSE, and R² evaluation metrics.

## Final Outcome

The project demonstrates an end-to-end agribusiness data workflow:

**Data Collection → Data Cleaning → EDA → Machine Learning → Evaluation → Agribusiness Recommendations**

This repository contains the weekly reports, cleaned dataset, and machine learning implementation required for the internship project.
