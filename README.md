# Comparing-ML-Models-to-Predict-Blood-Pressure-Signal-from-PPG-Signal
## Abstract
Coronary artery disease, also called as ischemic heart disease is a major cause of global mortality each year. Hypertension is a major factor contributing to this deadly condition. Arterial Blood Pressure (ABP) is a common indicator of hypertension and is one of the four main vital signs which provides clinical information about the cardiovascular activity. Regular BP monitoring is immensely important for people who suffer from cardiovascular diseases. However, current techniques to measure BP readings are often quite invasive and costly. Sphygmomanometer, a common apparatus to record the BP readings, has a drawback wherein it can be used only in rest. Additionally, people have formed an aversion for cuff-based blood pressure measuring devices. Recently, there have been an extensive study undergoing in this field where the researchers have tried to and succeeded in using Photoplethysmography signal (PPG signal) to obtain Arterial Blood Pressure signal using different Machine Learning and Deep Learning algorithms. In our proposed paper we are trying to analyze if it is feasible to obtain ABP signal from a PPG signal using Symbol Aggregate Approximation method and Transformer models. 

## Dataset
The dataset from UCI contains raw electrocardiogram (ECG), photoplethysmography (PPG), and arterial blood pressure (ABP) signals. The dataset is split to 12 parts to make it easier to load on machines with low memory. This database consists of a cell array of matrices, each cell is one record part. There might be more than one record per patient (which is not possible to distinguish). However, records of the same patient appear next to each other.
In each matrix each row corresponds to one signal channel:
•	PPG signal, FS=125Hz; photoplethysmography from fingertip
•	ABP signal, FS=125Hz; invasive arterial blood pressure (mmHg)
•	ECG signal, FS=125Hz; electrocardiogram from channel II.

For this project, 8 out of 12 mat files were used. 70% of the dataset was used as training set of which 0.1% was used as validation set. Remaining 30% was used as test set.

## Data Pre-processing
Feature Extraction (PPG, ABP and ECG) and Feature Scaling (Normalization) was carried out.

## Model Implementation
BP Prediction from PPG Signal was implemented using Linear Regression model, LSTM Model and Artificial Neural Network Model (ANN) with and without Normalization.

## Evaluation and Result
RMSE, MAE and MAPE with standard deviation was used as evaluation paremeters for the models implemented. ANN outperformed the other two models in terms of the evaluation parameters.
