# Machine Learning and Deep Learning - Final Exam
**May 16, 2025**

Final exam for Copenhagen Business School _Machine Learning and Deep Learning (CDSCO2004E)_ Spring 2025.


### Students:

Caoimhe Gallahue _(175890)_: [@caoimhegall](https://www.github.com/caoimhegall), caga24ad@student.cbs.dk

Eirik Sundsøy _(176654)_: [@eisu24ab](https://www.github.com/eisu24ab), eisu24ab@student.cbs.dk

______________________________________________________________________________________________
## Montgomery County Crash Reporting Data :rotating_light:
For our project, we explored crash data from Montgomery County, Maryland. This dataset reports details about crashes occuring on county and local roadways as collected by the Montgomery County Police via the Automated Crash Reporting System (ACRS). These collision reports are based on preliminary information provided to the Maryland State Police Department by reporting parties. Therefore the raw reporting data may reflect:

- Information not yet verified by further investigation
- Preliminary collision classifications may be changed at a later date based upon further investigation
- Information may include mechanical or human error

### Problem Statement
This project aims to develop a machine learning model that predicts the severity of injuries in traffic crashes based on initial input features from ACRS Maryland State Police Department reports. By providing a data-driven injury severity estimate, the model can support law enforcement in real-time crash reporting, improve consistency across entries, and assist in early triage decisions for emergency response.

### Research Questions
- _Can machine learning models accurately predict crash severity in Montgomery County using ACRS data?_
- _How do tree-based models compare to a Multi-Layer Perceptron in performance?_
______________________________________________________________________________________________
### Data:
Download the raw scraped data from data.gov [here](https://catalog.data.gov/dataset/crash-reporting-drivers-data). 

[`Crash_Reporting_-_Drivers_data.csv`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/data/Crash_Reporting_-_Drivers_Data.csv): The raw file downloaded on April 23, 2025.
[`processed_data.csv`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/data/processed_data.csv): The crash data after processing and EDA.

______________________________________________________________________________________________
### Notebooks:
[`ML Final Discovery.ipynb`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/src/ML%20Final%20Discovery.ipynb): Data cleaning and EDA. 

[`ML Final.ipynb`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/src/ML%20Final.ipynb): Modeling of the cleaned data


> [!NOTE] 
> Running `ML Final Discovery.ipynb` file will create a cleaned dataframe [`processed_data.csv`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/data/processed_data.csv) that we use for modeling.
______________________________________________________________________________________________
### How to Run :police_car:
1. Download the cleaned data [`processed_data.csv`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/data/processed_data.csv)
2. Download the modeling Notebook [`ML Final.ipynb`](https://github.com/caoimhegall/CBS-MachineLearning-Final/blob/main/src/ML%20Final.ipynb)
3. Change the import to match your path for `processed_data.csv`

   ```df = pd.read_csv('\CHANGE TO YOUR PATH')```
5. Run in your IDE of choice

See the [Google Colab](https://colab.research.google.com/drive/1eoh7xT6KE-tnHjSp4Ycx-QoC7KNQtCwy?usp=sharing) version
______________________________________________________________________________________________
### Machine Learning Models Utilized
- Baseline: [Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
- [Random Forest Classifier] (https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
- [XGBoost Classifier](https://cloud.google.com/python/docs/reference/bigframes/latest/bigframes.ml.ensemble.XGBClassifier) (eXtreme Gradient Boosting)
- [MLPClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html) (Multi-layer Perceptron)

______________________________________________________________________________________________

