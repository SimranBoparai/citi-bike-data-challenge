# Citi Bike Tableau Challenge 

Link to Tableau Public: 

# Table of Contents

- [Citi Bike Tableau Challenge](#citi-bike-tableau-challenge)
- [Table of Contents](#table-of-contents)
- [Challenge Overview](#challenge-overview)
  - [Dataset](#dataset)
- [Prerequisites](#prerequisites)
  - [Required Tools](#required-tools)
  - [Windows Installation Process](#windows-installation-process)
  - [Repository Setup:](#repository-setup)
- [Repository Structure](#repository-structure)
- [Challenge Instructions](#challenge-instructions)
- [Data Cleanup Code Example](#data-cleanup-code-example)
- [Acknowledgements](#acknowledgements)
- [Author](#author)


# Challenge Overview
This challenge analyzes the Citi Bike trip data from July 2023 to uncover two unexpected phenomena in bike usage patterns using Tableau. The analysis focuses on creating insightful visualizations and dashboards aimed at helping city officials make informed decisions about the bike-sharing system in New York City.


## Dataset
The dataset used in this project was downloaded from Citi Bike's trip data source. 

Data File Link: https://s3.amazonaws.com/tripdata/JC-202307-citibike-tripdata.csv.zip 


# Prerequisites

For the Citi Bike Tableau Challenge, ensure you complete the following requirements:

## Required Tools 
- Install Visual Studio Code,  Python, and Tableau on your machine 
- Install the Pandas and Numpy libraries

## Windows Installation Process
- Open your terminal or command prompt and run the following commands:

  ``` 
     pip install pandas
     pip install numpy
   ```


## Repository Setup:
  - Create a new repository called ```citi-bike-tableau-challenge``` on GitHub with a README file
  - Clone the repository to your local machine:   
  ```git clone https://github.com/yourusername/citibike-analysis.git``` 
  - Create a ipynb file called ```citibike_datacleaning.ipynb``` and Resources folder containing ```JC-202307-citibike-tripdata.csv``` to this folder 
  - Create a markdown file titled ```analysis```
  - Create a folder titled ```images```
  - Push the changes to your GitHub repository

```
git add .
git commit -m "Pushing updated notebook"
git push origin main
```


# Repository Structure
```- citi-bike-tableau-challenge
- citi-bike-data-challenge
    - images                      
    - Resources    
        - cleaned_JC-202307-citibike-trip_data
        - JC-202307-citibike-tripdata            
    - .gitignore                
    - citibike_datacleaning.ipynb    
    - analysis                    
    - README.md                 
```


# Challenge Instructions 

This challenge consists of three parts: data processing, visualization and analysis, and presentation. Each part contains specific tasks that need to be completed.

Data Preprocessing
- Cleaned the dataset using Python or Jupyter Notebook ```citibike_datacleaning.ipynb```
- Removed missing or inconsistent values to prepare the data for analysis in Tableau.
- Save the cleaned dataset as a csv file ```cleaned_JC-202307-citibike-trip_data.csv```

Visualization and Analysis
- Designed 2–5 visualizations for each discovered phenomena (4-10 total) using Tableau.
- Created two dashboards that help visualize key insights, trends, and unexpected phenomena.
- Create either a static map that displays all bike stations, showing start-to-end journeys with zip code data overlaid, or a dynamic map that tracks how the popularity of each station changes over time, also with zip code data overlaid.
- Write an analysis for the dashboards and map, highlighting key trends and insights. Be sure to explain the patterns you observe and any potential reasons behind them.

Final Presentation
- Developed a Tableau Story combining all visualizations and dashboards.


# Data Cleanup Code Example

```VS Code
# Check for missing values in each dataframe
print("July Data - Missing Values:")
print(july_data_df.isnull().sum())

# Drop rows with missing values
july_data_clean = july_data_df.dropna()

# Print the shape of the DataFrames to see how many rows were dropped
print(f"July Data: {july_data_clean.shape}")
```


# Acknowledgements

I want to mention the following individuals and resources for their assistance and support throughout this assignment: 
- Xpert Learning Assistant and ChatGPT
- Class Activities 


# Author

For any questions or feedback, please contact:
- Name: Gursimran Kaur (Simran)
- Email: kaursimran081999@gmail.com
