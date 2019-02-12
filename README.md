# README
This project contains natural languageg data for human-robot interaction in home domain which we collected and annotated for evaluating NLU Services/platforms.

## License
All data are released under the CC BY-SA 3.0 license.
## Content
It contains

1. Collected-Original-Data (25K):  collected original data with normalization for numbers/date etc which contain the pre-designed human-robot interaction questions and the user answers. They are organized in CSV format.

2. AnnotatedData (25716 Lines): annotated for Intents and Entities, organized in csv format.

3. The 10-fold cross-validation we used (here for reference only)

CrossValidation contains the generated data for different NLU services we used for our evaluations which are uploaded here for reference only as they can be generated from the annotated csv data using our scripts. NB: the script will shuffle the data each time when runing the script, so the generated data may not be exact the same each time.


autoGeneFromRealAnno/: generated trainset and testset from the annotated csv file.
The other four subdirectories (out4ApiaiReal, out4LuisReal, out4RasaReal and out4WatsonReal) in CrossValidation/ are the converted NLU service input data for Dialogflow, LUIS, Rasa and Watson respectively. The inside 'merged' directory contains the trainning input data.


## Scripts for the Data Preparation and Evaluation
Java for preparing the data and Python scripts for querying the Services/Platforms are [Here](https://github.com/xliuhw/NLU-Evaluation-Scripts)

## Contact
Please contact x.liu@hw.ac.uk, if you have any questions


