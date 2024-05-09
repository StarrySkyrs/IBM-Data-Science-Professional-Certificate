# 7. Data Analysis with Python
## 7.1 Week 1 Summary
- Each line in a dataset is a row, and commas separate the values.

- To understand the data, you must analyze the attributes for each column of data.

- Python libraries are collections of functions and methods that facilitate various functionalities without writing code from scratch and are categorized into Scientific Computing, Data Visualization, and Machine Learning Algorithms.

- Many data science libraries are interconnected; for instance, Scikit-learn is built on top of NumPy, SciPy, and Matplotlib.

- The data format and the file path are two key factors for reading data with Pandas.

- The read_csv method in Pandas can read files in CSV format into a Pandas DataFrame.

- Pandas has unique data types like object, float, Int, and datetime.

- Use the dtype method to check each column’s data type; misclassified data types might need manual correction.

- Knowing the correct data types helps apply appropriate Python functions to specific columns.

- Using Statistical Summary with describe() provides count, mean, standard deviation, min, max, and quartile ranges for numerical columns.

- You can also use include='all' as an argument to get summaries for object-type columns.

- The statistical summary helps identify potential issues like outliers needing further attention.

- Using the info() Method gives an overview of the top and bottom 30 rows of the DataFrame, useful for quick visual inspection.

- Some statistical metrics may return "NaN," indicating missing values, and the program can’t calculate statistics for that specific data type.

- Python can connect to databases through specialized code, often written in Jupyter notebooks.

- SQL Application Programming Interfaces (APIs) and Python DB APIs (most often used) facilitate the interaction between Python and the DBMS.

- SQL APIs connect to DBMS with one or more API calls, build SQL statements as a text string, and use API calls to send SQL statements to the DBMS and retrieve results and statuses.

- DB-API, Python's standard for interacting with relational databases, uses connection objects to establish and manage database connections and cursor objects to run queries and scroll through the results.

- Connection Object methods include the cursor(), commit(), rollback(), and close() commands.

- You can import the database module, use the Connect API to open a connection, and then create a cursor object to run queries and fetch results.

- Remember to close the database connection to free up resources.
## 7.2 Week 2 Summary
- Data formatting is critical for making data from various sources consistent and comparable.

- Master the techniques in Python to convert units of measurement, like transforming "city miles per gallon" to "city-liters per 100 kilometers" for ease of comparison and analysis.

- Acquire skills to identify and correct data types in Python, ensuring the data is accurately represented for subsequent statistical analyses.

- Data normalization helps make variables comparable and helps eliminate inherent biases in statistical models.

- You can apply Feature Scaling, Min-Max, and Z-Score to normalize data and apply each technique in Python using pandas’ methods.

- Binning is a method of data pre-processing to improve model accuracy and data visualization.

- Run binning techniques in Python using numpy's "linspace" and pandas' "cut" methods, particularly for numerical variables like "price."

- Utilize histograms to visualize the distribution of binned data and gain insights into feature distributions.

- Statistical models generally require numerical inputs, making it necessary to convert categorical variables like "fuel type" into numerical formats.

- You can implement the one-hot encoding technique in Python using pandas’ get_dummies method to transform categorical variables into a format suitable for machine learning models.
## 7.3 Week 3 Summary
- Tools like the 'describe' function in pandas can quickly calculate key statistical measures like mean, standard deviation, and quartiles for all numerical variables in your data frame.

- Use the 'value_counts' function to summarize data into different categories for categorical data.

- Box plots offer a more visual representation of the data's distribution for numerical data, indicating features like the median, quartiles, and outliers.

- Scatter plots are excellent for exploring relationships between continuous variables, like engine size and price, in a car dataset.

- Use Pandas' 'groupby' method to explore relationships between categorical variables.

- Use pivot tables and heatmaps for better data visualizations.

- Correlation between variables is a statistical measure that indicates how the changes in one variable might be associated with changes in another variable.

- When exploring correlation, use scatter plots combined with a regression line to visualize relationships between variables.

- Visualization functions like regplot, from the seaborn library, are especially useful for exploring correlation.

- The Pearson correlation, a key method for assessing the correlation between continuous numerical variables, provides two critical values—the coefficient, which indicates the strength and direction of the correlation, and the P-value, which assesses the certainty of the correlation.

- A correlation coefficient close to 1 or -1 indicates a strong positive or negative correlation, respectively, while one close to zero suggests no correlation.

