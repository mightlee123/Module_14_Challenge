# Module_14_Challenge
## Baseline (SVM):
![bokeh_plot (1)](https://user-images.githubusercontent.com/75819421/114354368-febe2680-9b22-11eb-9d23-b98e0ad8e2b5.png)
![image](https://user-images.githubusercontent.com/75819421/114356321-4f368380-9b25-11eb-8e32-235d77ab0b50.png)

	Short Window = 4 days
	Long Window = 100 days
	Dataset = 3 months
	svm_model accuracy = 55%
	svm_model precision on buy is 56% and sale is 43%
	svm_model recall on buy is 4% and sale is 96%
## Tuned Trainning Module:
Step 1: Adjusting the size of the training dataset (Dataset = 6 months)
![image](https://user-images.githubusercontent.com/75819421/114358795-2e236200-9b28-11eb-9c62-7948230b1a62.png)

	What impact resulted from increasing or decreasing the training window?
	A minor increase in svm_model's accuracy, precision on sale, and reall on sale.
	A minor decrease in recall on buy.

Step 2: Adjusting the SMA input features (Short Window = 8 , Long Window = 200, Dataset = 3 months)
![image](https://user-images.githubusercontent.com/75819421/114361675-3d57df00-9b2b-11eb-884b-a9a0b4095bee.png)

	What impact resulted from increasing or decreasing either or both of the SMA windows?
	Increasing both of the SMA windows results a slightly more accurate precision on selling. 
	The recall on buying has a minor decrease and on selling has a minor increase. 
Best Improved (increase dataset size)

		Based on the results from above, the best change in parameter to improve the trading algorithm returns is by 
		increasing the dataset size, which increases the accuracy of the model. 


## LogisticRegression Model
![bokeh_plot (2)](https://user-images.githubusercontent.com/75819421/114354370-ff56bd00-9b22-11eb-97cf-ce20a3380825.png)
![image](https://user-images.githubusercontent.com/75819421/114364323-22d33500-9b2e-11eb-8ac1-b2f2f4f12594.png)

	Short Window = 4 days
	Long Window = 100 days
	Dataset = 3 months
	logistic_regression_model accuracy= 52%
	logistic_regression_model precision on buy is 56% and sale is 44%
	logistic_regression_model recall on buy is 66% and sale is 33%
## SVM vs Tuned vs LogisticRegression
	Did this new model perform better or worse than the provided baseline model? 
	Did this new model perform better or worse than your tuned trading algorithm?
	Out of the three results the LogisticRegression model had the least accuracy. 
	The ratio bewteen the Precion for buy and sale in the LogisticRegression model 
	is much different compared to the other two results. 

## Summary
	Between the SVM model and the LogisticRegression model, the SVM model yelds a higher accuracy. 
	And by tunning the dataset from 3 to 6 months we can yeld a more accurate result. 
