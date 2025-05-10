# Machine Learning and Deep Learning - Final Exam
**May 16, 2025** | Final exam for Copenhagen Business School _Machine Learning and Deep Learning (CDSCO2004E)_.

#### Students:
- Caoimhe Gallahue [@caoimhegall](https://www.github.com/caoimhegall): _(175890)_
- Eirik Sundsøy [@eisu24ab](https://www.github.com/eisu24ab): _(176654)_

______________________________________________________________________________________________
## Montgomery County Crash Reporting Data :rotating_light:
For our project, we explored crash data from Montgomery County, Maryland. This dataset reports details about crashes occuring on county and local roadways as collected by the Montgomery County Police via the Automated Crash Reporting System (ACRS). These collision reports are based on preliminary information provided to the Maryland State Police Department by reporting parties. Therefore the raw reporting data may reflect:

- Information not yet verified by further investigation
- Preliminary collision classifications may be changed at a later date based upon further investigation
- Information may include mechanical or human error

### Problem Statement:
This project aims to develop a machine learning model that predicts the severity of injuries in traffic crashes based on initial input features from ACRS Maryland State Police Department reports. By providing a data-driven injury severity estimate, the model can support law enforcement in real-time crash reporting, improve consistency across entries, and assist in early triage decisions for emergency response.
______________________________________________________________________________________________
### Data:
Download the raw scraped data from data.gov [here](https://catalog.data.gov/dataset/crash-reporting-drivers-data). Or download the [`Crash_Reporting_-_Drivers_data.csv`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/data/Crash_Reporting_-_Drivers_Data.csv) raw file.

### Notebooks:
[`ML Final Discovery.ipynb`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/src/ML%20Final%20Discovery.ipynb) - Where we did all the data cleaning and EDA. 

[`ML Final.ipynb`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/src/ML%20Final.ipynb) - The modeling of the cleaned data

> [!NOTE] 
> Running `ML Final Discovery.ipynb` file will create a cleaned dataframe [`processed_data.csv`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/data/processed_data.csv) that we use for modeling.
______________________________________________________________________________________________
