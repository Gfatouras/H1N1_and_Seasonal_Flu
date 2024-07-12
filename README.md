# Predicting Vaccination Likelihood

## Overview

This repository contains the code and data used to analyze vaccination probabilities. The primary goal of this project is to extract and evaluate various features from our dataset and use them to create models to predict whether or not an individual received an H1N1 or seasonal vaccine.

## Business Problem

The project aims to predict vaccination outcomes based on extracted features from a dataset. By analyzing these features, we develop machine learning models to predict the likelihood of an individual receiving either the H1N1 or seasonal flu vaccine.

### Table of Contents

- [Overview](#overview)
- [Business Problem](#business-problem)
- [Data Sources](#data-sources)
- [Installation](#installation)
- [Analysis and Results](#analysis-and-results)
  - [Feature Extraction](#feature-extraction)
  - [Model Creation](#model-creation)
  - [Evaluation](#evaluation)
- [Conclusion](#conclusions-and-recommendations)

## Data Sources

We used data from the National 2009 H1N1 Flu Survey dataset, which includes anonymized features related to individuals' demographics, health-related variables, and past behaviors regarding vaccination. https://www.cdc.gov/nchs/index.htm

## Installation

To run the project, follow these steps:

1. Clone the repository: git clone [https://github.com/Gfatouras/H1N1_and_Seasonal_Flu.git](https://github.com/Gfatouras/H1N1_and_Seasonal_Flu)
   
## Analysis and Results

### Feature Extraction

Initial steps involved extracting 35 relevant features from the dataset, including demographic information, health-related variables, and opinions related to vaccines. Feature selection techniques were applied to identify the most predictive variables.

### Model Creation

Multiple machine learning models were developed using the extracted features. These models include but are not limited to:
- Logistic Regression
- Random Forest
- LightGBM
### Evaluation

Models were evaluated based on various metrics such as accuracy, confusion matricies, and ROC-AUC scores. Cross-validation and hyperparameter tuning techniques were employed to optimize model performance. 
Below are the results of our baseline logistic regression model with no pre-preocessing or hyperparameter tuning.

![image](https://github.com/Gfatouras/Phase3/assets/165408353/fe1c998b-b7da-4c04-8abc-afcb1b3d710a)



Below are the results of our LightBGM model, which resulted in an average ROC AUC score of 0.868.

![image](https://github.com/user-attachments/assets/7121e13a-8b15-4542-8b03-7dfc1e14fe17)

Below is the ROC AUC improvement from our baseline model compared to our LightGBM model.

![image](https://github.com/user-attachments/assets/337757be-25f8-45f1-bbe0-650160060063)


Below are the ROC AUC scores from each model, hyperparameter tuning was performed on all models except for our baseline. 

![image](https://github.com/user-attachments/assets/4945fd40-5cc2-498a-afe4-15fa5eb15951)

Below are the 10 most important socioeconomic features for our LightGBM model. This was obtaiend by plotting the LGBM model weights and selecting only socioecomomic features. These 10 features were very significant for our model's decision making process.

![image](https://github.com/user-attachments/assets/9c7234c1-794c-4113-8fe9-31e0550edda5)



# Conclusions and Recommendations

Based on the comprehensive analysis of the 2009 H1N1 Flu Survey data, we have developed a predictive model to determine the likelihood of individuals receiving H1N1 and seasonal flu vaccinations. The conclusions drawn from this study, coupled with actionable recommendations, are aimed at improving vaccination rates and public health outcomes.

**Key Findings:**

1. **Determinants of Vaccination:**
   - **Education and Age:** Individuals with lower education levels and younger age groups are less likely to receive vaccinations.
   - **Health Concerns:** Concerns about vaccine side effects and perceived effectiveness significantly impact vaccination decisions.
   - **Healthcare Access:** Those without health insurance and individuals who do not receive a doctor's recommendation are less likely to get vaccinated.
   - **Perception of Risk:** People who perceive a lower risk of not getting the seasonal vaccine are less likely to be vaccinated for both H1N1 and seasonal flu.

2. **Model Performance:**
   - The Light Gradient Boosting Model (LightGBM) emerged as the top performer with an ROC AUC score of 0.8679, indicating high predictive power.
   - The LightGBM model has very high specificity, as it predicts true negatives with the highest accuracy.
   - The importance of preprocessing techniques, such as encoding missing numerical data and using SMOTE for class imbalance, was highlighted in improving model performance.

3. **Socioeconomic Factors:**
   - Socioeconomic factors like health insurance status, occupation, and age group significantly influence vaccination likelihood. These insights can help target interventions more effectively.

**Recommendations:**

1. **Free Vaccination Programs:**
   - **Health Insurance:** Provide free vaccines to individuals without health insurance to remove financial barriers.
   - **Targeted Campaigns:** Conduct vaccination drives in communities with low vaccination rates, focusing on areas with higher populations of uninsured individuals.

2. **Public Awareness and Education:**
   - **Informing the Public:** Increase public awareness about the benefits and safety of vaccines through health worker training and targeted marketing campaigns.
   - **Doctor's Role:** Train healthcare providers to emphasize the importance of vaccination recommendations to their patients, especially for H1N1.

3. **Addressing Vaccine Hesitancy:**
   - **Risk Communication:** Develop communication strategies to address concerns about vaccine side effects and effectiveness.
   - **Engagement with Younger Populations:** Create specific outreach programs targeting younger age groups to educate them about the importance of vaccination.

4. **Policy and Healthcare Integration:**
   - **Electronic Health Records:** Integrate predictive models into electronic health records to help healthcare providers identify and engage with patients less likely to be vaccinated.
   - **Policy Development:** Use the insights from the predictive models to inform policymakers about potential outbreak locations and to design effective vaccination strategies.

**Future Steps:**

- **Data Expansion:** Utilize historical and real-time data to enhance the model's accuracy and predictive capabilities.
- **Survey Updates:** Conduct more frequent surveys to keep the model's predictions relevant and accurate.
- **Broader Applications:** Develop websites and visual tools to communicate data and predictions to the public, and leverage these insights for targeted marketing by pharmaceutical companies.

By implementing these recommendations, we can improve vaccination rates, prevent disease outbreaks, save lives, and create a healthier, more productive society. Predictive modeling serves as a powerful tool to guide effective vaccination strategies and improve public health outcomes on a broad scale.

# Contact
- Greg Fatouras
  + https://github.com/Gfatouras
  + https://www.linkedin.com/in/gfatouras/
  + fatourasg@gmail.com

- Chisum Lindauer
  + [https://github.com/minerva-ds/](https://www.linkedin.com/in/chisum-lindauer/)
  + https://www.linkedin.com/in/chisum-lindauer/
  + chisum@atrixtech.com

