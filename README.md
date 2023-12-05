# patient-survival-prediction

Data Description:

1) ID_Patient_Care_Situation: Care situation of a patient during treatment
2) Diagnosed_Condition: The diagnosed condition of the patient
3) ID_Patient: Patient identifier number
4) Treatment_with_drugs: Class of drugs used during treatment
4) Survived_1_year: If the patient survived after one year (0 means did not survive; 1 means survived)
5) Patient_Age: Age of the patient
6) Patient_Body_Mass_Index: A calculated value based on the patient’s weight, height, etc.
7) Patient_Smoker: If the patient was a smoker or not
8) Patient_Rural_Urban: If the patient stayed in Rural or Urban part of the country
9) Previous_Condition: Condition of the patient before the start of the treatment ( This variable is splitted into 8 columns - A, B, C, D, E, F, Z and Number_of_prev_cond. A, B, C, D, E, F and Z are the previous conditions of the patient. Suppose for one patient, if the entry in column A is 1, it means that the previous condition of the patient was A. If the patient didn't have that condition, it is 0 and same for other conditions. If a patient has previous condition as A and C , columns A and C will have entries as 1 and 1 respectively while the other column B, D, E, F, Z will have entries 0, 0, 0, 0, 0 respectively. 
10) The column Number_of_prev_cond will have entry as 2 i.e. 1 + 0 + 1 + 0 + 0 + 0 + 0 + 0 = 2 in this case. )
11) Feel free to google 'Diagnose' and 'Body Mass Index' if you don't know about these terms.
Evaluation Criteria
Submissions are evaluated based on the F1 Score calculated using the predicted value of your model and true value of of Survived_1_year on the unseen new test dataset mentioned under submission guidelines.

Basic Steps That You May Follow
1) The steps mentioned here are basic steps to get you started to solve the problem. You are free to use some techniques other than mentioned below to improve your model performance.

2) Load the necessary libraries such as pandas, numpy, scikit-learn and more if any
3) Load your dataset and perform exploratory data analysis to identify any patterns in the dataset
4) You may fill mssing values if any (use mode for categorical column and mean/median for numerical columns). If there are no missing values, you may skip this step. Perform any other data preprocessing step that you think is required.
5) Separate Input Variables and Target variable
6) Split the dataset pharma_data into train set and test set. Now what is this pharma_data? - don't worry, just scroll up to dataset section above, we have declared the name of our dataset as pharma_data.
7) Build a Model (You have to decide which model to use)
8) Predict the target variable for your own test dataset created in step 5 and check the model performance.
9) Not happy with your model performance? It is alright, you can try to optimise the model further to improve the performance of your model.