- For P-values, values less than .001 indicate strong certainty in the correlation, while larger values indicate less certainty. Both the coefficient and P-value are important for confirming a strong correlation.

- Heatmaps provide a comprehensive visual summary of the strength and direction of correlations among multiple variables.
## 7.4 Week 4 Summary
- Linear regression refers to using one independent variable to make a prediction.

- You can use multiple linear regression to explain the relationship between one continuous target y variable and two or more predictor x variables.

- Simple linear regression, or SLR, is a method used to understand the relationship between two variables, the predictor independent variable x and the target dependent variable y.

- Use the regplot and residplot functions in the Seaborn library to create regression and residual plots, which help you identify the strength, direction, and linearity of the relationship between your independent and dependent variables.

- When using residual plots for model evaluation, residuals should ideally have zero mean, appear evenly distributed around the x-axis, and have consistent variance. If these conditions are not met, consider adjusting your model.

- Use distribution plots for models with multiple features: Learn to construct distribution plots to compare predicted and actual values, particularly when your model includes more than one independent variable. Know that this can offer deeper insights into the accuracy of your model across different ranges of values.

- The order of the polynomials affects the fit of the model to your data. Apply Python's polyfit function to develop polynomial regression models that suit your specific dataset.

- To prepare your data for more accurate modeling, use feature transformation techniques, particularly using the preprocessing library in scikit-learn, transform your data using polynomial features, and use the modules like StandardScaler to normalize the data.

- Pipelines allow you to simplify how you perform transformations and predictions sequentially, and you can use pipelines in scikit-learn to streamline your modeling process.

- You can construct and train a pipeline to automate tasks such as normalization, polynomial transformation, and making predictions.

- To determine the fit of your model, you can perform sample evaluations by using the Mean Square Error (MSE), using Python’s mean_squared_error function from scikit-learn, and using the score method to obtain the R-squared value.

- A model with a high R-squared value close to 1 and a low MSE is generally a good fit, whereas a model with a low R-squared and a high MSE may not be useful.

- Be alert to situations where your R-squared value might be negative, which can indicate overfitting.

- When evaluating models, use visualization and numerical measures and compare different models.

- The mean square error is perhaps the most intuitive numerical measure for determining whether a model is good.

- A distribution plot is a suitable method for multiple linear regression.

- An acceptable r-squared value depends on what you are studying and your use case.

- To evaluate your model’s fit, apply visualization, methods like regression and residual plots, and numerical measures such as the model's coefficients for sensibility:

  - Use Mean Square Error (MSE) to measure the average of the squares of the errors between actual and predicted values and examine R-squared to understand the proportion of the variance in the dependent variable that is predictable from the independent variables.

  - When analyzing residual plots, residuals should be randomly distributed around zero for a good model. In contrast, a residual plot curve or inaccuracies in certain ranges suggest non-linear behavior or the need for more data.
## 7.5 Week 5 Summary
- How to split your data using the train_test_split() method into training and test sets. You use the training set to train a model, discover possible predictive relationships, and then use the test set to test your model to evaluate its performance.

- How to use the generalization error to measure how well your data does at predicting previously unseen data.

- How to use cross-validation by splitting the data into folds where you use some of the folds as a training set, which we use to train the model, and the remaining parts are used as a test set, which we use to test the model. You iterate through the folds until you use each partition for training and testing. At the end, you average results as the estimate of out-of-sample error.

- How to pick the best polynomial order and problems that arise when selecting the wrong order polynomial by analyzing models that underfit and overfit your data.

- Select the best order of a polynomial to fit your data by minimizing the test error using a graph comparing the mean square error to the order of the fitted polynomials.

- You should use ridge regression when there is a strong relationship among the independent variables.

- That ridge regression prevents overfitting.

- Ridge regression controls the magnitude of polynomial coefficients by introducing a hyperparameter, alpha.

- To determine alpha, you divide your data into training and validation data. Starting with a small value for alpha, you train the model, make a prediction using the validation data, then calculate the R-squared and store the values. You repeat the value for a larger value of alpha. You repeat the process for different alpha values, training the model, and making a prediction. You select the value of alpha that maximizes R-squared.

- That grid search allows you to scan through multiple hyperparameters using the Scikit-learn library, which iterates over these parameters using cross-validation. Based on the results of the grid search method, you select optimum hyperparameter values.

- The GridSearchCV() method takes in a dictionary as its argument where the key is the name of the hyperparameter, and the values are the hyperparameter values you wish to iterate over.
