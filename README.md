**Patient Survival Prediction – Hospital Data Analysis Project**

**Project Summary:**  
This project aims to understand the factors affecting in-hospital mortality rates by analyzing data related to the ICU processes of hospitalized patients. The dataset used includes patient demographic information, ICU admission sources, ICU types, and specific clinical measurements.

**Dataset:**  
The dataset contains detailed information about patients' conditions within the hospital and ICU. It includes missing values and various data types (numerical and categorical). During data processing, missing value analysis and data cleaning were performed.

**Dataset Features:**  
- **Ethnicity:** 6 categories, missing values are NaN.  
- **Gender:** 2 categories (M, F), missing values are NaN.  
- **ICU Admit Source:** 5 categories.  
- **ICU Stay Type:** Initial admission, readmission, or transfer.  
- **ICU Type:** 8 different types.  
- **Apache 3J Body System:** 12 body system categories.  
- **Apache 2 Body System:** 11 body system categories.

**Libraries Used:**  
- **Pandas:** Data processing and analysis.  
- **Matplotlib & Seaborn:** Data visualization.  
- **Missingno:** Missing data analysis and visualization.  
- **Scikit-learn:** Machine learning and prediction.

**Analysis Performed:**  
1. **Data Inspection and Cleaning:**  
   - Data type checks: Each column was reviewed, and categorical and numerical data types were separated.  
   - Missing Data Analysis: The missingno library was used to detect and visualize missing values.  
   - Missing data treatment:  
     - Rows were deleted if there was a high rate of missing values.  
     - Missing values were filled using mean, median, or mode methods.  

2. **Categorical Variable Analysis:**  
   - Frequency and percentage distributions were examined.  
   - Relationships between categories were analyzed using cross-tabulation.  
   - Visualizations were created with bar charts.

3. **Numerical Data Analysis:**  
   - Distribution and basic statistical metrics were examined.  
   - Outliers were detected through box plots and histograms.

4. **Missing Data Strategies:**  
   - **Deletion:** Rows with randomly distributed or low missing data were deleted.  
   - **Imputation:** Missing data was filled using mean, median, or mode. Forward and backward filling techniques were used for time series data.

**Outputs and Results:**  
The analysis identified key factors affecting in-hospital mortality rates, including:  
- Patient demographics (gender, ethnicity).  
- ICU admission source and type.  
- Clinical measurements based on Apache scores.  

These findings can provide insights for hospital management to improve patient care processes.


# Projenin Kaggle Linki : https://www.kaggle.com/code/ahmeteren9/patient-survival-prediction

