Codebook : Activity_data_per_activity_and_subject.txt
Dataset description:	The dataset is based on data originally collected by Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto at the Smartlab - Non Linear Complex Systems Laboratory DITEN - Università degli Studi di Genova, Genoa I-16145, Italy.  The original dataset �was a �Human Activity Recognition database built from the recordings of 30 subjects performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors�.  The original can be obtained at http://archive.ics.uci.edu/ml/machine-learning-databases/00240/UCI%20HAR%20Dataset.zip
	The original dataset was not easy to analyse statistically, as it was distributed across multiple text files, containing training and test sets, labels for activities, labels for subjects etc.
	The current dataset attempts to make the data more accessible, by providing a single data file of text format, in which each subject�s data is recorded in a single row.  In order to do this, we selected only mean and standard deviation data on the original activity variables, and then we averaged these across subjects.  
Transformations:	The R script file that records how the original dataset was transformed to its format from the original data is called run_analysis.R
	Briefly, the transformations were 
		1	Read in test data set files and name the vars
       2	Combine the subject names, activities, and data
3	Create a variable that reflects that all these data are from the test set	
4	Repeat 1-3 for training set
5	Combine the training and test data sets
6	Select and retain variables that reflect computations of mean and standard deviation
7	Reshape data file so that each record reflects one subject, with means computed for each of the variables in 6

File:	Activity_data_per_activity_and_subject.txt  Text format (Windows), comma separated.  30 records for 475 variables
Variables:	These are described in brief, the example specifications should be clear enough to interpret the content of the rest of the variables.  All measured variables report co-ordinates, and usually in XYZ space	
Variable





