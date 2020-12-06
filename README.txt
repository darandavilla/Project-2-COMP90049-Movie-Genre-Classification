Project 2: Introduction to Machine Learning COMP90049 S1-2020

All programs were tested in Jupyter 6.0.0 (Python 3.8.2), Anaconda environment. Windows 10 - 64 bits.

I - Files:

A - Pj 2 IML Dummy Classifier Baseline - ID992038.ipynb
B - Pj 2 IML LogReg - ID992038.ipynb
C - Pj 2 IML SVM - ID992038.ipynb
D - Pj 2 IML XGBoost - ID992038.ipynb
E - Pj 2 IML Test Predictions - ID992038.ipynb

Please feel free to run all the cells in the order they are given. If anything unexpected happens,
please see the requirements section of this README file.

II - File structures:

Files A-B-C-D are for training and validation and are executable in Jupyter environment.
Files A-B-C-D are all structured in the same manner, as we show in the following list:

1 - Load Data
2 - Clean Data
3 - Preprocessing
	3.1 - Vectorize words using Tfidf
	3.2 - One hot encoder for years
	3.3 - Scale data and match columns
4 - All features
	4.1 - Feature selection (All features)
	4.2 - Feature sizes
	4.3 - Learning curve (All features)
	4.4 - Validation (All features)
5 - Metadata features only
	5.1 - Feature selection (Metadata features only)
	5.2 - Learning Curve (Metadata features only)
	5.3 - Validation (Metadata features only)
6 - Audio/Visual features only
	6.1 - Feature selection (Audio/Visual features only)
	6.2 - Learning Curve (Audio/Visual features only)
	6.3 - Validation (Audio/Visual features only)

File E is for generation of Kaggle files in csv, where we included 2 models (LR and XGB).
The csv files will be created in the same folder/location where the jupyter notebook is.
File E is structured as follows:

1 - Load Data
2 - Clean Data
3 - Preprocessing
	3.1 - Vectorize words using Tfidf
	3.2 - One hot encoder for years
	3.3 - Scale data and match columns
4 - Feature selection (All features)
5 - Logistic Regression Upload
6 - XGBoost Upload

III Requirements

1 The dataset files should be all located in the same folder as the Jupyter files for execution
	- train_features.tsv
	- train_labels.tsv
	- valid_features.tsv
	- valid_labels.tsv
	- test_features.tsv
2 sklearn version --> 0.22.1, for installing:
	- pip install -U scikit-learn
	- conda install -c intel scikit-learn
3 xgboost version --> 0.90, for installing:
	- conda install -c anaconda py-xgboost
	- if that does not work, please try:
		1 latest version of python --> https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe (or above)
		2 latest version of pip --> https://bootstrap.pypa.io/get-pip.py
		2.1 then run in console python get-pip.py
		3 get python xgboost at --> https://www.lfd.uci.edu/~gohlke/pythonlibs/#xgboost
		3.1 download "xgboost‑0.90‑cp35‑cp35m‑win_amd64.whl" (or the 32 bit version if needed)
		4 install xgboost python whl file using the command
		  pip install xgboost-0.90-cp35-cp35m-win_amd64.whl
		5 finally, try "import xgboost" in a Jupyter cell, that's all :)