
TODO: Add iPython Notebook with details about the model approach and repro steps below 

To reproduce results:

Prequisites: python, pypy, pandas

1. Download the 3 original datafiles (TrainingData.csv,TestData.csv,and SubmissionFormat.csv) to origdata folder
2. Run "python MakeDatasets.py" - note that this currently requires Linux or OSX as it uses unix shell commands.  This can be easily fixed later.  This command produces the working files TrainPredictors.csv, TrainLabels.csv, and TestData2.csv.
3. Run "pypy Online.py 4 0.5" - note that pypy is required.  This command fits an online logistic regression model, taking 4 passes/epochs over the training data with a 50% chance of using an encountered example in each epoch. (The effect of playing with epochs and use_example_probability is not large, this is just an example configuration). 

The submission will then be placed in the file submission1234.csv. Score should be somewhere between 0.3605 and 0.3665 (public leaderboard). 



