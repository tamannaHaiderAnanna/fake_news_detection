Instruction for running the code:
--------------------------LSTM MODEL-------------------------
1.Run the cells #1 to #5 respectively for package installation and library initialization.
2.Then run the cell #6 for mounting the drive for database access.
3.Run the cell #7 to read the csv file which contain all the data.
4.Run the cell #8 for the shape of the whole dataset.
5.Run the cell #9 and #10 to replace and drop the null value in dataset.
6.Run the cell #11 to get the dependent features.
7.Next run the cell #12 and #13 for tokenization and counting the number of token.
8.In data pre-processing section, run the cell #14 and #15 respectively to pre-precess the data.
9.In word2vec model section, run the cell #16 to #28 respectively for word embedding.
10.Then in LSTM Model section, run the cell #29 for model evaluaion.
11.Next run the cell #30 to #34 respectively for result evaluation, plotting the accuracy and loss curve.
12.At last run the cell #35 for the classification report of LSTM model.
---------------------------CNN MODEL---------------------------
1. Repeat the step from 1 to 9 which is given in above description.
2.After in CNN model section, run the cell #36 for model evaluation.
3.Next run the cell #37 to #40 for result evaluation, plotting the accuracy and loss curve.
4.After that run the cell #41 and #42 for the classification report of CNN model.
---------------------------CNN-LSTM MODEL---------------------
1.Repeat the step from 1 to 9 which is given in LSTM MODEL.
2.In CNN-LSTM model section, run the cell #43 for the model evaluation.
3.Then run the cell #44 to #47 for result evaluation, plotting the accuracy and loss curve.
4.And then run the cell #48 and #49 for the classification report of CNN-LSTM model.
--------------------------CROSS Validation for CNN-------------
1.Repeat the step from 1 to 9 which is given in LSTM MODEL.
2.Then run the cell #50 for 5-fold cross validation of CNN model.
-------------------------CROSS Validation for CNN-LSTM--------
1.Repeat the step from 1 to 9 which is given in LSTM MODEL.
2.Then run the cell #51 for 5-fold cross validation of CNN-LSTM model.
-------------------------CROSS Validation for LSTM--------------
1.Repeat the step from 1 to 9 which is given in LSTM MODEL.
2.Then run the cell #52 for 5-fold cross validation of LSTM model.

**Run the cell #53 to draw barchart for the result of precentage split validation.
**RUn the cell #54 to draw barchart for the result of cross validation approach.