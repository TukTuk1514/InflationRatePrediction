Inflation Rate Prediction Method Based on Regression

1.Introduction :
Inflation is a complex economic phenomenon that refers to a general increase in prices and fall in the purchasing power of money. Economists view inflation as a function of the supply and demand for money, with an increase in the money supply leading to a decrease in the value of each dollar. Moderate inflation levels are often seen as necessary for economic growth, as they can drive consumption and keep businesses profitable. However, high inflation rates can have negative impacts, such as making it harder to save money, increasing debt costs, and potentially leading to a slowdown in the economy. The Federal Reserve aims for a long-term inflation rate of 2%, believing that slow and steady price increases help encourage business activity. Inflation can also have both positive and negative effects on different groups of people, depending on their economic situations.
While a small amount of inflation can be a sign of a healthy economy, high inflation rates can have negative impacts, such as making it harder to save money and increasing debt costs. Inflation can be caused by demand-pull factors, such as increased demand for goods or services, or cost-push factors, such as limited supply. It is measured by indexes such as the Consumer Price Index (CPI), Producer Price Index (PPI), and Personal Consumption Expenditures Price Index (PCE).

Prediction of Inflation can be done in many ways, one of it is the “Regression Model”.Predicting inflation rates using regression involves building a statistical model that uses historical data to estimate future inflation. This can be done using a variety of techniques, such as simple linear regression or more complex models like auto regressive integrated moving average (ARIMA) models. The goal is to identify patterns and relationships in the data that can help predict future inflation rates. For example, a regression model might use past inflation rates, economic indicators like GDP growth or unemployment rates, and other factors like interest rates or exchange rates to predict future inflation. The model would then use these variables to estimate the likelihood of future inflation rates, providing a forecast that can help policymakers, businesses, and individuals make informed decisions. However, it's important to note that no model is perfect, and there are always factors that can impact inflation rates that may not be captured by the model. As a result, it's important to use multiple sources of information and to continually monitor and adjust forecasts as new data becomes available.
In this process our main focus will be on :
1.Linear Regression (LR)
2.Support Vector Regression (SVR)
3.Random Forest Regression (RFR)


2.Basics of Regression Model :
A regression model is a statistical tool that helps to understand the relationship between a dependent variable and one or more independent variables. The model uses historical data to estimate the coefficients that best describe the relationship between the variables. In other words, it finds the best-fitting line or curve that explains the behavior of the dependent variable based on the independent variables.
These are following variants that will be used :
1.Linear Regression (LR)
2.Support Vector Regression (SVR)
3.Random Forest Regression (RFR)
	
2.1. Working of “Linear Regression” :
Linear regression is a simple and widely used statistical method for 	modeling the relationship between a dependent variable and one or 	more independent variables. In the context of inflation prediction, linear 	regression can be used to model the relationship between the consumer 	price index (CPI) and various economic indicators, such as the 	unemployment rate, GDP growth rate, and interest rates.

2.2. Working of “Support Vector Regression” :
Support vector regression (SVR) is a machine learning method that can 	be used for regression analysis. SVR is based on the concept of support 	vector machines (SVM), which are used for classification tasks. In SVR, 	the goal is to find a function that fits the data within a certain margin of 	error. SVR can be used to model non-linear relationships between the 	CPI and economic indicators, making it a powerful tool for inflation 	prediction.

2.3. Working of “Random Forest Regression” :
Random forest regression is another machine learning method that can 	be used for regression analysis. Random forest regression is based on the 	concept of decision trees, which are used for both classification and 	regression tasks. In random forest regression, multiple decision trees are 	combined to create a more accurate model. Random forest regression 	can also be used to model non-linear relationships between the CPI and 	economic indicators, making it a useful tool for inflation prediction.

In this study, we will be taking notes about these regression models while create a working model to predict the “INFLATION RATE” and compare among the above mentioned methods, which of them is more accurate and easy to incorporate in the Model.



2.1. Steps in “Linear Regression” :



2.2. Steps in “Support Vector Regression” :



2.3. Steps in “Random Forest Regression” :







3.Experiments and Analysis :
In this operation we will be importing the available datasets and process the information in the way we want it, so that we can get the desired output


	Step 1: Importing Dependencies :




	Step 2: Importing the Data Set :




	Step 3: Data Refining (Removing the noise) :




	Step 4:  Printing the Inflation Rates :




	Step 4.1: Inflation Rate :




	Step 5: Yearly CPI Calculation (from Monthly Data) :



	Step 5.1: Yearly CPI :



	Step 6: Complete data integration :


	
	Step 6.1 : Complete Data Frame :



	Step 7 : Creating Model :

	Step 7.1 : Importing Libraries :



	Step 7.2 : Preparing Training and Test Data :



	Step 7.3 : Linear Regression Model :












	Step 7.4 : Random Forest Regression and Support Vector Regression 	Model :



	Step 7.5 : Model Implementation Values : (Comparisons)



Analysis : 

The linear regression model has a mean squared error (MSE) of 2.6833811160858447 and a root mean squared error (RMSE) of 1.6381029015558957. The R-squared value is negative, indicating that the model does not fit the data well.

The random forest regression model has a lower MSE of 2.8992266379082627 and a positive R-squared value of 0.3289612329474715, indicating that the model explains 32.89% of the variation in the inflation rate.

The support vector regression model has the highest MSE of 9.340399788121246 and a negative R-squared value of -0.27122569369538985, indicating that the model does not fit the data well.

Overall, the random forest regression model appears to be the best fit for the data, as it has the lowest MSE and a positive R-squared value. However, the R-squared value is still relatively low, indicating that there may be other factors that are not accounted for in the model. It's important to note that these results are specific to the data used in the study and may not generalize to other datasets.

