# Airbnb-Data-Analysis
This project performs an in-depth analysis of an Airbnb dataset to understand various aspects of the listings, including pricing, location, room types, and review trends.

## Project Goals
The primary objectives of this project are to:

Clean and preprocess the raw Airbnb dataset.
Explore the distributions of key variables like price and room type.
Visualize the geographical distribution of listings across different neighbourhood groups.
Investigate the relationship between price and room type.
Analyze the trend of reviews over time.

## Methodology
The analysis follows a standard data analysis workflow:

Data Loading: The dataset is loaded using pandas.
Data Cleaning: Missing values in 'reviews per month', 'last review', 'NAME', and 'host name' are addressed. The 'house_rules' and 'license' columns are dropped. Price and service fee columns are cleaned and converted to numeric types. Duplicate rows are removed.
Descriptive Statistics: Summary statistics are generated to understand the central tendencies and spread of numerical data.
Visualization: Various plots are created using Matplotlib and Seaborn to visually represent the data and findings.

## Key Findings
The analysis provides insights into:

The overall distribution of listing prices.
The prevalence of different room types within the dataset.
The concentration of Airbnb listings in specific neighbourhood groups.
How pricing varies across different room types.
The pattern and volume of reviews over time.

## Repository Contents
Jupyter Notebook containing the complete analysis code.
airbnb_data.csv: The dataset used for the analysis.

## How to Run
Clone this repository to your local machine.
Make sure you have Python installed along with the necessary libraries (pandas, numpy, matplotlib, seaborn). You can install them via pip:
pip install pandas numpy matplotlib seaborn

Open the Jupyter Notebook (.ipynb file) in a compatible environment (like Google Colab, Jupyter Notebook, or JupyterLab).
Run the cells sequentially to execute the data cleaning, analysis, and visualization steps.
This README provides a good overview of your project for potential viewers on GitHub. Remember to replace airbnb_data.csv with the actual filename of your dataset if it's different.
