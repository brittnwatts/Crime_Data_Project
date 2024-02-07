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
  1.	Crime Data Explorer API: The primary data source is the Crime Data Explorer API from https://api.usa.gov/crime/fbi/cde/.
  2. 	Endpoint for Agency Data: The agency endpoint is used to retrieve agency data based on the state abbreviation ("NC" for North Carolina).
  3.	Endpoint for Crime Data: The summarized/agency endpoint is used to retrieve summarized crime data for each agency. 	The offense type, start year, and end year are specified.

Data Analysis:
  1.	Looping Through Agencies: The script iterates through the list of agencies obtained and constructs URLs to fetch crime data for each agency.
  2.	Creating DataFrames: The script creates a pandas DataFrame (crime_df) to store the crime data obtained from each agency.
  3.	Merging DataFrames: The script merges the agency data DataFrame (agency_df) and the crime data DataFrame (crime_df) based on the common key 'ori'.
  4.	Output: The merged DataFrame (merge_df) is saved to a CSV file in the "Output" directory.
  5.	Potential Analysis:
     	Analysis of Violent Crimes by agency types,
     	Crime Density Among different agencies,
     	Analysis top 10 counties with crime count,
     	Total crime committed and solved over 10 years

Technologies Used
  1.	Programming Language: Python
  2.	Libraries and Modules:
      Requests: For making HTTP requests to the Crime Data Explorer API,
     	Pandas: For data manipulation and analysis,
     	NumPy: For numerical operations and array manipulations,
     	JSON: Part of the Python standard library, used for handling JSON data,
     	PPrint: Part of the Python standard library, used for pretty-printing data structures.
  4.	API:
     	Crime Data Explorer API: The primary data source for crime data in North Carolina.
  5.	Integrated Development Environment (IDE):
     	Jupyter Notebook: Used for writing, testing, and debugging the Python script.
  6.	Version Control:
     	Git: Used for version control and collaborative development.
  7.	Project Documentation:
     	README.md: For project documentation and instructions.

Results
Analysis of Violent Crimes by agency type

![image](https://github.com/brittnwatts/Project_1/assets/150114216/b156878e-d674-4db7-bec3-e5f73d6a1da0)
![image](https://github.com/brittnwatts/Project_1/blob/cc5a80c0871b17cbb752703a871500d6471e06d7/Output/ashleigh-line.png)

Crime Dentsity among different agencies
 
![image](https://github.com/brittnwatts/Project_1/assets/150114216/94cff0fb-6add-4f84-a135-0aa7882188ff)

Analysis of top 10 and top county wrt crime count
 
![image](https://github.com/brittnwatts/Project_1/assets/150114216/58b757ba-350f-49cc-8ad7-bcf6cdfba443)
![image](https://github.com/brittnwatts/Project_1/assets/150114216/7c1dd360-25f7-4626-bccd-06f5f2c62af3)

Analysis of total crimes committed over years
 
![image](https://github.com/brittnwatts/Project_1/assets/150114216/1b7c1ca0-7fe9-4a0b-9c33-5fafb2733acc)

Solve Rate Over Years 2013-2022

 ![image](https://github.com/brittnwatts/Project_1/blob/c617c1290a58c1e1399ff1826d542baee4749458/solve_rate.png)

Conclusions

1. From the first graph, the analysis of violent crimes by agency type, we can see that "City" agencies account for ~ 77% of violent crimes committed and ~ 73% of all solved. From this graph, we can also see that "County" agencies have the second most number of actual and cleared crimes.
2. From the Crime Density Map, we are able to see all of the individual agencies in the state and their crime rates relative to each other in the form of colored markers. The larger and darker the marker, the more crime. We observe that Agency with the largest marker and number of crimes is the Charlotte-Mecklenburg Police Department. The runner-ups are in order: Raleigh, Durham, Greensboro, Winston-Salem, Fayetteville
3. In the graph that analyzes the top 10 counties' crimes, we observed that Mecklenburg County as a whole, has the most crime in NC over the 10 year period. Mecklenburg county has highest number of cleared crimes as well but the cleared crimes are only ~41% of the total crimes. The runner-ups are in order: Forsyth County, Guilford County, Cumberland County.
4. In the Mecklenburg County graph, we see that there is a steep increase in crimes from 2019 to 2020 when it was COVID time, however cleared crime totals only increased a small amount relative to the normal cleared rate for Mecklenburg County.
5. In the Total Crimes Committed and Solved Over Time Graph, we can see that crime has steadily increased over the years 2013-2020. From 2020 to 2022, the actual crime counts have dropped. Finally, we have a Solve Rate Per Year Graph that shows us the percentages of crimes cleared for crimes committed over the same 10-year period. We see here that the rate of crimes solved has significantly decreased over the 10-year period consistently. 
