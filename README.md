# Enhanced Post-Prandial Glycemic Response Prediction in Type 2 Diabetes with a Comprehensive Deep Learning Approach.

This work is published in *Journal name* (doi link)  
This repository contains a collection of codebook that we use to analyze data and develope the models for PPGR prediction. 
## Introduction  
Using data from **2 cohorts** totalling **88 participants**, we developed an algorithmic framework, utilizing multi-modal deep learning predictor, to precisely predict individuals' post-prandial glycemic responses(PPGR).  

Our study workflow is consisted of 4 phases as follow.  
(1) Data collection & analysis  
(2) Model development   
(3) Model evaluation  
(4) Model interpretation  

Our codebook open the code for data analysis (risk factor analysis and subgroup analysis) and DNN model development, evaluation and interpretation.
![workflow](https://github.com/user-attachments/assets/c6256326-1142-413d-b78c-e2a05846afdc)

## Prerequisites
The tool was developed using the following dependencies: 
* Python 3.11.7.  
* Scipy 1.13.0.   
* scikit-bio 0.5.8.   
* matplotlib 3.8.4.   
* seaborn 0.12.2.   
* tensorflow 2.12.0.   
* xgboost 1.7.6.   
* umap 0.1.1.  
* scikit-learn 1.4.1.   
* shap 0.44.1.
* PyComplexHeatmap 1.6.2.  

## Data preparation
The detailed data collection and preprocessing procedures are descripted in our **supplementary information** (doi link)  
To replicate this implementation, you should prepare the following data:  
1. Merged data (per meal) of *meal data* and *CGM recording* 
    1. *Meal data* including nutritional composition and meal timing
    2. *CGM recording* (Record must be included from 30 minutes before meal to 4 hours after meal)
2. 16s microbiome data (taxonomic mapped read count profile)
3. clinico demographic data (e.g., Age, BMI, HbAc1)
4. medication usage

## Data analysis
The data analysis process consists of two stages:  
### 1. Causal inference analysis
All code related to Causal inference analysis is under <code>./code/causal_inference_analysis.jpynb</code>.
