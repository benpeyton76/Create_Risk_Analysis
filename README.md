# ***Create Risk Analysis***


## ***Overview:***
In this module, Supervised Machine Learning techniques are used to train and evaluate models with unbalanced classes. Supervised Learning is a way of creating artificial learning by a computer. It uses algorithms to "train" a computer to sort through input data that has been designated to a predetermined, particular output. This analysis will focus on the real-life issue of credit card risk. By reading in the supplied dataset, different techniques will be used to determine which applicants fall into a high or low risk category. Using the RandomOverSampler and SMOTE algorithms, the data will be oversampled, then undersampled using the  ClusterCentriods algorithm. Next, the SMOTEEN alogrithm will use the oversampling and undersampling techniques to combine the data. By using models that reduce bias, the BalancedRandomForestClassifier and EasyEnsembleClassifier algorithms will predict credit risks.


## ***Results:***

  ***Accuracy score*** is a way to validate a model's performance, but should not be used as a performance metric.
  
  ***Precision*** or positive prediciton value, is a measure of how reliable a positive classification is.
  
  ***Recall*** or sensitivity, is the number of true positives and the number of false negatives. The recall is intuitively the ability of the classifier to find   all the positive samples. The best value is 1 and the worst value is 0.
  
  
- ***Naive Random Oversampling:***
  
  By using the RandomOverSampler algorithm, we are able to calculate the balanced accuracy score which is 67%. Then use confusion matrix to determine the number   of actual and predicited high and low number of applicants. 
  <img width="1027" alt="Mod17deliveralbe1a" src="https://user-images.githubusercontent.com/87077325/149365605-8914aee2-892b-4e1c-8614-4862f9c1c227.png">

 
  
  The precision and recall scores are shown below:
  <img width="728" alt="Mod17deliveralbe1b" src="https://user-images.githubusercontent.com/87077325/149365741-9780dae4-4227-41ba-8e25-0b768a26c97a.png">

  The overall predicted score is 99% while the recall score is 61%.
  
  
- ***SMOTE Oversampling:***
  
  By using the SMOTE algorithm, we are able to calculate the balanced accuracy score which is 66%. Then use confusion matrix to determine the number of actual     and predicited high and low number of applicants.
  <img width="1018" alt="Mod17e" src="https://user-images.githubusercontent.com/87077325/149370359-3256264a-1ff8-4f9e-9b07-e7804740df84.png">

  
  The precision and recall scores are shown below:
  <img width="734" alt="Mod17f" src="https://user-images.githubusercontent.com/87077325/149370538-da95d1bd-0c29-4638-8ea1-e77f3aa98cd4.png">

  The overall predicted score is 99% while the recall score is 69%.
  
- ***Undersampling using ClusterCentroids:***

  By using the ClusterCentroids algorithm, we are able to calculate the balanced accuracy score which is 66%. Then use confusion matrix to determine the number     of actual and predicited high and low number of applicants.
  <img width="1037" alt="Mod17g" src="https://user-images.githubusercontent.com/87077325/149371490-adf0c6c8-7022-44bb-9e04-1117ed13f5a6.png">
  
  The precision and recall scores are shown below:
  <img width="740" alt="Mod17h" src="https://user-images.githubusercontent.com/87077325/149371559-904b312d-9b87-4db6-99fd-90bad88bef16.png">
  
  The overall predicted score is 99% while the recall score is 69%.
  
- ***SMOTEENN:***

  By using the SMOTE algorithm, we are able to calculate the balanced accuracy score which is 64%. Then use confusion matrix to determine the number of actual     and predicited high and low number of applicants.
  <img width="1031" alt="MOD17i" src="https://user-images.githubusercontent.com/87077325/149373016-798caa9f-3c49-4392-b23f-9216413b7300.png">
  
  
  The precision and recall scores are shown below:
  <img width="773" alt="Mod17j" src="https://user-images.githubusercontent.com/87077325/149373115-16e1dc4e-bfd5-4866-8cc1-d86b5fc06a18.png">

  The overall predicted score is 99% while the recall score is 57%.
  
- ***BalancedRandomForestClassifier:***

  By using the BalancedRandomForestClassifier algorithm, we are able to calculate the balanced accuracy score which is 78.8%. Then use confusion matrix to         determine the number of actual and predicited high and low number of applicants.
  <img width="1023" alt="Mod17k" src="https://user-images.githubusercontent.com/87077325/149374333-b5c00aa9-7b93-4888-b35b-1f321b2a2978.png">


  The precision and recall scores are shown below:
  <img width="724" alt="Mod17L" src="https://user-images.githubusercontent.com/87077325/149374413-55694026-0b3c-4f52-aad6-cf583bfbf48c.png">
  
  The overall predicted score is 99% while the recall score is 87%.
  
- ***EasyEnsembleClassifier:***
  
  By using the EasyEnsembleClassifier algorithm, we are able to calculate the balanced accuracy score which is 78.8%. Then use confusion matrix to                 determine the number of actual and predicited high and low number of applicants.
  <img width="877" alt="Mod17M" src="https://user-images.githubusercontent.com/87077325/149375821-e015edfe-582a-4f3d-bf2d-4dabfd365a2c.png">
  
  
  The precision and recall scores are shown below:
  <img width="755" alt="Mod17N" src="https://user-images.githubusercontent.com/87077325/149376067-407cbb8a-5c9c-414d-a654-d15f763895c6.png">

  The overall predicted score is 99% while the recall score is 87%.


## ***Summary:***
 As the graphics above show, the algorithms in the oversampling, undersampling, and combined techniques have lower balanced accuracy, precision, and recall       scores. The RandomOverSampler algorithm has a balanced accuracy score of 67% and have a precision and recall scores of 99% and 61% respectively. The SMOTE and   ClusterCentriods algorithms both have a balanced accuracy score of 66% and have a precision and recall scores of 99% and 69%. The SMOTEENN algorithm has a       balanced accuracy score of 64% and have a precision and recall scores of 99% and 57%. The BalancedRandomForestClassifier and EasyEnsembleClassifier algorithms, which are overall more beneficial due to the robustness of the algorithms, both have   a balanced accuracy score of 78.8% and have a precision and recall scores of 99% and 87% respectively. Based on the overall scores, using BalancedRandomForestClassifier and EasyEnsembleClassifier algorithms appear to be more useful in predicting credit card risks. 
