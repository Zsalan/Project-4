# Project-4

NRI Risk Analysis and Model Comparison

This Python Programming Assignment 4 is completed by Abdi Aden for CIVE 202 and is intended to be shared with the instructor.

# Purpose

This project involves the analysis of real-world data related to natural disaster risk. The project involves the following:

FEMA National Risk Index (NRI) - national disaster risk data

ATSDR Social Vulnerability Index (SVI) - community vulnerability data

## The purpose of the project is:

To evaluate FEMA’s current risk assessment methodology
To create a custom hazard-based risk model using physical variables only
To compare FEMA risk scores with custom risk calculations
To analyze how social vulnerability and resilience affect results
To demonstrate the use of Python in engineering data analysis and decision-making

The project also shows the potential for Python to be used as an engineering tool instead of traditional tools such as Excel.

Repository Contents

This repository includes all the required materials for Project #4. The materials are as follows:

README.md
- A summary of the project and a guide on how to run the code

Scope of Work (SOW)
- A detailed outline of the project activities and requirements

Annotated Code Document (ACD)
- An explanation of the Python code written

Technical Report
- A comprehensive report comprising an introduction, methods, results, and discussion

Gantt Chart
- A project plan showing the project timeline and scheduling

Engineering Timesheet
- A log of the hours spent working and the activities completed

Python Code (.ipynb)
- A Jupyter Notebook that is used to produce the analysis and results

Datasets (NRI, SVI, Shapefile)
- Data required for the project

## How to Run the Code

Make sure you have Python installed with the following libraries:

pip install pandas numpy matplotlib geopandas scikit-learn

Open the file:

Project-4_CIVE-102_AbdiAden.ipynb

in Jupyter Notebook or VS Code

# Run each section top to bottom:

## Import Libraries
Loads pandas, numpy, matplotlib, geopandas, scikit-learn

Load Datasets
Reads: Alaska NRI California NRI Alaska SVI California SVI Shapefile

## Data Cleaning
Selects variables: earthquake, wildfire, cold wave, SOVI, RESL
Handles missing values using median replacement
Fixes merge keys (STCNTY, TRACTFIPS)
Removes duplicates

Data Processing
Merges datasets
## Calculates hazard-based risk:

Earthquake Risk = ERQK_AFREQ × ERQK_EXPB
Wildfire Risk = WFIR_AFREQ × WFIR_EXPB
Cold Wave Risk = CWAV_AFREQ × CWAV_EXPB

Normalizes values and creates custom risk score

# Data Visualization

The code generates:

## Maps
- FEMA Risk vs Custom Risk (side-by-side)

## Bar Charts
- Top 10 highest risk counties
- Top 10 lowest risk counties

## Tables
- Mean risk comparisons by county

After running the code the program will:

Display all maps and charts
Show comparisons between FEMA and custom risk
Provide visual insight into how risk definitions change results

## Results

Removing social variables significantly changes risk rankings
Some areas ranked high by FEMA are not high in the hazard-only model
FEMA’s model reflects both hazard and social vulnerability
The custom model isolates physical hazard risk only
Risk results vary depending on how risk is defined

# Engineering Relevance

## This project is important for:

- Disaster risk assessment
- Infrastructure planning
- Emergency management
- Resource allocation
- Public policy decisions

# Project Timeline

## The project followed a structured schedule including:

Data review
Cleaning and processing
Risk model development
Visualization creation
Report writing

(Look at Gantt Chart for full breakdown)

Work Summary

Total Hours Worked: 36.8

## Tasks included:

Data cleaning
Model development
Visualization
Report writing
Debugging and validation

## Final Deliverables

Python Code (.ipynb)

Annotated Code Document

Scope of Work

Gantt Chart

Engineering Timesheet

Technical Report

GitHub Repository

## References

FEMA National Risk Index (NRI)
ATSDR Social Vulnerability Index (SVI)
FEMA Risk Methodology Documentation
CIVE 202 Course Materials
