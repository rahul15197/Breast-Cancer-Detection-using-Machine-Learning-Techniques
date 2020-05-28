# Breast Cancer Detection using Machine Learning Techniques
Detection of Breast Cancer using Machine Learning (ML) models and FastAI novel method.

# Table of Contents
- [Introduction](#introduction)
- [Methods](#methods)
- [Dataset](#dataset)
- [Models](#models)
- [Methodology](#methodology)
- [Installation](#installation)
- [Requirements](#requirements)
- [Results](#results)
- [Contribution](#contribution)

## Introduction
Breast cancer affects nearly 10% of the women across
the world and is listed among the top 10 cause of deaths
in women by the World Health Organization (WHO). It is
claimed as the second highest cause of death in women after
lung cancer in the United States by the American Society of
Clinical Oncology (ASCO). Major studies have proved that
the rate of survival in breast cancer is nearly 91% five years
after it was first diagnosed and nearly 84% ten years after
its diagnosis. The high survival rates hence provide the
importance for its early detection.

## Methods
Diagnosis of breast cancer is done by classifying the tumour
as benign or malignant. Three types of diagnostic techniques
are available for the detection of breast cancer. First is the
diagnostic Mammography where additional pictures of
the breast are taken when a woman is experiencing severe
symptoms like new lumps or nipple discharge. Second is
the Ultrasound that uses sound waves to recreate an image
of the breast tissue. Third is an MRI, which is also the
most common diagnosis techniques for breast cancer. It
utilizes the magnetic field to detect cancerous cells in lymph
nodes. Such methods are costly, time-consuming and require
frequent visits to the oncologist.

All these disadvantages have
led the researchers to look more closely at the classification
techniques available in data science to distinguish between
the tumour categories based on patients’ medical records.
This can enhance the prediction and survival rate significantly
so that patients can be informed to take clinical treatment at
the earliest and avoid needless treatments that are otherwise
harmful.

## Dataset
Dataset named as **"Breast Cancer Wisconsin (Diagnostic) Data Set"** available in [UCI (University of California, Irvine) Machine Learning repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)).

The dataset mentioned consists of 569 samples with 32
attributes each. Out of these 32 attributes, one of them is the
classifier output, Benign(B) or Malignant(M) and the other is
the Case ID. Rest 30 attributes are numerical and correspond to
the patients’ medical records. Out of these 569 data points, 212
are malignant tumour cases while the rest are benign tumour
cases.

![count_plot](https://drive.google.com/uc?export=view&id=1JNUxKB-QJ51497yhpNbHQ_iT8QKIRcBv)

Ten real valued attributes used for preparing the model are
described as follows. They have been computed for each cell
nucleus.

The mean, worst and the standard error values were
calculated for each of the 569 samples which resulted in 30
attributes.

![attribute_values](https://drive.google.com/uc?export=view&id=1ZI8Nzg4F4lmYVqvVv6JduWGjVwXvoiVT)

It is named as **"wdbc.csv"**

## Models
We have used Random Forest, K-Nearest neighbor, Logistic
regression, Support Vector Machine, Multi-layer Perceptron
and Neural Network for tabular data using FastAI for the given
classification task at hand.

## Methodology
Dataset analysis was done using count plot followed by correlation of features analysis.  The selected features have
been normalized using the MinMaxScaler of scikit-learn.
This has been done to reduce all the features between
the range 0-1. The MinMaxScaler subtracts the minimum
value and then divides by the original range. This is done
for each attribute, i.e., column wise in the given data.

Predictive Power Score (PPS) and Principle Component Analysis (PCA) are also applied and tested for better accuracy and performance of models.

After this, all ML models were applied. Features and labels were prepared in tabular form of FastAI as the dataset contains numerical values only.

## Installation
```bash
python bdmh_project.py # to run the project without PCA and PPS
python bdmh_project_pps_pca.py # to run the project with PCA and PPS
```
Run BDMH_Project.ipynb and BDMH_Project_PPS_PCA.ipynb in Jupyter or [Google Colab](https://colab.research.google.com/)

## Requirements
Following are the libraries required
* numpy
* pandas
* matplotlib
* Decimal
* seaborn
* fastai
* sklearn
* keras
* tensorflow

## Results
We have applied six different models to solve the presented
classification problem and have compared results for each
model. Within each model four variations have been presented.
* Model without feature selection without cross validation
* Model without feature selection with cross validation
* Model with feature selection without cross validation
* Model with feature selection with cross validation

We have presented FastAI as the novel method for classi-
fication of breast cancer, along with feature selection using
predictive power score.

Model without feature selection without cross validation

![variation1_accuracy](https://drive.google.com/uc?export=view&id=1yK2LFc4qmyQH4nmSZVT3WK09a-eZQ5Zl)

Model without feature selection with cross validation

![variation2_accuracy](https://drive.google.com/uc?export=view&id=1Im9pd6gQ11HfUihqW_NaIjD7EOYwulLG)

Model with feature selection without cross validation

![variation3_accuracy](https://drive.google.com/uc?export=view&id=1x8qBLAsQBP8mT_tAGlygFEjxTwr7fFC2)

Model with feature selection with cross validation

![variation4_accuracy](https://drive.google.com/uc?export=view&id=127kpAi2gR1eQRkSE_JjWnOz0Cy5akDoN)

For detailed process and result with analysis please refer to BDMH_Report.pdf

## Contribution
Project was created by [Rahul Maheshwari](mailto:rahul19027@iiitd.ac.in), [Nikunj Agarwal](mailto:nikunj19093@iiitd.ac.in), [Sumedha Bhatia](mailto:sumedha19129@iiitd.ac) and [Surbhi](mailto:surbhi19055@iiitd.ac.in). Feel free to contact us.


