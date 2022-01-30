* R^2 is amount of variation explained by X variables
* Reviewed Linear Regression Estimation
	* Assumptions on Data: 
		* Linearity, Low Noise, Non-Collinearity in IV, Gaussian Distributions 
			* What is BoxCox? Can use Log to make distribution more normal 
	* null hypothesis testing X-Y relationship
		* t = a - 0/(SE(a)), SE(a) = S/n^.5
	* Regularization 
		* Ridge: 1/n * Sum (y(i) - (ax + b))^2  + Lambda sum(a^2) --- what is the a^2 again? 
			* Impose a penaltiy equivalent to the sum of squares of the model's coefficents.
			* Coefficient shrinkage
			* reduces model complexity
			* Lasso: absolute value on |a|^2
				* Better for feature selection, zeroes out most coefficients, more robust. 
	* Error Calculation
		* RSS y - model prediction ^ 2
		* MAE: 1/n sum (y - predy)
		* MSE: 1/n (y - predy) ^ 2
			* big disparities are penalized more than with MAE
		* MAPE: mean absolute % error | y - predy|/y 
			* different from MAE which is the average magnitude of error generated
		* RMSE = Root Mean Square Error => MSE from above
		* Adjusted R^2  = falls when bad variables are added. 
* Is each p value is a multivariate regression separately interpretable?
* Why is MSE not more robust and better than MAE?f