4.Result and Analysis :

Calculating the Values for making prediction and implement the 	model :


	




Graph of Predicted Vs Actual Values using Linear Regression :








Graph of Predicted Vs Actual Values using Support Vector and 		Random Forest Regression :

	
Accuracy Comparison between Linear, Support Vector and 		Random Forest Regression :




















5.Conclusion :

This project investigated the potential of machine learning to predict the Inflation rate changes over the year. By leveraging data on CPI and Inflation rate over the year we explored the ability to estimate the future changes in the Inflation Rate.

We have evaluated the performance of linear regression, support vector regression, and random forest regression in predicting inflation rates in the United States.

The results indicate that the random forest regression model (RFR) provides the best performance in predicting inflation rates, with the lowest mean absolute error (MAE), lowest mean squared error (MSE), and highest R-squared value.

Linear regression is a simple and widely used regression model that assumes a linear relationship between the input features and the output variable. In this case, it does not provide accurate predictions, as indicated by its high MAE and MSE values and low R-squared value.

Support vector regression (SVR) is a non-linear regression model that incorporates an additional term into the loss function to penalize outliers. In this case, SVR provides slightly better predictions than linear regression, with a lower MAE and MSE. However, its R-squared value is still lower than that of RFR.

Random forest regression is an ensemble learning method that combines the predictions of multiple decision trees. In this case, it provides the most accurate and robust predictions, with the lowest MAE, MSE, and highest R-squared value.

Therefore, it is recommended to use RFR as the primary model for predicting inflation rates in the United States. However, it is important to note that prediction accuracy may still vary depending on the specific features and time period used in the analysis. It is also worthwhile to consider alternative regression models and ensemble techniques for future research and exploration.

6.Data Availability :
The datasets used in this paper is publicly available.

7.Conflict of interest :
The authors declare that there are no conflicts of interest regarding the publication of this paper.


8.References :

[1 ] E. F. Fama, “\Term-structure forecasts of interest rates, inflation and real returns,” Journal of Monetary Economics,
vol. 25, no. 1, pp. 59–76, 1990.
[2] A. Ang, G. Bekaert, and M. Wei, “Do macro variables, asset
markets, or surveys forecast inflation better?” Journal of
Monetary Economics, vol. 54, pp. 1163–1212, 2007.
[3] K. Hubrich, “Forecasting euro area inflation: does aggregating
forecasts by HICP component improve forecast accuracy?”
International Journal of Forecasting, vol. 21, no. 1, pp. 119–
136, 2005.
[4] A. D’Agostino and P. Surico, “A century of inflation forcasts,”
,e Review of Economics and Statistics, vol. 94, no. 4,
pp. 1097–1106, 2012.
[5] A. Atkeson and L. E. Ohanian, “Are Phillips curves useful for
forecasting ination?” Federal Reserve Bank of Minneapolis
Quarterly Review, vol. 25, no. 1, pp. 2–11, 2001.
[6] T. Cogley and A. M. Sbordone, “Trend inflation, indexation,
and inflation persistence in the new keynesian Phillips curve,”
,e American Economic Review, vol. 98, no. 5, pp. 2101–2126,
2008.
[7] S. McKnight, A. Mihailov, and F. Rumler, “Inflation forecasting using the new keynesian Phillips curve with a timevarying trend,” Economic Modelling, vol. 87, pp. 383–393,
2020.
[8] C. S. Bos, P. H. Franses, and M. Ooms, “Inflation, forecast
intervals and long memory regression models,” International
Journal of Forecasting, vol. 18, pp. 243–264, 2002.
[9] A. Barnett, H. Mumtaz, and K. 'eodoridis, “Forecasting UK
GDP growth and inflation under structural change. A comparison of models with time-varying parameters,” International Journal of Forecasting, vol. 30, no. 1, pp. 129–143, 2014.
[10] S. Eickmeier, W. Lemke, and M. Marcellino, “Classical time
varying factor-augmented vector auto-regressive models-estimation, forecasting and structural analysis,” Journal of the
Royal Statistical Society: Series A, vol. 178, no. 3, pp. 493–533,
2015.
[11] F. S. Mishkin, “What does the term structure tell us about
future inflation?” Journal of Monetary Economics, vol. 25,
no. 1, pp. 77–95, 1990.
[12] F. S. Mishkin, “A multi-country study of the information in
the shorter maturity term structure about future inflation,”
Journal of International Money and Finance, vol. 10, no. 1,
pp. 2–22, 1991.
[13] V. Kotlan, “'e term structure of interest rates and future ´
inflation,” Eastern European Economics, vol. 37, no. 5,
pp. 36–51, 1999.
[14] N. R. Sari, W. F. Mahmudy, and A. P. Wibawa, “Inflation rate
forecasting through adaptive neuro fuzzy inference system,”
AICIT, vol. 8, no. 1, pp. 11–19, 2017.
[15] M. H. Pesaran, T. Schuermann, and L. V. Smith, “Forecasting
economic and financial variables with global VARs,” International Journal of Forecasting, vol. 25, no. 4, pp. 642–675,
2009.
[16] P. McAdam and P. McNelis, “Forecasting inflation with thick
models and neural networks,” Economic Modelling, vol. 22,
no. 5, pp. 848–867, 2005.
[17] F. I. Estiko and W. Wahyuddin, “Analysis of Indonesia’s
inflation using ARIMA and artificial neural network,” Economics Development Analysis Journal, vol. 8, no. 2, pp. 151–
162, 2019.


Main Data Sets : https://github.com/jaronritter01/InflationRatePrediction
