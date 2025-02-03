# Hepatitis Data Analysis

This project analyzes the hepatitis dataset by performing data cleaning, missing value imputation, and various statistical tests to understand the relationships between different variables and their impact on the outcome (Class). The dataset includes both categorical and numerical variables, and the analysis utilizes various techniques such as ANOVA, correlation, and Chi-Square tests.

## Steps Involved:

1. **Data Loading**:
   - The dataset is loaded into R from a CSV file.

2. **Missing Value Identification and Imputation**:
   - Missing values are identified and visualized for each column.
   - For categorical variables (e.g., Sex, Steroid, Fatigue), missing values are replaced by the mode of each respective column.
   - For numerical variables (e.g., Bilirubin, Alk.Phosphate), missing values are replaced by the mean of the respective column.

3. **Statistical Tests**:
   - **ANOVA**: Used to determine the impact of variables like Age, Bilirubin, Alk.Phosphate, Sgot, Albumin, and Protime on the "Class".
   - **Kendall Correlation**: Measures the ordinal relationship between variables such as Age, Bilirubin, Alk.Phosphate, etc., with "Class".
   - **Chi-Square Test**: Performed on categorical variables (e.g., Sex, Steroid, Fatigue) to assess their association with "Class".

4. **Correlation**:
   - **Pearson Correlation**: Computes the linear correlation between all numeric columns in the dataset.
   - **Spearman Correlation**: Computes the rank-based correlation between numeric columns.

## Requirements:
- R (version 3.x or higher)
- dplyr package

## Setup Instructions:

1. Clone the repository:
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2. Install the required R packages:
    ```r
    install.packages("dplyr")
    ```

3. Load the dataset by specifying the correct file path:
    ```r
    originalDataFrame <- read.csv("path_to_your_file/hepatitis_data.csv")
    ```

4. Run the R script:
    ```r
    source("hepatitis_analysis.R")
    ```

## Output:
- The script will display the structure of the dataset and the number of missing values for each column.
- A bar plot will be generated showing the number of missing values per column.
- The results of ANOVA, Kendall correlation, Chi-Square tests, and Pearson/Spearman correlations will be printed in the console.

## License:
This project is licensed under the MIT License - see the LICENSE file for details.

## Author:
[Your Name]
