
BoxPlots First Place Model
==========================

To reproduce results:

Prerequisites:
* python 2.7+,
* pypy 2.2.1,
* pandas 0.14.1

Scripts: `MakeDatasets.py`, `Online.py`

1.  Download the 3 original datafiles (`TrainingData.csv`,`TestData.csv`,and `SubmissionFormat.csv)` to the folder  `origdata/`.
2.  Run `python MakeDatasets.py` - this command produces the training and test files `trainPredictors.csv`, `trainLabels.csv`, and `TestData2.csv`.
3.  Run `pypy Online.py 4 0.5` - note that PyPy is required. This command fits an online logistic regression model, taking 4 passes/epochs over the training data with a 50% chance of using an encountered example in each epoch. (The effect of playing with epochs and `use_example_probability` is small for reasonable values - this is just an example configuration but the one used for the winning submission).
The submission will then be placed in the file `submission1234.csv`. Score should be somewhere around 0.3665 (public leaderboard).

For more details see: `BoxPlots_First_Place_Model.ipynb`
