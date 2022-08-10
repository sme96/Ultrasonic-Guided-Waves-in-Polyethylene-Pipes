# About this repository

The programs in this repository read the data from a number of damaged state trials of both finite element models (FEMs) and physical experiments. 

The database of model results is populated by the original signal responses from the model for a number of transducer array locations. The program generates white noise 
of user-specified properties and time-averages the the noisy responses.

The database of physical experimental results is populated by signal responses picked up by a bus-powered USB (NI 4431). Environmental white noise is a natural inclusion 
of the signal in this case; therefore a number of trace responses are populated into the database for time-averaging.

All of the trials are marked by their states of damage, and the type of damage variation is specified by the user. Principal Component Analysis (PCA) is used to reduce 
the dimensionality of the data and clearly present the relation of the damaged state with the PCs. Machine Learning via Support Vector Machines (SVM) is used to 
determine the optimal number of PCs. It may also be used to classify the data through application of feature extraction methods.
