# Machine-Learning---Boolean-Satisfiability-SAT-Dataset
This repository contains a solution jupyter notebook outlining ML techniques performed and appropriate SAT dataset files (test and train). 

## Dataset - Objective
The Boolean satisfiability (SAT) problem consists in determining whether a Boolean formula is satisfiable or not. This problem is one of the most widely studied combinatorial problems in computer science. It is the classic NP-complete problem. Over the past number of decades, a significant amount of research work has focused on solving SAT problems with both complete and incomplete solvers.

An extended version of the problem is Model Counting (#SAT). In #SAT the solver needs to compute the number of solutions of a Boolean formula. A wide variety of solvers have been designed to tackle this problem.

In this project, we want to create an Algorithm Selection (AS) approach to Model Counting. For each #SAT instance, there is a specific solver that works better than the others, the goal of your machine learing approach is to classify it.

In AS we represent #SAT problems with a vector of 72 features with general information about the problem, e.g., number of variables, number of clauses, etc. For each instance, there is a 'label' column representing the name of the optimal solver.

## Results 
After performing various pre-processing techniques such as Scaling, feature selection (PCA and Seelct Percentile), Cross Validation various Machine Learning techniques such as KNN, RandomForestClassifier, Gradient Boosting (GBM), LightGBM, XGBoosting and CatBoostClassifier were applied to determine the best model to use to test on the test dataset. The Catboost Classifier yielded the best validation accuracy of 77.80% and was used as the final model to test on the unseen test data. Test accuracy - 74.83%
