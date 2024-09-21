# **Geochemical Data Exploration and Classification Using Earth MRI Dataset**

## **Project Overview**
This project is an extensive exploratory data analysis (EDA) and classification of geochemical data from the Earth Mapping Resources Initiative (Earth MRI) dataset. The dataset includes geochemical measurements aimed at identifying mineralized areas containing critical minerals across various regions. The goal of this project is to explore, clean, and analyze the data, as well as build a machine learning model to classify geological ages based on geochemical features.

## **Table of Contents**
1. [Dataset](#dataset)
2. [Project Steps](#project-steps)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Results](#results)
6. [Contributing](#contributing)
7. [License](#license)

## **Dataset**
The dataset used in this project is provided by the U.S. Geological Survey (USGS) as part of the Earth MRI initiative:
- **Primary Dataset**: Geochemical measurements of various samples (EMRI_Data.csv).
- **Supplementary Datasets**:
  - **Data Dictionary**: Descriptions of the data fields (EMRI_DataDictionary.csv).
  - **Limits of Analytical Methods**: Detection limits for different elements (Limits_AnalyticalMethods.csv).
  - **QA/QC Values**: Quality control data for reference materials (QAQC_Values.csv).

## **Project Steps**

1. **Data Loading and Exploration**:
   - Load and inspect the primary and supplementary datasets.
   - Review data dictionary for understanding feature descriptions.
   
2. **Data Cleaning**:
   - Handle missing values via imputation (mean for numeric columns).
   - Detect and remove outliers using Z-scores.

3. **Descriptive Statistics and Correlation Analysis**:
   - Generate summary statistics and correlation heatmaps.
   - Perform multicollinearity analysis using Variance Inflation Factor (VIF).

4. **Distribution Analysis**:
   - Visualize the distribution of geochemical features using histograms and box plots.
   
5. **Geospatial Visualization**:
   - Use Folium to create interactive maps displaying sample locations.
   
6. **Feature Engineering**:
   - Encode categorical variables using Label Encoding and One-Hot Encoding.

7. **Class Imbalance Handling**:
   - Address class imbalance in the **Geologic Age** target variable using SMOTE.

8. **Modeling**:
   - Build a Random Forest classifier to predict geological ages.
   - Evaluate the model using confusion matrix and classification metrics.

9. **Cross-Validation**:
   - Validate the model using 5-fold cross-validation.

10. **Feature Importance**:
    - Analyze and visualize the most important features affecting the classification.

## **Installation**

1. Clone the repository:
    ```bash
    git clone https://github.com/VENKAT1pandi/Geochemical-Data-Exploration-and-Classification-Using-Earth-MRI-Dataset.git
    cd Geochemical-Data-Exploration-and-Classification-Using-Earth-MRI-Dataset
    ```

2. Create a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## **Usage**

1. To run the analysis, ensure you have Jupyter Notebook installed:
   ```bash
   pip install notebook
   jupyter notebook
