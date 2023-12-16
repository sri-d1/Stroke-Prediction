
# Stroke Disease Prediction

Stroke occurs when the blood supply to the brain is either interrupted or reduced, typically due to a blockage (ischemic stroke) or the rupture of a blood vessel (hemorrhagic stroke). When deprived of blood, the brain lacks oxygen and nutrients, leading to the death of cells in affected areas. Consequently, the parts of the body controlled by the damaged brain region experience impaired functionality.

Recognized as a medical emergency, stroke demands immediate attention, as brain cells can perish within minutes. Swift and appropriate treatment measures are crucial to minimize brain damage and avert potential complications.

The focus of this machine learning project lies in addressing health concerns related to stroke. The goal is to predict the likelihood of stroke in individuals with specific conditions, considering factors such as age, prevalent diseases (e.g., hypertension, heart disease), and lifestyle choices like smoking. By leveraging machine learning, this project aims to provide valuable insights that can aid in early detection, particularly among those at high risk, fostering awareness and preventing strokes before they become life-threatening


## Language / Libraries
Language: Python

Packages: Sklearn, Matplotlib, Seaborn, imblearn

## DataSet Details
This dataset has been used to predict stroke with . This dataset has:

4088 samples or rows
10 features or columns
1 target column (stroke).

Features in Datasets:

1.Gender: Patient's gender ('Male', 'Female', and 'Other') [str]

2.age : Age of the patient [int]

3.Hypertension: Hypertension or high blood pressure is a disease that puts a person at risk for stroke. 0 if the patient does not have hypertension, 1 if the patient has hypertension. [int]

4.heart_disease: Heart disease is a disease that puts a person at risk for stroke. 0 if the patient does not have heart disease, 1 if the patient has heart disease. [int]

5.ever_married : Describes whether the patient is married or not ('Yes' or 'No') [str]

6.work_type : Type of employment or status ('children' for children, 'Govt_job' for civil servants,
'Never_worked' for those who have never worked, 'Private' or 'Self-employed' for entrepreneurs or freelancers) [str]

7.Residence_type : Condition of residence ('Rural' for rural areas and 'Urban' for urban areas) [str]

8.avg_glucose_level : Average amount of glucose (sugar) in the blood [float]

9.bmi : Body Mass Index to measure the stability of body weight with height. [float]

10.smoking_status : Description of smoking ('formerly smoked' for those who have smoked, 'never smoked' for those who have never smoked, 'smokes' for those who smoke, and 'unknown' for those whose smoking status is unknown) [str]

Target: stroke : Prediction target if the patient has a stroke then 1, otherwise 0 [int]

## PREPROCESSING

1. Only BMI-Attribute had NULL values. Deleted the Null values. 
2. In the gender attribute, there were 3 types - Male, Female and Other. There was only 1 record of the type "other". Deleted the single record.
3. Dummy encoding converting categorical values to one hot encoding.
4. Balancing the dataset using SMOTE as Target value dataset'stroke' was highly imbalanced.


## EDA - Exploratory Data Analysis

1. Plotted plots of each attribute - Analyse trends if any.
2. Plotted relation of target attribute to other attributes to find any correlation.

## MODEL BUILDING

Applied various Machine learning models for predictive analysis

1. LogisticRegression
2. RandomForestClassifier
3. SVC
4. KNeighborsClassifier

  
Accuracies calculated:
1. LogisticRegression : 0.92
2. RandomForestClassifier : 0.975
3. SVC : 0.97
4. KNeighborsClassifier : 0.97
Chosen model - RandomForestClassifier

## License

[MIT](https://choosealicense.com/licenses/mit/)



