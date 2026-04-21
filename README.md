# Project-4

## NRI Risk Analysis and Model Comparison
This Python Programming Assignment 4 is completed by Abdi Aden for CIVE 202 and is intended to be shared with the instructor.

## Purpose
This project evaluates how natural disaster risk is defined using FEMA’s National Risk Index (NRI) and compares it to an independently developed hazard-based risk model.

The purpose of this project is:

To evaluate the existing risk assessment methodology at FEMA
To create a new risk model relying solely on physical risks
To examine the impact of various definitions of risk on calculations
To pinpoint any biases introduced through social vulnerability and resilience factors
To prove the utility of Python in large-scale data analytics and engineering decisions

## Project Overview

Two states were analyzed at the census tract level using both:

## FEMA’s NRI Risk Model
A custom hazard-based model (earthquake + wildfire only)

The comparison highlights how removing social variables changes:

Risk rankings
Spatial distribution of high-risk areas
Interpretation of disaster vulnerability
Repository Contents

This repository includes all required materials for Project #4:

### README.md
– Overview of the project and instructions to run the code
### Python Code (.ipynb)
– Jupyter Notebook used for full analysis and visualization
### Scope of Work (SOW)
– Detailed plan outlining variables, datasets, and analysis approach
### Annotated Code Document (ACD)
– Line-by-line explanation of the Python code
### Gantt Chart
– Timeline of project tasks and dependencies
### Engineering Timesheet
– Log of hours worked and task distribution
### Written Report / Summary
– Final report including methods, results, and discussion
### Raw Data Files
– NRI dataset and supporting files used for analysis
How to Run the Code

Make sure Python is installed with the following libraries:

pip install pandas numpy matplotlib seaborn geopandas

Open the notebook:

Project4_CIVE-202_Abdi-Aden_Code.ipynb

Run each section in order:

1. Import Libraries
pandas
numpy
matplotlib
seaborn
geopandas

3. Load Data
NRI dataset
SVI dataset (if applicable)

4. Data Cleaning
Select relevant variables:
Earthquake risk variables
Wildfire risk variables
FEMA risk score
Handle missing values
Ensure consistent merge keys (STCNTY)

5. Data Processing
Merge datasets
Calculate hazard-based risk:
Earthquake Risk = ERQK_AFREQ × ERQK_EXPB
Wildfire Risk = WFIR_AFREQ × WFIR_EXPB
Total Custom Risk = Earthquake + Wildfire

7. Analysis
Group data by county or tract
Compute mean and summary statistics
Normalize values for comparison

9. Visualization

The code generates:

Bar chart comparing:
FEMA Risk vs Custom Risk
Tables showing:
Mean risk values per state
Optional maps (if GeoPandas used)
Results

Key findings from the analysis include:

Removing social variables significantly changes risk rankings
Some areas classified as high risk by FEMA are not high risk in the hazard-only model
FEMA’s model reflects broader vulnerability, not just physical hazard exposure
Custom model isolates physical risk but ignores community impact
Engineering Relevance

This project is important for:

Disaster risk assessment
Infrastructure planning
Emergency management
Resource allocation decisions
Policy development

It shows how model assumptions directly influence engineering decisions.

## Project Timeline

The project followed a structured workflow:

Data review and understanding
Data cleaning and merging
Risk model development
Statistical analysis
Visualization creation
Report writing

(See Gantt Chart for full schedule and dependencies)

## Work Summary

Total Hours Worked: (update with your final number)

Tasks included:

Data preprocessing
Model development
Visualization
Report writing
Debugging and validation
Final Deliverables
Python Code (.ipynb)
Annotated Code Document
Scope of Work
Gantt Chart
Engineering Timesheet
Written Report
Raw Data Files
GitHub Repository
GitHub Link Included

The GitHub repository contains all required materials for submission and reproducibility.

## References

FEMA National Risk Index (NRI)
ATSDR Social Vulnerability Index (SVI)
CIVE 202 Course Materials
FEMA Documentation on Risk Calculation
