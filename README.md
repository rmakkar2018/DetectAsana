# DetectAsana

# Code folder
The Code folder contains the **DetectAsana_ML_Project.ipynb** file with the implementation of various Machine Learning Algotirhm's on PUC-RIO dataset for training and pre-processing of data. 

In the Feature Extraction Section:
Apart from the existing features in PUC-RIO dataset, we have manually extracted other features.We calculated norm=sqrt(x^2 + y^2 + z^2), pitch=tan_inverse(y/(x^2+z^2)) and roll=tan_inverse(-x/z) and added those to the features.

In the Resampling and Feature Selection:
Class weights: We have also used Class weights technique to handle dataimbalance which punishing classes with more samples lesser for each misclassification.
Oversampling: We have used the ADASYN(Adaptive Synthetic) sampling to deal with data imbalance.
Undersampling: We have also used undersampling techniques like monte carlo to deal with the data imbalance.

In the "Classwise Comparison of raw data and oversampled data" section: We compare the original data wit the data we get after oversampling.

#Feature analysis
After that we have perform the feature analysis by plotting all four accelerometer's reading along the three axis separately:
1-On waist, 2-On Right ankle, 3-On right upper arm, 4-On left thigh

#Raw featue vs Extracted feature analysis:
We have compared the performance using the above two feature set and plotted the confusion matrix for the same with Logistic Regression and Decision Trees. 

# Using various ML algoritms with different preprocessing techniques and feature set:

#1-Using all the features(Extracted and Raw features) for Ml Models: Logistic Regression, SGD Classifier, Decision Tree Classifier, Random Forest Classifier, 
Support Vector Classification and Guassian Naive Bayes and generating Evaluation matrix for all cases.


#2-Using class weights technique to handle data imbalance and then using the data for Ml Models: Logistic Regression, SGD Classifier, Decision Tree Classifier, Random Forest Classifier, Support Vector Classification and Guassian Naive Bayes and generating Evaluation matrix for all cases.


#3-Using Raw features for Ml Models: Logistic Regression, SGD Classifier, Decision Tree Classifier, Random Forest Classifier, 
Support Vector Classification and Guassian Naive Bayes and generating Evaluation matrix for all cases.


#4-Using Undersampling technique to handle data imbalance and then using the data for Ml Models: Logistic Regression, SGD Classifier, Decision Tree Classifier, Random Forest Classifier, Support Vector Classification and Guassian Naive Bayes and generating Evaluation matrix for all cases.


#5-Using Monte Carlo Undersampling technique to handle data imbalance and then using the data for Ml Models: Logistic Regression, SGD Classifier, Decision Tree Classifier, Random Forest Classifier, Support Vector Classification and Guassian Naive Bayes and generating Evaluation matrix for all cases.

# Final pipeline
The Code folder also contains a **DetectAsana_final.ipynb** file which is a complete main pipeline for the classification task after analysing their affects on the performance.
The Feature set that we have used are **'weight', 'body_mass_index', 'pitch1', 'y3', 'roll4', 'y4', 'pitch2', 'z1', 'z4', 'z2', 'norm1', 'x4', 'y2', 'y1', 'x3', 'z3', 'x2', 'roll1', 'norm4', 'norm2', 'norm3', 'x1'**. The Resampling technique that we have used is **Bagging/Monte Carlo** to deal with the data imbalance. Finally we have used the best accuracy giving ML model i.e. **Random Forest** for the classification task. The final accuracy that we get using the main pipeline is : **99.5%.**

# Other files
#Dataset folder
The dataset folder contains the PUC-RIO dataset in .csv format along with a Readme file which contains the dataset's description.

#DetectAsana Proposal.pdf is the project proposal submitted for the Machine Learning Project on Sept 10.

#Mid-Progress Report.pdf is the midsem-progress report of Machine Learning Project submitted on Nov 22.

#Pipeline.pdf is the final pipeline suggested for the classification task
#DetectAsana-poster.pdf is the poster on the literature review performed

# Weights folder
It consists of the final model trained using the suggested pipeline
