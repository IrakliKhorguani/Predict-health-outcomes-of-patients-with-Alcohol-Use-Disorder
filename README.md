# Data Science project to predict health outcomes of patients with Alcohol Use Disorder admitted in Intensive Care Unit

## Introduction

In this project, the objective is to predict health outcomes of patients with Alcohol Use Disorder (AUD), who are admitted in Intensive Care Unit (ICU).

Alcohol is one of the most commonly abused addictive substances in the general population, that causes millions of deaths, and is legal to buy and consume in most of the countries. People with AUD can’t stop or control their alcohol consumption, and AUD is considered as a brain disorder. Patients with AUD have higher risks of comorbidities, serious illness and death, and this is why an early intervention and prognosis for severity of illness is highly important to improve treatment and survival rates of AUD patients. I want to focus on the prediction of people’s survival, when they are admitted to the Intensive Care Unit (ICU). The main idea is trying to strengthen medical care for those less likely to survive, and help them survive. But it can be used to increase doctor’s knowledge about the chances of survival of those patients, and so better inform and support families and relatives in this difficult process.

First, I will explore the dataset in order to understand each feature by conducting feature engineering and exploratory data analysis (EDA). Then I will build and train various machine learning models and evaluate them in order to have the most accurate prediction.

## Data
The data used in our report is entirely extracted from the Medical Information Mart for Intensive Care (MIMIC-III), a freely-available database comprising deidentified healthrelated data from patients who were admitted to the critical care units of the Beth Israel Deaconess Medical Center. This database was co-developed by the Laboratory for Computing Physiology at MIT and Philips Healthcare, containing 26 tables storing data such as vital signs, demographics, and survival for more than 40,000 ICU patients from years ranging from 2001 to 2012. This database is widely used in academic discourse for training models to predict medical outcomes for patients.

The variables in this data frame are defined as:

Variable       | Description
-------------- | ------------------------------------------------------------------
subject id | Unique identifier which specifies an individual patient - hadm id A single patient’s admission to the hospital
icustay id | ID which defines a single ICU stay - gender Patient's gender - age Patient's age - ethnicity Patient's ethnicity
los hospital | Length of stay at hospital Days (in Days)
los icu | Length of stay at ICU (in Days)
first icu stay | Flag (1) if it is the patient's first icu stay
sofa | Sequential Organ Failure Assessment (SOFA) - mortality prediction score
sapsii | Simplified Acute Physiology Score - severity of disease classification
congestive heart failure | Flag (1) if the patient has congestive heart failure
hypertension | Flag (1) if the patient has hypertension
liver disease | Flag (1) if the patient has liver disease
fluid electrolyte | Flag (1) if the patient has fluid electrolyte
coagulopathy | Flag (1) if the patient has coagulopathy
chronic pulmonary | Flag (1) if the patient has chronic pulmonary disease
admittime| Date and time the patient was admitted to the hospital
deathtime | Date and time of in-hospital death for the patient
glucose | Glucose level (mmol/L)
platelet | Platelet count ($10^3$/𝜇L)
ast | Aspartate aminotransferase measurement (U/L)
alt | Alanine aminotransferase measurement (U/L)
mcv | Mean corpuscular volume (𝜇m$^3$)
rdw | Red cell distribution width (%)
wbc |White blood cell count K/uL
hemoglobin | Hemoglobin measurement (g/dL) 
