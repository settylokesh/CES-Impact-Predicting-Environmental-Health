
# CES Impact: Predicting Environmental Health

## Project Overview

This project aims to analyze the environmental and demographic characteristics in California communities using data from CalEnviroScreen 3.0 (CES 3.0). CES 3.0 identifies communities within California that are most impacted by pollution and most vulnerable to its effects. The project explores relationships between environmental, health, and socioeconomic factors and their impact on the cumulative CES 3.0 score, with a particular focus on developing predictive models to assist in policy simulation and decision-making.

## Problem Statement

The project investigates the association between various indicators (environmental, health, and socioeconomic) and the CES 3.0 score. Using statistical and machine learning techniques, the project aims to:
1. Identify significant indicators contributing to CES 3.0.
2. Develop predictive models for CES 3.0.
3. Provide actionable insights for improving environmental quality and public health outcomes in vulnerable communities.

## Data

### Source
The data used in this project comes from the [CalEnviroScreen 3.0](https://data.ca.gov/dataset/calenviroscreen-3-0-results) dataset, provided by the California Environmental Protection Agency (CalEPA). The dataset contains a wide variety of environmental, demographic, and health indicators for census tracts across California.

### Data Preprocessing
- The dataset required cleaning, which included addressing missing data using an imputation pipeline.
- Columns like **Pollution Burden**, **Population Characteristics (Pop. Char.)**, and **PM2.5** were central to the analysis as they represent critical environmental and demographic factors.

### Key Features
- **Pollution Burden**: Score representing pollution levels for each census tract.
- **Population Characteristics**: Socioeconomic and demographic vulnerability indicators.
- **PM2.5 Levels**: Particulate matter levels representing air quality.
- **CES 3.0 Score**: The target variable representing cumulative environmental vulnerability.

## Project Workflow

### 1. Data Exploration and Preprocessing
- Initial exploration included loading and cleaning the dataset.
- Handled missing data using an imputation strategy to ensure model accuracy.

### 2. Correlation Analysis
- **Correlation Matrix**: Identified relationships between CES 3.0 score and various predictors.
- Higher **Pollution Burden** and **PM2.5 levels** were associated with increased CES 3.0 scores.
- **Population Characteristics** also showed a strong relationship, indicating that socio-economic vulnerabilities play a role in community health risks.

### 3. Feature Engineering
- Extracted and transformed features that were most relevant to the prediction task.
  
### 4. Model Development
- Several machine learning models were tested to predict CES 3.0 scores:
  - **Linear Regression**
  - **Decision Trees**
  - **Random Forests**
  - **XGBoost**
  
- Performance metrics like **Mean Squared Error (MSE)** and **R-squared** were used to evaluate model performance.

### 5. Model Evaluation
- Comparative analysis was done to determine the best predictive model based on accuracy and interpretability.
- Visualizations, including **feature importance plots** and **error analysis**, provided insights into model effectiveness.

## Results and Insights

- Models identified key factors that contribute to environmental risks in California communities.
- **Pollution Burden** and **Population Characteristics** were strong predictors of CES 3.0 scores.
- The findings offer useful policy insights to target high-risk areas and improve community well-being.

## Dependencies

The project requires the following libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`

You can install these libraries using the following command:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

## How to Run

1. Clone the repository:
```bash
git clone https://github.com/settylokesh/CES-Impact-Predicting-Environmental-Health.git
```

2. Navigate to the project directory:
```bash
cd CES-Impact-Predicting-Environmental-Health
```

3. Open the notebook CES_Impact_Analysis.ipynb in Jupyter.


4. Run each cell to execute the analysis.

## Project Structure

- `CES_Impact_Analysis.ipynb`: Jupyter notebook containing the entire analysis from data exploration to modeling.
- `data/`:Folder containing the dataset.
- `README.md`: Detailed documentation of the project.
  
