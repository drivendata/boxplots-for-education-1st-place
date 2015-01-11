
BoxPlots First Place Model
==========================

To reproduce results:

Prerequisites: python 2.7+, pypy 2.4.0, pandas 0.14.1

Scripts: MakeDatasets.py, Online.py

Download the 3 original datafiles (TrainingData.csv,TestData.csv,and SubmissionFormat.csv) to a folder called "origdata"
Run "python MakeDatasets.py" - this command produces the training and test files TrainPredictors.csv, TrainLabels.csv, and TestData2.csv.
Run "pypy Online.py 4 0.5" - note that pypy is required. This command fits an online logistic regression model, taking 4 passes/epochs over the training data with a 50% chance of using an encountered example in each epoch. (The effect of playing with epochs and use_example_probability is small for reasonable values - this is just an example configuration but the one used for the winning submission).
The submission will then be placed in the file submission1234.csv. Score should be somewhere between 0.3605 and 0.3665 (public leaderboard).

For more details see:
http://nbviewer.ipython.org/url/machinelearner.net/boxplots-for-education-1st-place/BoxPlots_First_Place_Model.ipynb


