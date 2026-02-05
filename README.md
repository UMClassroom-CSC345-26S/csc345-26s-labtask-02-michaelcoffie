[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/L8zfSSmy)
# Identify the Car Style

Can a K-nearest neighbours classifier predict the style of a car from it's make, interior volume, and number of doors?
This labtask has several parts:
- Collect the data for 10 cars.
  The sample must be a *Simple Random Sample*. 
  Put the data in an Excel spreadsheet called `MyCars.csv` with the columns `Make`, `Volume`, `Doors`, and `Style`.
  The `Make` is something like `Ford`, `Tesla`, `Nissan`, etc.
  The `Volume` is a real number of cubic feet.
  The `Doors` is an integer (count a hatchback as a door).
  The `Style` is one of `Sedan`, `SUV`, `Jeep`, `Pickup`, or `Van`.
  You can get the interior volume of a car by asking an LLM, giving the make and model - something like
  "What is the interior volume of a Nissan Xterra?".
  Submit `MyCars.csv`. (1.0%)
- The TA will combine all the samples into one spreadsheet that everyone can use. You can add it to your
  repository by merging my pull request.
- Remove non-ordinal features, and normalize the ordinal features.
  Randomly split the resultant data set into a training set of 80% and a testing set of 20%.
  Put the training set in a spreadsheet called `Training.csv` and the testing set in a spreadsheet
  called `Testing.csv`.
  Use K-nearest neighbours classification in Python to train the model, then predict the `Style` of
  each car in the testing set.
  You must iterate over K to find the highest accuracy.
  Call the Python program `KNNClassifier.ipynb`/`KNNClassifier.py` (depending how you implement it).
  Create a spreadsheet called `Accuracy.csv` with the columns `K` and `Accuracy`, and record the
  accuracy achieved for each `K`.
  Report the results for the `K` with the highest accuracy by adding two new columns to  `Testing.csv` called
  `Prediction`, and `Confidence` to store the prediction and confidence for each car in the testing set.
  Submit `Training.csv`, `Testing.csv`, `Accuracy.csv`, and `KNNClassifier.ipynb`/`KNNClassifier.py`. (3.0%)
