There are two folders.
	- k_fold folder is for getting the accurary of each AI technique. 
	It used k=12 which partitioned the data into 12 subset represeting the year.
	
	- prediction folder is mainly for visualizing the model and its one time prediction accuracy.
	It prints out the graph of the model and the predicting point as well  the accuracy.
	Please follow instruction in How-to run the code section below.

*********
	Please use python3 and have library inlcuding sk-learn and mathplotlib
*********

How-to-run the code
	-k_fold folder
	py <codes> <data text file>
	ex: py .\svr_kfold.py '.\Demand Data.txt'
	This will print out the accuracy of each subset and also the total average.

	-prediction folder
	py <code> <data text file>
	ex: py .\svr_prediction.py '.\Demand Data.txt'
	Dataset start from 01_07 to 10_18
	Enter a desired length for model training serperated by space:
****	From month year to month year:1 7 12 17
****	How many month ahead you want to predict? 10

****Important: As mention above, since we want get the prediction and the accuracy at the same time we can only do the training and the predictiong within the dataset range, 01-2017 to 10-2018. 
In the field for model training input, please input 1 7 12 17. This means the training is up to 12-2017.
In the field for prediction, please input 10. This means the prediction is the next 10 months which is up to 10-2018.


