* Description of data:  
  - A cohort study (subjects were recruited at birth and followed for 25 years).
  - A high dimensional data (more than 50 relevant variables)
  - Dental examinations were performed at age 5, 9, 13, 17 and 23. 
  - Independent variables data were collected at every 6 months. 
  - Almost 2000 subjects were recruited at birth but only about 336 subjects were retained after 25 years (a lot of missing data).
  
ABSTRACT 
Introduction and Aims: Dental caries is a chronic, multifactorial disease influenced by biological, behavioral, and environmental factors across the life course. While traditional trajectory analyses have been used to classify caries progression, no prior studies have applied machine learning to predict caries trajectories from childhood to early adulthood. This study uses unsupervised machine learning to identify distinct trajectory groups and applies supervised to predict risk-group membership based on behavioral, dietary, fluoride, and sociodemographic variables.

Methods: This study utilized data from the Iowa Fluoride Study. Caries trajectories were identified using K-means for Longitudinal Data (KmL) based on dental examinations at ages 9, 13, 17, and 23. The optimal number of groups was selected using the Calinski–Harabasz criterion and clinical relevance. Trajectory group membership served as the outcome in supervised models trained on sociodemographic, fluoride intake, dietary, and behavioral variables. Ordered Multinomial Logistic Regression, Least Absolute Shrinkage and Selection Operation, Gradient Boosting Machine, Extreme Gradient Boosting and Neural Network were applied. Class imbalance was addressed with Synthetic Minority Over-sampling Technique.

Results: Three caries trajectory groups were identified: low (70.5%), medium (21.1%), and high (8.4%). XGBoost outperformed Ordered Multinomial Logistic Regression, LASSO, GBM, and NNET, with 85.9 % accuracy and a Brier score of 0.21. Precision for the low-, medium-, and high-risk groups was 80.0%, 81.0%, and 96.0%, respectively; recall was 75.5%, 82.7%, and 97.5%. Top predictors included sex, maternal education, composite SES, fluoride intake, and consumption of milk, sugar-free beverages, sugar-sweetened beverages, and 100% juice.

Conclusion: This study is the first to combine machine learning models to predict caries trajectories from childhood to adulthood with high accuracy. Future work should validate findings with additional clinical data from diverse populations.

Clinical Relevance: Predicting dental caries trajectories using machine learning could enable early identification of high-risk individuals and inform targeted, age-appropriate preventive interventions.

