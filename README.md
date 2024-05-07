# Anomaly Detection and Root Cause Analysis in Time Series Data

## Project Description

This project involved analyzing multiple sets of time series data with corresponding anomaly labels. The objective was to understand the data's characteristics, identify potential root causes of the anomalies, and determine the variables contributing most significantly to them.

## Data Acquisition

The data was provided in a ZIP file containing four sets of CSV files. Each set consisted of a data file (e.g., test.csv) containing multivariate time series data and a corresponding label file (e.g., test_labels.csv) specifying anomaly region timestamps.

## Methodology

1. **Data Preprocessing (a)**: Python code was developed using libraries like Pandas to read the data from both the time series and label files. This resulted in DataFrames for easy manipulation and analysis.

2. **Visualization and Exploration (b)**: Time series plots were created to visualize the values of each variable over time. These plots were further enhanced by highlighting anomaly regions using visual cues. This facilitated visual inspection of data and variable behavior during anomalies.

3. **Exploratory Data Analysis (c)**: A comprehensive EDA was conducted to understand the data's characteristics and potential causes of anomalies. This involved:

    - **Statistical Analysis**: Statistical properties like mean, median, and standard deviation were calculated for each variable across the entire dataset and within anomaly and non-anomaly periods. Significant changes in these statistics during anomalies were investigated.
    - **Relationship Exploration**: Scatter plots and correlation matrices were utilized to explore relationships between variables. Particular attention was paid to unusual patterns or changes in relationships during anomalies.
    - **Domain Knowledge Integration (if applicable)**: If relevant domain knowledge about the data generation process was available, it was used to interpret the findings from statistical analysis and visualizations.

4. **Identifying Root Cause Variables (d)**: A crucial aspect of the project involved pinpointing variables contributing most to the anomalies. This was achieved through several techniques:

    - **Statistical Tests**: Statistical tests like t-tests or ANOVA were conducted to compare the means or variances of variables during anomaly and non-anomaly periods. Variables exhibiting statistically significant differences were considered strong candidates for contributing to anomalies.
    - **Anomaly Detection Models (if applicable)**: When appropriate domain knowledge about anomaly types was available, anomaly detection models (e.g., Isolation Forest, LSTMs) were trained. The models potentially provided insights into which features were most relevant to the detected anomalies.
    - **Domain Knowledge Application**: My understanding of the data generation process was utilized to identify variables that could logically lead to the observed anomalies.

## Outcomes

This project successfully explored time series data, identified potential root causes of anomalies, and determined the variables contributing most to them. The developed Python code and analysis techniques can be applied to other datasets with similar characteristics for future anomaly detection and root cause investigation.

