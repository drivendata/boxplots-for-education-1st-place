
TODO: Add iPython Notebook with details about the model approach and repro steps below 

To reproduce results:

1.  Download the 3 original datafiles (TrainingData.csv,TestData.csv,and SubmissionFormat.csv) to origdata folder
2.  Run "python MakeDatasets.py" - note that this currently requires Linux or OSX as it uses unix shell commands.  This can be easily fixed later
3.  Run "pypy Online.py 4 0.5" - note that pypy is required.  

The submission file will then be placed in submission1234.csv. Score should be somewhere between 0.3605 and 0.3665 (public leaderboard). 



