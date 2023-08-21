# Medical-Insurance-Price-Prediction
## Task:
Build a Machine Learning model to predict medical insurance prices.</br> This comes under **Supervised learning** as we have provided labelled data. As in this problem, we need to predict the continuous numbers i.e. prices, we use regression models to predict the value. We have built a Linear Regression model for this.

## Dataset:
The dataset contains information about the insurance policies bought by individuals. The dataset contains 1338 records of different policies with 7 features each about them. The features are:</br>
. age: age of the primary beneficiary</br>
. sex: insurance contractor gender, female, male</br>
. bmi: Body mass index, providing an understanding of the body, weights that are relatively high or low relative to height, an objective index of body weight (kg / m ^ 2) using the ratio of height to weight, ideally 18.5 to 24.9</br>
. children: Number of children covered by health insurance / Number of dependents</br>
. smoker: Smoking</br>
. region: the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.</br>
. charges: Individual medical costs billed by health insurance</br></br>
Source: https://www.kaggle.com/datasets/mirichoi0218/insurance
## Steps Involved:
### Import Dependencies
Libraries needed to achieve the result are: </br>
. pandas</br>
. numpy</br>
. matplotlib.pyplot</br>
. seaborn</br>
. LinearRegression from sklean.linear_model</br>
. train_test_split from sklearn.model_selection</br>
. metrics from sklearn</br>
### Data Collection and Analysis
. Use read_csv function from pandas to import the dataset.</br>
. Use the function such as shape, describe, head, and info to know more about the data set</br>
. Check for the missing value using the isnull function</br>
### Data Visualization
. Created distribution and count plots for all the features using **Seaborn** and **Matlplotlib** libraries.
### Data Processing
. There are 3 Categorical Columns in our dataset that is 'sex', 'smoker' and 'region'. We converted all the 3 to numerical values such that for </br>
sex = male : 0, female : 1,</br>
smoker = yes : 0,no : 1, </br>
region = southeast : 0,southwest : 1,northeast : 2,northwest : 3</br>
. Finally, splitting the dataset into features and target. The target will contain the column **charges** and the feature will contain the rest of the column except charges.
### Model Training and Evaluation 
. Split the dataset into training and test data. We have taken 20% of the for test purposes and the rest 80% for the training.</br>
. We have used Linear Regression Algorithm to predict the result. </br>
. Prediction and Evaluation are being carried out for both trained and test data.</br>
. **Linear Regression**: </br>
R squared value for training data:  0.751505643411174 </br>
R squared value for test data:  0.7447273869684077</br>

### Build a predictive system
. Take some random data from the X dataset.</br>
. Transform it to numpy array then reshape it into a 2D array.</br>
. Feed it to the created model.</br></br></br></br>

Reference: Project 11. Medical Insurance Cost Prediction using Machine Learning with Python | ML Projects, Siddhardhan, https://www.youtube.com/watch?v=ntBa7YKc9XM&list=PLfFghEzKVmjvuSA67LszN1dZ-Dd_pkus6&index=11

