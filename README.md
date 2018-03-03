# LassoLogisticRegression-ClassificationTree-Bagging-RandomForests-Boosting-NeuralNetwork
The rehabilitation data set contains 1 binary response variable (acceptable vs unacceptable phonation during rehabilitation) and 310 real-valued predictors. The aim is to use the 310 features to predict the binary response, and identify the top 5 predictors. To solve this problem, I implement and compare six classification methods – Lasso Logistic Regression, Classification Tree, Bagging, Random Forests, Boosting, and Neural Networks – in terms of training and test misclassification errors. I split the dataset randomly into half training and half test data before model fitting, and this procedure is repeated multiple times to obtain a stable result of misclassification rates. The obtained training and test misclassification rates are presented in below figure. Neural Networks outperforms the other five methods with small training and test misclassification rates. 
 
In terms of interpretability, Regression Tree yields the best interpretable results since it provides a clear tree structure.
 
In addition, Lasso Logistic Regression performs variable selection by shrinking some coefficients to zero. From the solution path, it is found that the top 5 predictors are follows. 

V4: Jitter..F0_PQ5_classical_Baken
V110: X12th.delta
V37: Shimmer..Ampl_PQ5_classical_Baken
V103: X5th.delta
V42: Shimmer..Ampl_abs0th_perturb
