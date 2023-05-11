REPOSITORY OUTLINE

"*" A jupyter notebook
"*" A non technical presentation.
"*" CRISP-DM report
"*" README file
"*" SyriaTel Customer churn data
"*" SyriaTel company logo
"*" churn distribution visual

# Phase 3 Project

Another module down--you're almost half way there!

![awesome](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-2-project-campus/master/halfway-there.gif)


![image](https://github.com/Carol-Kambura/Phase_3_Project/assets/119498882/b14694de-f46a-4784-91c6-5589f6d52570)

## Project Overview : syriatel company customer churn analysis project

Using binary classification to build a model that accurately predicts customer churn to help syriatel company identify the factors contributing to the churn and take proactive actions towards retaining their customers


## BUSINESS OVERVIEW

SyriaTel is a telecommunication company based in Syria. The services of the company include voice and data services. Recently, the company has been concerned about the increased rate of customer churn that is resulting to high loss of revenue. The company is looking to outsource a data scientist to help identify the contributing factors that are leading to customer's opting out on the services.

### Business Problem 🤔

### ABOUT DATA

The data comes from SyriaTel and includes their customer information. Tha datasets shows customer's state of residence, telephone numbers and length of the account. From the datasets we can see if a customers has subcribed to an international plan, a voice plan and the number of voice mails they recieve. Additionally the dataset includes how many minutes they spend talking, how many calls they make and how much they are charged during a day, evening and night periods.
*Data Source : https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset

Objectives ✍🏽

👉🏽 This notebook aims to:

- Explore and preprocess the data for binary classification
- Explore different classifier models to help predict the target variable

👩🏽‍💻 Machine Learning models to be explored in this project are:

- KNN Classifier
- Logistic regression
- Decision Trees
- Random forest
(NB: All models will be explored but application will be dependent on the data)

### Research Question
 - What factors influence churn and what patterns are the patterns observed among churners?

### Methods

The project used the CRISP-DM data science process to analyse and create a model best for the churn analysis. All the data science steps are described in the CRISP-DM.
Report:

Steps followed:

### Data Preparation
      1. Importing relevant packages i.e. Pandas, Matplotlib, Seaborn, Scipy, Sklearn and Statsmodel
      
      2. Data extraction:
          - Dataset `churn_telcom.csv`
          
     3. Data Cleaning
          - Dropping columns
          
     4. Data Wrangling
         - Indexing data
         - Dealing with outliers
         - Data standardization and normalization
         - Dealing with categorical data
         
### Data Modelling

      1. KNN Classiffier  
      
### Results

This classifiers had the lowest perfomance based on precision, recall and F1 scores. Observing a recall score of 19.31% means that the model has a high rate of producing false negative churns and could only correctly 19.31% positive instances (i.e., churners) out of all instances classified as positive by the model. 

Model 1: KNN Confusion Matrix

![image](https://github.com/Carol-Kambura/Phase_3_Project/assets/119498882/51deae13-1ef0-4c69-89ce-e47f24ddee29)

Logistic Regression findings

The recall score for the clssifier was 28% which also indicated that the clasifier perfomed poorly on correctly predicting customer churn, thus the classifier could not be adopted for this project.

Model 2: logistic regresion confusion matrix

![image](https://github.com/Carol-Kambura/Phase_3_Project/assets/119498882/22ae1f89-0868-40f2-95a7-e823edfa2800)

Model 3: Decision Tree

Among all the models explored, Decision tree performed the best, we observed an accuracy of 92.9% and the highest recall score of 78.4% with a precision of 70.4% . The model is therefore able to identify chuners the AUC-ROC score of 86.70% indicates that the model is able to distinguish between positive and negative instances.

decision tree confusion matrix

![image](https://github.com/Carol-Kambura/Phase_3_Project/assets/119498882/06460066-ed33-487e-8f7e-3ce65bccb50e)

Model 3: Random Forest 

The model did perform reasonably well with a high accuracy and AUC - ROC score of 86.85 with a precision and recall score of 82.71% and 76.13% respectively. This means that the model is able to identify a large proportion of churners but is also making some false positive. However, it is performing well in distinguishing between positive and negative instances

Model 3: Random forest confusion matrix

![image](https://github.com/Carol-Kambura/Phase_3_Project/assets/119498882/789b0ac8-5422-4319-8af8-3865752c1455)


### CONCLUSION

Based on the findings, the business conclusion can be drawn as follows:

- Importance of Recall: In the context of predicting customer churn, the focus was placed on optimizing for Recall. By prioritizing Recall, the goal was to minimize the number of customers who are incorrectly classified as non-churners.
- Best Model: Among the models explored was the decision tree Classifier. The model was able to identify 78% of the customers who were likely to churn with an accuracy score of 92.8%. However, the Random forest classifier could also be used as there wasn't such significance difference between the 2 models in performance.
- The top 3 factors that were observed to influence the rate of customer churners included total day charge, customr service calls and number oof voice mail messages.
- Predicting customer churn rate is an ongoing process, and it is important to continuously refine and improve the model. Regularly monitoring the model's performance, collecting new data, and incorporating feedback from business stakeholders can lead to better predictions and more accurate identification of customers who are at risk of churning

### BUSINESS RECOMMENDATION

Determine the unique needs for the following customers and develop strategic plans for each group of customers;

- SyriaTel communication should conduct bi-annual and annual annalysis of their customer churn rate to identify patterns
- To reduce customer churn, the company should review the charge rate for the day calls as total day charge is the most influencial predictor for churn.
- SyriaTel should improve the customer service calls through attentive listening to customers issues, feedbackd and complains and also through offering timely solutions for the same.
- SyriaTel company should reach out to the customers with high numbers of voicemail messages to determine the cause for the voicemail messages surge and know how to adress the same.
- SyriaTel should come up with a tailormade data and voice plan products for the international customers based on their unique needs.
