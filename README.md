# 🦈 Shark Attacks Data Analysis

## Overview
This project analyzes shark attack incidents worldwide. The dataset is cleaned and validated to ensure accurate country names and coordinates are used for visualization. The analysis culminates in a geographical representation of shark attack incidents, highlighting the countries most affected.

## 📚 Table of Contents 

* __Installation__

* __Usage__

* __Data Cleaning Process__

* __Coordinate Extraction__

* __Visualization__

* __Technologies Used__

      
## 🛠️ Installation

To run this project, you need to have Python installed along with the required libraries. You can install the necessary libraries using pip:

     pip install pandas numpy openpyxl geopy plotly
## 🚀 Usage
1. Clone the repository:
    
      git clone <repository-url>
      cd shark-attacks-data-analysis
    
2. Place the dataset file (`GSAF5.xls`) in the project directory.
    
3. Run the analysis script:
    
      python your_script_name.py
    
4. The final geographical plot will be displayed, showcasing shark attack incidents by country.

## 🧹 Data Cleaning Process

The data cleaning process involves several steps:

- __Loading the Dataset:__ The dataset is loaded from an Excel file into a DataFrame.
- __Whitespace Removal:__ Leading and trailing whitespace from the Country column is stripped.
- __Country Validation:__ Regex patterns are used to validate and categorize country names, including:
    *  All uppercase letters
    *  Proper capitalization
    *  Names separated by slashes or ampersands
- __Country Correction:__ Common naming issues are addressed (e.g., replacing "&" with "AND").
- __Filtering:__ Only valid countries are retained for further analysis.

## 🗺️ Coordinate Extraction
Using the Nominatim API from the geopy library, the latitude and longitude of each valid country are extracted. A delay is implemented to respect API rate limits.

## 📊 Visualization
The final analysis is visualized using ( `plotly` ):

A scatter geo plot displays the number of shark attack incidents per country.
The top five countries with the most incidents are highlighted for better visibility.

## 🛠️ Technologies Used

- __Python:__ The primary programming language.
-  __Pandas:__ For data manipulation and analysis.
- __NumPy:__ For numerical operations.
- __Geopy:__ For geographical coordinate extraction.
- __Plotly:__ For interactive data visualization.
- __Openpyxl:__ For reading Excel files.


