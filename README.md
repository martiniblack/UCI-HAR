# UCI-HAR
ML project for human activity classification

Classification and clustering of uci-HAR data

This dataset comes from the <a href=https://archive.ics.uci.edu/ml/>UCI Machine-Learning repository</a>. Please first read the <a href=https://archive.ics.uci.edu/ml/datasets/Smartphone+Dataset+for+Human+Activity+Recognition+%28HAR%29+in+Ambient+Assisted+Living+%28AAL%29>dataset description</a> to understand what is the data.
The goal on this dataset is first to perform clustering on UNLABELLED data, and to learn a classifier on LABELLED. Finally, analysis should be conducted to check whether or not the clustering could be used for classification (i.e. does the clusters properly map on classes, possibly with more than 1 cluster per class?).

Data Set

Information

We collected more dataset to improve the accuracy of our HAR algorithms applied in a Social connectedness experiment in the domain of Ambient Assisted Living. The dataset was collected from the in-built accelerometer and gyroscope of a smartphone worn around the waist of participants. See waist_mounted_phone.PNG. The data was collected from 30 participants within the age group of 22-79 years. Each activity (standing, sitting, laying, walking, walking upstairs, walking downstairs) was performed for 60secs and the 3-axial linear acceleration and 3-axial angular velocity were collected at a constant rate of 50Hz.
Data of extracted features:

For each record in the dataset it is provided:

A 561-feature vector with time and frequency domain variables.
Its activity label. The labels are from 1 to 6, corresponding to: 1 WALKING; 2 WALKING_UPSTAIRS; 3 WALKING_DOWNSTAIRS; 4 SITTING; 5 STANDING; 6 LAYING

File details:

'train/X_train.txt': Training set: 7352 samples * 561 features

'train/y_train.txt': Training labels: 7352 samples * 1 label

'test/X_test.txt': Test set: 2947 samples * 561 features

'test/y_test.txt': Test labels: 2947 samples * 1 label

'features.txt': List of all features.

'features_info.txt': Shows information about the variables used on the feature vector.

'activity_labels.txt': Links the class labels with their activity name.

Data of time sequences:

The dataset also includes the time sequences of Accelerometer & Gyroscope signals of each record before extracting the features. They are available for the train and test data. Their descriptions are equivalent.

'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_y_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis.

'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.

'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.

Algorithms to use:

For this mini project, we will use following machine learning algorithms to analyze the data of extracted features:

Dimensionality Reduction (Unsupervised Learning):

TSNE

Clustering (Unsupervised Learning):

K-Means

AHC

GMM

Classification (Supervised Learning):

Random Forest

MLP

We will also use following machine learning classification algorithms to analyze the time sequences of Accelerometer & Gyroscope signals:

HMM (Supervised Learning) -- Please check "uci_HAR_sequence_HMM.ipynb"

LSTM (Supervised Learning) -- Please check "uci_HAR_sequence_LSTM.ipynb"
