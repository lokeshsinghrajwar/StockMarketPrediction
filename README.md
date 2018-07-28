# StockMarketPrediction
In this project I have use three different models to predict the prices of Alphabet stocks, then plot them all on a graph to compare the results.

I have collected the past 30 days Historical prices of Alphabet from NASDAQ.

I have used the support vector regression is a type of SVM that uses the space between data points as a margin of error and predicts the most likely next point in a dataset.

First we create a linear support vector regression model. 
Takes in 3 parameters: 
 	1. kernel: type of SVM
 	2. C: penalty parameter of the error term
	3. gamma: defines how far too far is.

	Two things are required when using an SVR, a line with the largest minimum margin and a line that correctly separates as many instances as possible. Since we can't have both.
	C determines how much we want the latter.

Next we make a polynomial SVR because in math folklore, the no free lunch theorem states that there are no guarantees for one optimization to work better than the other. So we'll try both.

Finally, we create one more SVR using a radial basis function. RBF defines similarity to be the Euclidian distance between two inputs.

The result is shown in Result.png, in which we can clearly see that RBF model covers the maximum points, thus predicts the most accurate price among the three models.
