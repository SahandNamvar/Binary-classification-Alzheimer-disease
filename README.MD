# 🧠 Alzheimer's Disease Prediction - Machine Learning 🧠

**View My Solution on Kaggle**[https://www.kaggle.com/code/sahandnamvar/binary-classification-eda-prediction](https://www.kaggle.com/code/sahandnamvar/binary-classification-eda-prediction)

## Team Members

- **Sahand Namvar**

## Project Introduction

The "Alzheimer's Disease Dataset" from Kaggle provides a comprehensive set of health information for 2,149 patients. The dataset includes a variety of features such as demographic details, lifestyle factors, medical history, clinical measurements, cognitive and functional assessments, symptoms, and a diagnosis of Alzheimer's Disease (AD). These features can offer great insights into the interplay of various factors contributing to AD.

The goal of this project is to apply and compare several machine learning classification algorithms to predict the presence of AD based on the provided data. By leveraging these algorithms, we seek to identify the most effective model for predicting AD status.

### Objectives:

- **Descriptive:** Analyze and visualize the dataset to understand the distribution and relationships among different features.
- **Predictive:** Evaluate various machine learning classification algorithms to predict AD status.
- **Techniques:** Implement and compare the following supervised learning techniques to determine the most accurate and reliable model for binary classification:
  - Decision Tree
  - Random Forest
  - K-Nearest Neighbor (KNN)
  - Logistic Regression
  - Random Forest Classifier
  - Support Vector Machine
  - Gradient Boosting Classifier

## Research Question

How effective are different machine learning classification algorithms in predicting AD based on extensive patient health information? Specifically, which algorithm provides the highest accuracy and reliability for early detection of AD?

**Assumptions** (_Hypothesis_)

1. When symptoms appear after the age of 60, it implies late-onset AD which is the most common form of the disease. Family history of dementia is a known risk factor for developing late-onset AD. Therefore, I expect that family history is a factor contributing to AD. Therefore, it could be highly positively correlated with AD positives. Is that true, given the dataset?

2. Does education level affect AD? :trollface:

## Dataset Details

- **Source:** Kaggle
- **URL:** [https://www.kaggle.com/datasets/rabieelkharoua/alzheimers-disease-dataset](https://www.kaggle.com/datasets/rabieelkharoua/alzheimers-disease-dataset)

### Dataset Features

| No  | Feature                   | Description                                                      |
| --- | ------------------------- | ---------------------------------------------------------------- |
| 1   | PatientID                 | Unique identifier for each patient.                              |
| 2   | Age                       | Ranges from 60 to 90 years.                                      |
| 3   | Gender                    | 0 = Male, 1 = Female.                                            |
| 4   | Ethnicity                 | 0 = Caucasian, 1 = African American, 2 = Asian, 3 = Other.       |
| 5   | EducationLevel            | 0 = None, 1 = High School, 2 = Bachelor's, 3 = Higher.           |
| 6   | BMI                       | Ranges from 15 to 40.                                            |
| 7   | Smoking                   | 0 = No, 1 = Yes.                                                 |
| 8   | AlcoholConsumption        | Weekly units ranging from 0 to 20.                               |
| 9   | PhysicalActivity          | Weekly hours ranging from 0 to 10.                               |
| 10  | DietQuality               | Score from 0 to 10.                                              |
| 11  | SleepQuality              | Score from 4 to 10.                                              |
| 12  | FamilyHistoryAlzheimers   | 0 = No, 1 = Yes.                                                 |
| 13  | CardiovascularDisease     | 0 = No, 1 = Yes.                                                 |
| 14  | Diabetes                  | 0 = No, 1 = Yes.                                                 |
| 15  | Depression                | 0 = No, 1 = Yes.                                                 |
| 16  | HeadInjury                | 0 = No, 1 = Yes.                                                 |
| 17  | Hypertension              | 0 = No, 1 = Yes.                                                 |
| 18  | SystolicBP                | Ranges from 90 to 180 mmHg.                                      |
| 19  | DiastolicBP               | Ranges from 60 to 120 mmHg.                                      |
| 20  | CholesterolTotal          | Ranges from 150 to 300 mg/dL.                                    |
| 21  | CholesterolLDL            | Ranges from 50 to 200 mg/dL.                                     |
| 22  | CholesterolHDL            | Ranges from 20 to 100 mg/dL.                                     |
| 23  | CholesterolTriglycerides  | Ranges from 50 to 400 mg/dL.                                     |
| 24  | MMSE                      | Score from 0 to 30 (lower scores indicate impairment).           |
| 25  | FunctionalAssessment      | Score from 0 to 10 (lower scores indicate greater impairment).   |
| 26  | MemoryComplaints          | 0 = No, 1 = Yes.                                                 |
| 27  | BehavioralProblems        | 0 = No, 1 = Yes.                                                 |
| 28  | ADL                       | Score from 0 to 10 (lower scores indicate greater impairment).   |
| 29  | Confusion                 | 0 = No, 1 = Yes.                                                 |
| 30  | Disorientation            | 0 = No, 1 = Yes.                                                 |
| 31  | PersonalityChanges        | 0 = No, 1 = Yes.                                                 |
| 32  | DifficultyCompletingTasks | 0 = No, 1 = Yes.                                                 |
| 33  | Forgetfulness             | 0 = No, 1 = Yes.                                                 |
| 34  | Diagnosis                 | 0 = No Alzheimer's, 1 = Alzheimer's Disease.                     |
| 35  | DoctorInCharge            | Confidential column with the value "XXXConfid" for all patients. |

## Relevant Domain Information

- Rapid Alzheimer's Disease Diagnosis Using Advanced Artificial Intelligence Algorithms: [https://www.ijisrt.com/assets/upload/files/IJISRT24JUN1915.pdf](https://www.ijisrt.com/assets/upload/files/IJISRT24JUN1915.pdf)
- Early-Stage Alzheimer's Disease Prediction Using Machine Learning Models: [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8927715/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8927715/)
- Classification of Alzheimer's Disease using Machine Learning Techniques: [https://www.scitepress.org/Papers/2019/79499/79499.pdf](https://www.scitepress.org/Papers/2019/79499/79499.pdf)

## Binary Classification Workflow

- **Exploratory Data Analysis (EDA)** - visualize features' relationships & distributions.
- **Data Preprocessing** - Scale cumulative features. Convert categorical features to binary.
- **Model Training & Testing** - Train & test models on the preprocessed data. Select top 10 features with higher importance relevant to the target variable to improve the models.
- **Model Evaluation** - Evaluate the models' performance and plot the Neural Networks' validation graph.

## Dataset Citation

@misc{rabie_el_kharoua_2024,
title={Alzheimer's Disease Dataset},
url={https://www.kaggle.com/dsv/8668279},
DOI={10.34740/KAGGLE/DSV/8668279},
publisher={Kaggle},
author={Rabie El Kharoua},
year={2024}
}
