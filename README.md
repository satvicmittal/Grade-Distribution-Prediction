# Grade-Distribution-Prediction

Predicting the Grade Distribution of the final exam on the basis of the historical data of practice exam.
For this project, anonymised test results of 3 cohorts are utilized.

## Description of the python files:

1. Exam_Attempt_Cleaning_Final.ipynb : Cleans the attempts log by students (Practice and final exam)
2. Data_Generation_Model : Feature Engineering code which converts the attempts details into a format that could be used to train our model. It converts the the data into the format {'No of Students', 'No of Question', 'Total Marks', 'Exam Duration', 'Average Difficulty Index', 'Average Time Taken', 'Mean', 'Standard Deviation'}. For Training, attempts are picked at random for each student which then corresponds to a new data point. For test data we we convert the results from 3 cohorts into 3 datapoints in the format mentioned above.
3. Grade_Distribution_Model : Linear Regression is implemented to predict the mean and standard deviation of the grade distrbution. Ridge Regression is implemented to identify the key predictors and analyse the interations between the features.

## Instructions to Run the code

1. Run 
