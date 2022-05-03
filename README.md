CSCE 5218 Final Report
The Importance of the hyperparameters tuning tools, Grid Search Cross Validation and Random Search Cross Validation



Group Members
Tanakit Phamornratanakun (11345560)
Chandrasekaran Isabella Jaya Rani (11504607)


Introduction
The Importance of the hyperparameters tuning tools, Grid Search Cross Validation and Random Search Cross Validation. In the past few years, tuning parameters for machine learning models were problematic, time-consuming, complex codes and extra steps and processes with random directions. This project wants to explore more about the performance and effectiveness of Grid Search Cross Validation and Random Search Cross Validation, one of the packages from Scikit-Learn library, combined with a few machine learning algorithms. We use Thera Bank dataset which is a Binary Classification problem which means that there are only 2 classes for the prediction.
Related Work
 Our group will follow the data preprocessing method from ADITYA KADIWAL thread from Kaggle shared code. Using his Exploratory Data Analysis as reference for our project. In the model selection part, we used the code example from the Great Learning website which provides the basic concepts of GridSearchCV technique.
Method
After applying a general preprocessing method, dropping 0 values and unreasonable values, we run models with 4 algorithms, and 3 model selection techniques with 12 combinations of hyperparameters. We selected Logistic Regression and Decision Tree Classification from the Scikit-Learn library as shallow learning algorithms because they are two of the most popular shallow learning algorithms in the present. We also selected Multi-layer Perceptron and Feed Forward Neural Network as Deep Learning algorithms. Cross validation, Grid Search Cross Validation and Random Search Cross Validation are 3 model selection techniques which are the main part of this project. Being used as the hyperparameters tuning tool, this model selection tool will select the set best of hyperparameters among 12 combinations in each algorithm.
Baseline and Evaluation Metrics
The baseline for this study is going to be 90% according to the class distribution of this problem is 90:10 ratio. In this study, we will measure performance and effectiveness of the models by using both accuracy and runtime which are built-in functions of Scikit-Learn. 
Results
The Thera Bank consists of 14 features including the class with 5000 records. The objective of this dataset is to identify the potential customers who have a higher probability of purchasing the loan.
There are 52 missing records that were excluded from the models. The class distribution is biased with a ratio of 9:1 for class 0 and class 1 respectively. 
Other than that, other features such as age, experience, education and family members are well-distributed. (Fig 1, 2, 3.). The heatmap shows that there are high correlations between class (personal loan) and household income(income), credit card average spending (CC Avg) and having a certificate of deposit with the bank (CD account). (Fig 4.)
Predicting the majority class of the dataset, class 0, the baseline model results in accuracy of 0.903031. run-time cannot be determined. Resulting in, all the 24 models perform better than the baseline model. (Fig 5, 6, 7, 8)
In conclusion, for shallow learning algorithms, Decision Tree Classification provides higher overall accuracy scores and lower runtime (in seconds).(Table 2, Fig 5, 6)
On the other hand, for deep learning algorithms, Feed Forward Neural Network provides higher overall accuracy scores. Both Multi-layer Perceptron and Feed Forward Neural Network have indifferent run time but significantly higher compared to shallow learning algorithms.(Table 2, Fig 7, 8)
For shallow learning algorithms, Cross Validation performs best in terms of run time while Random Search Cross Validation achieves the highest accuracy score without concern for overfitting.(Table 2.)(Table 2, Fig 5, 6)
On the other hand, for deep learning algorithms, Feed Forward Neural Network achieved higher overall accuracy scores. In terms of runtime, between Grid Search Cross Validation and Random Search Cross Validation has no difference, but both of them used less runtime than Cross Validation technique.(Table 2, Fig 7, 8)
 Discussion
Although, there is no significant difference in the amount of time for running the model on a small scale, the amount of time used for writing codes, having no concrete proof or evidence, is notably different. We can try 12 combinations of hyperparameters in the model tuning process with only 1 more line of code compared to no hyperparameter tuning coding, on the other hand, with no advance model selection techniques like Grid Search Cross Validation or Random Search Cross Validation, we have to write 12 more chunks of code and run it separately. 
Figures and Tables

Table 1: Example of Thera Bank Dataset

Figure 1: Example of  Univariate Analysis


Figure 2: Example of Bivariate Analysis


Figure 3: Example of  Pairplot


Figure 4: Heatmap of Thera Bank dataset’s features.

Table 2: Results of model using hyperparameter tuning tools.

Figure 5: Scatter plot of Logistic Regression algorithm results.



Figure 6: Scatter plot of Decision Tree Classification algorithm results.

Figure 7: Scatter plot of Multi-layer Perceptron algorithm results.

Figure 8: Scatter plot of Feed Forward Neural Network algorithm results.

Citations and Reference
https://www.mygreatlearning.com/blog/gridsearchcv/
https://www.analyticsvidhya.com/blog/2021/06/tune-hyperparameters-with-gridsearchcv/
https://www.kaggle.com/itsmesunil/bank-loan-modelling
https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html
https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html
https://scikit-learn.org/stable/modules/cross_validation.html?highlight=cross_validate
 https://www.mygreatlearning.com/blog/gridsearchcv/
