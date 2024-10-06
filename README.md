# classification-challenge

## Description
In this project, we worked on improving the email filtering system for an Internet Service Provider (ISP). The goal was to accurately detect spam emails using a dataset provided to us. We created and compared two machine learning models: a **Logistic Regression model** and a **Random Forest model**.

## Table of Contents
- [Description](#description)
- [Steps](#steps)
- [Results](#results)
- [Usage](#usage)
- [Credits](#credits)

## Steps
> What we did step-by-step...
1. **Data Preparation**: We started by reading the dataset into a Pandas DataFrame. The dataset contained information about emails, labeled as either spam or not spam.

2. **Data Splitting**: We split the data into training and testing sets to evaluate our models properly.

3. **Feature Scaling**: We scaled the features using StandardScaler to ensure that our models performed optimally.

4. **Model Creation**: We created two models:
   - **Logistic Regression**: This model assumes a linear relationship between the features and the target variable.

   - **Random Forest**: This model uses multiple decision trees to capture complex patterns in the data.

5. **Model Evaluation**: We evaluated both models using accuracy scores and other metrics like precision, recall, and f1-score.

## Results
- **Logistic Regression**: The model performed well with an accuracy score of `0.9427`. It was good at identifying legitimate emails but slightly less effective at catching spam.

<br>
<p align="center"> 

|                | Predicted Not Spam [0] | Predicted Spam [1] |
|----------------|-------------------------|--------------------|
| Actual Not Spam [0] | 678                     | 31                 |
| Actual Spam [1]     | 56                      | 386                |
</p>

___

- **Random Forest**: This model performed even better with the same accuracy score of `0.9427` but had higher precision, recall, and f1-scores. It was more effective at catching spam emails while still accurately identifying legitimate ones.

<br>
<p align="center"> 

|                | Predicted Not Spam [0] | Predicted Spam [1] |
|----------------|-------------------------|--------------------|
| Actual Not Spam [0] | 678                     | 31                 |
| Actual Spam [1]     | 39                      | 403                |
</p>

___
<br>

The **Random Forest** model outperformed the **Logistic Regression** model, confirming our initial prediction that it would handle the complex patterns in the data better.

## Usage
1. Clone the repository `git clone https://github.com/rune-encoder/classification-challenge.git`

2. Navigate to the project directory `cd classification-challenge`

3. Open the Jupyter Notebook `jupyter notebook spam_detector.ipynb`

## Credits
Starter code for this assignment was provided by [edX bootcamp](https://www.edx.org/boot-camps).

Dataset: [spam-data.csv](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv)