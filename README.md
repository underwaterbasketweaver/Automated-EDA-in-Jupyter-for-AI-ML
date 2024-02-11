# Automated-EDA-in-Jupyter-for-AI-ML

## Documentation of Updates, Bug Fixes, and Improvements
## Version: 1.1
## Date: February 11, 2024
## Overview
This documentation outlines the updates, bug fixes, and improvements made to the automated EDA notebook creation script. These changes aim to enhance functionality, ensure compatibility with various data types, and improve user experience by providing clearer, error-free visualizations and analyses.

## Updates
Dynamic Data Loading: Extended the data loading function to support various file formats including CSV, Excel (.xls, .xlsx), and JSON. This update allows users to input data files in these formats directly into the notebook creation script.

Improved Error Handling:Integrated try-except blocks and conditional checks to gracefully handle errors that may arise during data loading and processing. This ensures the script runs smoothly without interruption.

## Bug Fixes
Non-Numeric Data Handling in Visualizations: Addressed an issue where attempting to create visualizations (e.g., scatterplot matrices, correlation heatmaps) with non-numeric data types would result in errors or warnings. The script now automatically filters for numeric data types before generating these visualizations.

ValueError in Correlation Heatmap: Fixed a ValueError that occurred when attempting to generate a correlation heatmap with non-numeric columns present in the dataset. The script now selectively includes only numeric columns for correlation analysis.

## Improvements
Selective Visualization for Data Types: Enhanced the script to check column data types and selectively apply visualizations appropriate to those types. For example, count plots are now generated only for categorical data, and box plots and histograms are limited to numeric data.

ADF Test Compatibility Check: Added a compatibility check for the Augmented Dickey-Fuller (ADF) test to ensure it is only performed on numeric columns, thus avoiding errors related to data type incompatibility.

User Experience Enhancements: Made improvements to the script's output, including clear messages when certain types of data are not present for expected visualizations. This makes the notebook's output more informative and easier to interpret.

## Instructions for Users
Running the Script: Users should ensure their data file is accessible in the specified path and enter the file path when prompted by the script.

Supported Data Formats: Currently, the script supports CSV, Excel, and JSON formats. Users are encouraged to convert their data into one of these formats for compatibility.

Reviewing Generated Notebooks: After running the script, users should review the generated notebook for any messages or notes regarding data compatibility or visualization adjustments. This can provide insights into data preprocessing needs.

## Future Directions
Support for Additional Data Formats: Plans to extend support to other data formats like Parquet and SQL databases.

Automated Data Cleaning: Investigating the integration of automated data cleaning steps before analysis to further streamline the EDA process.

Customization Options: Exploring user-defined settings for visualizations and analyses, allowing for more tailored EDA notebooks based on user preferences.

## Conclusion
These updates and improvements significantly enhance the automated EDA notebook creation script's functionality, making it a more robust and user-friendly tool for data analysis.  Try it out and feel free to reach out with any bugs or specialized needs.
