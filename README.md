
[200~This is a course project code. It is required to apply deep learning method to an APP business case to predict if a customer will buy product again.

The .csv summarizing the data. There are several variables: Customer ID, ), Book length overall (sum of the minute length of all purchases), Book length avg (average length in minutes of all purchases), Price paid_overall (sum of all purchases) ,Price Paid avg (average of all purchases), Review (a Boolean variable whether the customer left a review), Review out of 10 (if the customer left a review, his/her review out of 10, Total minutes listened, Completion (from 0 to 1), Support requests (number of support requests; everything from forgotten password to assistance for using the App), and Last visited minus purchase date (in days).

These are the inputs (excluding customer ID, as it is completely arbitrary. It's more like a name, than a number).

The targets are a Boolean variable (0 or 1). Here is taking a period of 2 years in the inputs, and the next 6 months as targets. So, in fact, I am predicting if: based on the last 2 years of activity and engagement, a customer will convert in the next 6 months. 6 months sounds like a reasonable time. If they don't convert after 6 months, chances are they've gone to a competitor or didn't like the Audiobook way of digesting information. 

The task is simple: create a machine learning algorithm, which is able to predict if a customer will buy again. 

This is a classification problem with two classes: won't buy and will buy, represented by 0s and 1s.

the process for analysis:
- Data preprocessing
1 Preprocess the data, (sometimes it needs to shuffle the dataset)
2 balance the dataset,
3 create 3 datasets: training, validation, and test
4 save the newly created sets in a tensor friendly format (e.g. *.npz)

- Create the machine learning algorithm
5 import the dataset in friendly format
6 create the model ( outline, optimizers, loss, early stopping and training)
7 test the model



