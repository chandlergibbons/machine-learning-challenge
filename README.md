# machine-learning-challenge

Althought the data itself including all the starting parameters peak of astronomy related mesurements that I struggle to understand, I found that my GridSearchCV tuned random forest model preformed much better than my logistical regression model. The score for the logistical regression model score was roughly .26 where as the random forest tuned model score was roughly 0.89. Significantly better on the tuned model. Although I dont have a solid understanding of the parameters that produce this best score of .89 they can be found here: 

{'classifier': RandomForestClassifier(bootstrap=True, ccp_alpha=0.0, class_weight=None,
                       criterion='gini', max_depth=None, max_features=16,
                       max_leaf_nodes=None, max_samples=None,
                       min_impurity_decrease=0.0, min_impurity_split=None,
                       min_samples_leaf=1, min_samples_split=2,
                       min_weight_fraction_leaf=0.0, n_estimators=90,
                       n_jobs=None, oob_score=False, random_state=None,
                       verbose=0, warm_start=False), 'classifier__max_features': 16, 'classifier__n_estimators': 90}
                       
                       
 