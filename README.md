# PhysioPainClassifier



Project Description
You are to develop a new system that can identify (i.e. classify) pain from physiological data that will be collected from wearable devices. You will have access to the type of data that will be collected to train and test your system.
Experimental Design
•	You are required to write a script called Project2.py, however, you are free to split up your program into multiple files.
•	Data types available: Diastolic BP, Systolic BP, EDA, and Respiration
•	Your script needs to take a command line parameter to determine which data type will be run - python Project2.py <data_type> <data_file>, where data_file is an absolute directory and data_type is one of the following:
o	dia – Diastolic BP
o	sys – Systolic BP
o	eda – EDA
o	res – Respiration
o	all – Fusion of all data types
•	There are 60 subjects in total, each having of the data types above for both classes (pain and no pain). Data has been collected into a CSV file with the following columns: Subject ID, Data Type, Class, Data. Data is variable length, which is a common problem when working with physiological data.
•	You will create hand-crafted features for this project. From Data you will calculate the mean, variance, min, and max for all 4 data types. In total there will be 16 features (4 features from each type). These values are your training and testing data.
o	For the 4 data types, you will have a list of size 4 for each instance of the data. For the fusion, you will create a list of size 16 that contains all data types.
•	You will use these features to build and train a classifier to classify pain vs. no pain. You get to chose your classifier for this project.
•	For training your models and testing, you need to perform 10-fold cross-validation. The same subject cannot be in the training and testing. Each fold will have 6 subjects in it. You will use 9 of them for training and 1 for testing. You need to test on each fold.
•	The output of your script must print the confusion matrix, classification accuracy, precision, and recall. As you are doing 10-fold cross validation, you need to take the average of these values over all folds of your testing. For the confusion matrix, you will have 10 confusion matrices from each test, you need to add these matrices and take the average for the final matrix.
•	Final note on experiments. Overall accuracy does not matter for this project. You are not required to classify at 100% accuracy. The goal is to learn how different data types can give different accuracies for the same problem.
 
