# The Impact of COVID-19 on Cook County, IL

## Goal of the Project

The goal of this project is to combine data on politicians across the world along with the countries they are from to identify any bias in the quality of the articles from those countries.

## Data Sources  
[Illinois Report Card Data](https://www.isbe.net/pages/illinois-state-report-card-data.aspx)  
[Chicago Public Schools Dropout Rates](https://www.cps.edu/about/district-data/metrics/)
[City of Chicago Progress Reports](https://data.cityofchicago.org/Education/Chicago-Public-Schools-School-Progress-Reports-SY2/ngix-dc87)
[RAW_us_confirmed_cases](https://www.kaggle.com/antgoldbloom/covid19-data-from-john-hopkins-university?select=RAW_us_confirmed_cases.csv)
[State and Territorial Mask Mandates](https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i)
[Mask Use Survey](https://github.com/nytimes/covid-19-data/tree/master/mask-use)

## Python Packages Used
pandas
matplotlib
scipy
numpy  

install in your CLI by running:  

`pip install {package_name}`

## Setup
* Download the [mask mandates dataset](https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i) and include it in the same directory as this readme.
* Install all needed packages and jupyter notebooks
* run A4567 COVID Analysis Cook County Data.ipynb within a jupyter environment

## Data Dictionary
As seen in this repository, there are many datasets that were procured for this analysis.
The only datasets used to identify the findings in the final analysis notebook (A4567 COVID Analysis Cook County Data.ipynb)
was the mask mandates dataset, the confirmed cases dataset, and the
state education dataset. All other datasets were used in exploratory data analysis and will
not be documented in the data dictionary.

### Data Dictionary for state_data.csv
Year: School year for which data is collected  
RCDTS:Unique school identifier  
School Name: Name of school  
City: City school is located in  
County: County school is located in, filtered to only cook county  
Title 1 Status: Whether the school qualifies or is enrolled in a title 1 program. See detailed definition below.  
Student Attendance Rate: Number of days a student is present as a percentage of total number of school days  
Student Mobility Rate: Unduplicated count for students who transferred in and out of the serving school at  
any time during the school year (October 1 – May 1) for reasons other than normal educational program transitions  
Student Chronic Truancy Rate: Include the number of chronic truants, divided by enrollment, multiplied by 100  
High School Dropout Rate - Total: Percentage of students enrolled who drop out  
School Type: Elementary, Middle, High School, or Charter School  
Teacher Retention Rate: Three year average of the percentage of teachers returning to the school from the previous year  

For more detailed definitions, see [here](https://www.isbe.net/Documents/2021-Report-Card-Glossary-Terms.pdf)  

### Data Dictionary for U.S._State_and_Territorial_Public_Mask_Mandates_From_April_10__2020_through_August_15__2021_by_County_by_Day.csv
Dataset is too large to be included in repository. See "State and Territorial Mask Mandates" link above and include it in the same directory  
as this readme.  

State_Tribe_Territory:Two letter code for US State  
County_Name: Name of County  
FIPS_State: Digit code for state  
FIPS_County: Digit code for county  
date: Date in which a mask mandate may have been in place  
order_code: 
Face_Masks_Required_in_Public: Whether masks were required at that date  
Source_of_Action: Type of data source  
URL: URL for data source  
Citation: Type of data source  

### Data Dictionary for RAW_us_confirmed_cases.csv  
Province_State: U.S. State  
Admin2: County  
UID: Unique identifier  
iso2: Region  
iso3: Region  
code3:  
FIPS: Unique Identifier  
Country_Region: Country  
Lat: Latitude  
Long_: Longitude  
Combined_Key: Combined State, County, Country  
Date Columns: Each column contains the case count at that date  
