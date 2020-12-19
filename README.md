# DetectAsana

#Code folder
The Code folder contains the .pynb file with the implementation of various Machine Learning Algotirhm's on PUC-RIO dataset for training and pre-processing of data. 

In the Feature Extraction Section:
We calculated norm=sqrt(x^2 + y^2 + z^2), pitch=tan_inverse(y/(x^2+z^2)) and roll=tan_inverse(-x/z) and added those to the features.

In the Resampling and Feature Selection:
Oversampling: We have used the ADASYN(Adaptive Synthetic) sampling to deal with data imbalance. 

Tsne-plot for the above:

In the Classwise Comparison of raw data and oversampled data: We compare the original data wit the data we get after oversampling and got the results below:

After that we perform the Raw feature analysis by plotting all the accelerometer's reading along the three axis separately:
On waist:

On Right ankle:

On right upper arm:

On left thigh:



#Dataset folder
The dataset folder contains the PUC-RIO dataset in .csv format along with a Readme file which contains the dataset's description.

#DetectAsana Proposal.pdf is the project proposal submitted for the Machine Learning Project.

#Mid-Progress Report.pdf is the midsem-progress report submitted.
