# Project_1: North Carolina Crime Data Investigation Project

Overview

The Crime Data Investigation Project focuses on analyzing and interpreting crime data collected from the Crime Data Explorer for North Carolina. Our objective is to gain valuable insights into the patterns, trends, and factors associated with crime in the region. By leveraging data analytics techniques, we aim to contribute to a better understanding of the dynamics of criminal activities and changes in the past 10 years across the state.

Key Objectives:
  1.	Data Exploration: Dive into the Crime Data Explorer for North Carolina to understand the available datasets and     variables.
  2.	Analysis of Crime Trends: Identify and analyze patterns and trends in various types of crimes over time and across different regions  within North Carolina.
  3.	Demographic Correlations: Explore correlations between crime rates and demographic factors, such as population density, income levels, and education.
  4.	Community Impact: Consider the implications of the findings on community safety, law enforcement strategies, and policy recommendations.

Team Members:
  Ashleigh Wittenburg
  Brittney Watts
  Payal Bansal
  Lyane Batchi

Data Source
  1.	Crime Data Explorer API:
     
     •	The primary data source is the Crime Data Explorer API from https://api.usa.gov/crime/fbi/cde/.
  2. 	Endpoint for Agency Data:
     
    • The agency endpoint is used to retrieve agency data based on the state abbreviation ("NC" for North Carolina).
   3.	Endpoint for Crime Data:
      
    •	The summarized/agency endpoint is used to retrieve summarized crime data for each agency. 
    •	The offense type, start year, and end year are specified.

Data Analysis:
  1.	Looping Through Agencies: 
    •	The script iterates through the list of agencies obtained and constructs URLs to fetch crime data for each agency.
  2.	Creating DataFrames:
    •	The script creates a pandas DataFrame (crime_df) to store the crime data obtained from each agency.
  3.	Merging DataFrames: 
    •	The script merges the agency data DataFrame (agency_df) and the crime data DataFrame (crime_df) based on the common          key 'ori'.
  4.	Output:
    •	The merged DataFrame (merge_df) is saved to a CSV file in the "Output" directory.
  5.	Potential Analysis:
    •	Analysis of Violent Crimes by agency types
    •	Crime Density Among different agencies
    •	Analysis top 10 counties with crime count
    •	Total crime committed and solved over 10 years

Technologies Used
  1.	Programming Language:
    •	Python
  2.	Libraries and Modules:
    •	Requests: For making HTTP requests to the Crime Data Explorer API.
    •	Pandas: For data manipulation and analysis.
    •	NumPy: For numerical operations and array manipulations.
    •	JSON: Part of the Python standard library, used for handling JSON data.
    •	PPrint: Part of the Python standard library, used for pretty-printing data structures.
  3.	API:
    •	Crime Data Explorer API: The primary data source for crime data in North Carolina.
  4.	Integrated Development Environment (IDE):
    •	Jupyter Notebook: Used for writing, testing, and debugging the Python script.
  5.	Version Control:
    •	Git: Used for version control and collaborative development.
  6.	Project Documentation:
    •	README.md: For project documentation and instructions.

Results
Analysis of Violent Crimes by agency type

![image](https://github.com/brittnwatts/Project_1/assets/150114216/b156878e-d674-4db7-bec3-e5f73d6a1da0)


Crime Dentsity among different agencies
 
![image](https://github.com/brittnwatts/Project_1/assets/150114216/94cff0fb-6add-4f84-a135-0aa7882188ff)

Analysis of top 10 and top county wrt crime count
 
![image](https://github.com/brittnwatts/Project_1/assets/150114216/58b757ba-350f-49cc-8ad7-bcf6cdfba443)


Analysis of total crimes committed over years
 
![image](https://github.com/brittnwatts/Project_1/assets/150114216/1b7c1ca0-7fe9-4a0b-9c33-5fafb2733acc)

solve rate here

 

Conclusions
