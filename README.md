# DetectAsana

#Code folder
The Code folder contains the .pynb file with the implementation of various Machine Learning Algotirhm's on PUC-RIO dataset for training and pre-processing of data. 

In the Feature Extraction Section:
We calculated norm=sqrt(x^2 + y^2 + z^2), pitch=tan_inverse(y/(x^2+z^2)) and roll=tan_inverse(-x/z) and added those to the features.

In the Resampling and Feature Selection:
Oversampling: We have used the ADASYN(Adaptive Synthetic) sampling to deal with data imbalance. 

Tsne-plot for the above:

In the Classwise Comparison of raw data and oversampled data: We compare the original data wit the data we get after oversampling and got the results below:

#Feature analysis
After that we perform the feature analysis by plotting all the accelerometer's reading along the three axis separately:
On waist:

On Right ankle:

On right upper arm:

On left thigh:

#Raw featue vs Extracted feature analysis:




# Now we begin with Ml algoritms using different preprocessing techniques and feature set:

#1-Using all the features(Extracted and Raw features) 
1- Logistic Regression:
Evaluation Matrix:

2- SGD Classifier:
Evaluation Matrix:

3- Decision Tree Classifier: 
Evaluation Matrix:

4- Random Forest Classifier:
Evaluation Matrix:

5- Support Vector Classification:
Evaluation Matrix:

6- Guassian Naive Bayes:
Evaluation Matrix:

#2-Using class weights technique to handle data imbalance
1- Logistic Regression:
Evaluation Matrix:

2- SGD Classifier:
Evaluation Matrix:

3- Decision Tree Classifier: 
Evaluation Matrix:

4- Random Forest Classifier:
Evaluation Matrix:

5- Support Vector Classification:
Evaluation Matrix:

6- Guassian Naive Bayes:
Evaluation Matrix:

#3-Using Raw features
1- Logistic Regression:
Evaluation Matrix:

2- SGD Classifier:
Evaluation Matrix:

3- Decision Tree Classifier: 
Evaluation Matrix:

4- Random Forest Classifier:
Evaluation Matrix:

5- Support Vector Classification:
Evaluation Matrix:

6- Guassian Naive Bayes:
Evaluation Matrix:

#4-Using Undersampling technique to handle data imbalance
1- Logistic Regression:
Evaluation Matrix:

2- SGD Classifier:
Evaluation Matrix:

3- Decision Tree Classifier: 
Evaluation Matrix:

4- Random Forest Classifier:
Evaluation Matrix:

5- Support Vector Classification:
Evaluation Matrix:

6- Guassian Naive Bayes:
Evaluation Matrix:

#5-Using Monte Carlo Undersampling technique to handle data imbalance
1- Logistic Regression:
Evaluation Matrix:

2- SGD Classifier:
Evaluation Matrix:

3- Decision Tree Classifier: 
Evaluation Matrix:

4- Random Forest Classifier:
Evaluation Matrix:

5- Support Vector Classification:
Evaluation Matrix:

6- Guassian Naive Bayes:
Evaluation Matrix:

#Dataset folder
The dataset folder contains the PUC-RIO dataset in .csv format along with a Readme file which contains the dataset's description.

#DetectAsana Proposal.pdf is the project proposal submitted for the Machine Learning Project.

#Mid-Progress Report.pdf is the midsem-progress report submitted.
