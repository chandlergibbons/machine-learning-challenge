# machine-learning-challenge

Althought the data itself including all the starting parameters speak of astronomy related mesurements that I struggle to understand, I found that my GridSearchCV tuned random forest model preformed much better than my logistical regression model. The score for the logistical regression model score was roughly .26 where as the random forest tuned model score was roughly 0.89. Significantly better on the tuned model. The best score of this random forest model occures when the nodes expand until all leaves are pure or until all leaves contain less than min_samples_split samples. Also when the max features at each split is 16. The criteria required to produce this score also requires a minimum sample size of 2 to split an internal node. All the parameters that produce this best score of .89 they can be found here: 

{'classifier': RandomForestClassifier(bootstrap=True, ccp_alpha=0.0, class_weight=None,
                       criterion='gini', max_depth=None, max_features=16,
                       max_leaf_nodes=None, max_samples=None,
                       min_impurity_decrease=0.0, min_impurity_split=None,
                       min_samples_leaf=1, min_samples_split=2,
                       min_weight_fraction_leaf=0.0, n_estimators=90,
                       n_jobs=None, oob_score=False, random_state=None,
                       verbose=0, warm_start=False), 'classifier__max_features': 16, 'classifier__n_estimators': 90}
                       
When tuneing my random forest model with GridSearchCV I tried to work efficently by passing in parameters to the param_grid that wouldnt take my computer forever to tune. like modifying the classifier__n_estimators and classifier__max_features from the documentation I found to be more realistic goals/tasks for my comupter to handle. Even doing so my computer ran harder then I have ever heard it run before and it did so for roughly 7.6min. 
                       
 
