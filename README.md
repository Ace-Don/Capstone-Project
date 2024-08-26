# Capstone-Project
## Table of Contents
1. Project Overview
2. Objectives
3. Dataset
4. Methodology
5. Results
6. Technologies Used
7. Acknowledgements

## Project Overview
This capstone project was conducted as part of the completion requirements for the IBM Data Science Professional Certificate program hosted on Coursera. The primary goal of this project was to use data on past Space X Falcon 9 Rocket Launches to determine under what conditions the first stage of the rocket will land.

## Objectives
The key objective of this project was to be able to build a model that will be able to predict the binary class of, 'land', or 'not land' after proper analysis of the conditions that affect the landing of the first stage of Falcon 9 rockets. This could considerably reduce the costs of these rockets, as a landed first stage could be reused on another rocket for another space flight.

## Dataset
The dataset used for this project was sourced from a Space X Representational State Transfer(REST) API; source: https://api.spacexdata.com/v4/launches/past , where we retrieved 90 records of 17 features,all related to Falcon 9 Launches . The key features include:

1.FlightNumber 
2.Date               
3.BoosterVersion     
4.PayloadMass        
5.Orbit              
6.LaunchSite         
7.Outcome            
8.Flights            
9.GridFins           
10.Reused - If the first stage was resued or not
11.Legs               
12.LandingPad       
13.Block              
14.ReusedCount        
15.Serial             
16.Longitude          
17.Latitude
        
## Methodology Overview
The project followed these steps:

- Data Collection(Web Scraping & REST APIs)
- Data Preprocessing
- Exploratory Data Analysis (EDA), even with SQL
- Modeling/Analysis with Python

## Results
The key findings of the project include:

1. Launch sites have different success rates. CCAFS LC-40, has a success rate of 60 %, while KSC LC-39A and VAFB SLC 4E has a success rate of 77%.
2. If you observe Payload Vs. Launch Site scatter point chart you will find for the VAFB-SLC launchsite there are no rockets launched for heavypayload mass(greater than 10000).
3. In the LEO orbit the Success appears related to the number of flights; on the other hand, there seems to be no relationship between flight number when in GTO orbit.
4. Landing sucess rate since 2013 kept increasing till 2020

## Technologies Used
This project was implemented using the following technologies and tools:
1. Programming Language: Python
2. Libraries/Packages: NumPy, Pandas, Scikit-learn, Folium, Plotly Dash
3. Data Visualization: Matplotlib, Seaborn
4. Environment: Jupyter Notebook

## Acknowledgements
I would like to thank IBM, Skills Network Labs, Coursera, and all the tutors within this Profesional Data Science program. Your time and efforts are highly appreciated.
