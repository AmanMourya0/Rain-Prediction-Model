# Rain-Prediction-Model
A CNN-Model trained on Australian rainy weather for Rain Prediction

<h2>Table of Contents</h2>
<div class="alert alert-block alert-info" style="margin-top: 20px">
    <ul>
    <li><a href="#Section_1">Instructions</a></li>
    <li><a href="#Section_2">About the Data</a></li>
    <li><a href="#Section_3">Importing Data </a></li>
    <li><a href="#Section_4">Data Preprocessing</a> </li>
    <li><a href="#Section_5">One Hot Encoding </a></li>
    <li><a href="#Section_6">Train and Test Data Split </a></li>
    <li><a href="#Section_7">Train Logistic Regression, KNN, Decision Tree, SVM, and Linear Regression models and return their appropriate accuracy scores</a></li>
</a></li>

<hr>


# Instructions
<div id="Section_1">
In this repository, you will  practice the classification algorithms.

Below, is where we are going to use the classification algorithms to create a model based on our training data and evaluate our testing data using evaluation metrics.

We will use some of the algorithms, specifically:

1.  Linear Regression
2.  KNN
3.  Decision Trees
4.  Logistic Regression
5.  SVM

We will evaluate our models using:

1.  Accuracy Score
2.  Jaccard Index
3.  F1-Score
4.  LogLoss
5.  Mean Absolute Error
6.  Mean Squared Error
7.  R2-Score

Finally, you will use your models to generate the report at the end.
</div>

# About The Dataset
<div id="Section_2">
The original source of the data is Australian Government's Bureau of Meteorology and the latest data can be gathered from 
[http://www.bom.gov.au/climate/dwo/](http://www.bom.gov.au/climate/dwo/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01).

The dataset to be used has extra columns like 'RainToday' and our target is 'RainTomorrow', which was gathered from the Rattle at [https://bitbucket.org/kayontoga/rattle/src/master/data/weatherAUS.RData](https://bitbucket.org/kayontoga/rattle/src/master/data/weatherAUS.RData?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01)


This dataset contains observations of weather metrics for each day from 2008 to 2017. The **weatherAUS.csv** dataset includes the following fields:

| Field         | Description                                           | Unit            | Type   |
| ------------- | ----------------------------------------------------- | --------------- | ------ |
| Date          | Date of the Observation in YYYY-MM-DD                 | Date            | object |
| Location      | Location of the Observation                           | Location        | object |
| MinTemp       | Minimum temperature                                   | Celsius         | float  |
| MaxTemp       | Maximum temperature                                   | Celsius         | float  |
| Rainfall      | Amount of rainfall                                    | Millimeters     | float  |
| Evaporation   | Amount of evaporation                                 | Millimeters     | float  |
| Sunshine      | Amount of bright sunshine                             | hours           | float  |
| WindGustDir   | Direction of the strongest gust                       | Compass Points  | object |
| WindGustSpeed | Speed of the strongest gust                           | Kilometers/Hour | object |
| WindDir9am    | Wind direction averaged of 10 minutes prior to 9am    | Compass Points  | object |
| WindDir3pm    | Wind direction averaged of 10 minutes prior to 3pm    | Compass Points  | object |
| WindSpeed9am  | Wind speed averaged of 10 minutes prior to 9am        | Kilometers/Hour | float  |
| WindSpeed3pm  | Wind speed averaged of 10 minutes prior to 3pm        | Kilometers/Hour | float  |
| Humidity9am   | Humidity at 9am                                       | Percent         | float  |
| Humidity3pm   | Humidity at 3pm                                       | Percent         | float  |
| Pressure9am   | Atmospheric pressure reduced to mean sea level at 9am | Hectopascal     | float  |
| Pressure3pm   | Atmospheric pressure reduced to mean sea level at 3pm | Hectopascal     | float  |
| Cloud9am      | Fraction of the sky obscured by cloud at 9am          | Eights          | float  |
| Cloud3pm      | Fraction of the sky obscured by cloud at 3pm          | Eights          | float  |
| Temp9am       | Temperature at 9am                                    | Celsius         | float  |
| Temp3pm       | Temperature at 3pm                                    | Celsius         | float  |
| RainToday     | If there was rain today                               | Yes/No          | object |
| RISK_MM       | Amount of rain tomorrow                               | Millimeters     | float  |
| RainTomorrow  | If there is rain tomorrow                             | Yes/No          | float  |

Column definitions were gathered from [http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml](http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkML0101ENSkillsNetwork20718538-2022-01-01)

</div>

# Installation
<div id="Section_3">
To run this project, you'll need to have Python installed along with the following libraries:
<ul>
<li>pandas</li>
<li>numpy</li>
<li>scikit-learn</li>
<li>matplotlib</li>
<li>seaborn</li>
<li>requests</li>
<li>jupyter</li>
</ul>
</div>

# Usage
Clone the repository:
            git clone https://github.com/your-username/rain-prediction-australia.git
            cd rain-prediction-australia

<h3>Download the dataset:</h3> Download the dataset from Kaggle and place it in the data/ directory.

<h3>Run the Jupyter Notebook:</h3>

            jupyter notebook
            Open and run the rain_prediction.ipynb notebook to preprocess the data, train the models, and evaluate their performance.

# Modeling
The project involves the following steps:
<ol>
<li>Data Preprocessing: Handling missing values, encoding categorical variables, and feature scaling.</li>
<li>Feature Engineering: Creating new features based on domain knowledge.</li>
<li>Model Training: Training various machine learning models including Logistic Regression, Decision Trees, Random Forests, and Gradient Boosting.</li>
<li>Model Evaluation: Evaluating models using accuracy, precision, recall, F1-score, and ROC-AUC.</li>
</ol>

# Results
The results of the models are compared to identify the best-performing model. The performance metrics for each model are documented in the notebook.

# Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

<ol>
<li>Fork the repository.</li>
<li>Create a new branch (git checkout -b feature-branch).</li>
<li>Commit your changes (git commit -am 'Add new feature').</li>
<li>Push to the branch (git push origin feature-branch).</li>
<li>Create a new Pull Request.</li>
</ol>

# Acknowledgements

<ul>
<li>Thanks to Kaggle for providing the dataset.</li>
<li>This project was inspired by various online tutorials and machine learning resources.</li>
</ul>
