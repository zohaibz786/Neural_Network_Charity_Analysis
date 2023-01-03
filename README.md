# NEURAL_NETWORK_CHARITY_ANALYSIS

## OVERVIEW
The aim of this machine learning project was to build a classifier that can accurately predict whether a charity will have a successful outcome if they fund a particular applicant. To accomplish this task, we extensively explored the use of neural networks.

## RESULTS

### BEFORE OPTIMIZATION

- **Data preproccessing**
the target variable for our model is the column `IS_SUCCESSFUL` column. In this first attempt we dropped the columns `EIN` and `NAME`.
This left us with 10 columns, the `IS_SUCCEFFUL` target column and 9 columns to be used as features for our model.

- **Compiling, Training, and Evaluating the Model**
In this first attempt we used a model with two hidden layers of 80 neuros and 30 neurons, respectively, and the same activation function **ReLU** and 100 epochs. This resulted in an accuracy of 72%.

![firstAttempt](/Images/results1.PNG)

### AFTER OPTIMIZATION

In order to achieve an accuracy greater than 75% we dropped only the `EIN` column and applied bucketing on the `NAME`column. We also used three hidden layers of 100 neurons, 30 neurons and 10 neurons, respectively, for the second and third hidden layers we used the **sigmoid** activation function. The epochs number wasn't changed. This resulted in an accurcay of almost 79% which successfully met our expected value. 

![firstAttempt](/Images/results2.PNG)

## SUMMARY 

In this project, we used neural networks to build a classifier that could accurately predict the likelihood of a successful outcome for charities that funded particular applicants. The classifier was trained on a dataset of previous funding decisions and their outcomes, and was able to achieve an accuracy of 78.9% when tested on a separate set of data. This high level of accuracy allows charities to make more informed funding decisions, increasing the chances of a successful outcome for both the charity and the funded applicant. Overall, the use of neural networks proved to be an effective method for building a classifier that can accurately predict the success of charitable funding decisions.