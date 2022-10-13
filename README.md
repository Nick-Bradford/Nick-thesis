# Nick-thesis
Code and data used for my Honours Thesis "Recurrence quantification analysis and machine learning: Parameter extraction and feature selection" at the University of Western Australia, Applied Mathematics, 2022.

#Abstract
This thesis explores recurrence techniques in the context of machine learning for time series parameter extraction of a benchmark dynamical system. We trained both support vector machine and random forest models on a data set whose features were engineered using recurrence quantification analysis on a drifting R\"{o}ssler system. Specifically, to predict the bifurcation parameter $a$, through the window [0.3, 0.55]. This window exhibits both periodic and chaotic regimes for the R\"{o}ssler system, enabling a thorough simultaneous test of both, model time series parameter extraction capabilities and, feature engineering through recurrence quantification analysis. In addition, due to the inherent qualities of a random forest model, feature importance was also explored. The data set was created through a dynamical systems Julia package and read using Python. Based on a baseline regression accuracy measure, we found that model performance was adequate, but only for predictions during periodic regimes of the R\"{o}ssler system. Both models showed greater variance in predictions of chaotic regimes, especially during screw-type chaotic regimes. Regression results demonstrated $R^2$ scores on the training set of approximately 0.974 and 0.996 for the support vector machine and random forest model, respectively. For the test set, the scores were 0.966 and 0.976 respectively. These findings indicate that the current dynamic regime heavily influences the accuracy prediction for both models. For the random forest model, we found that recurrence rate was the most critical feature by a large margin, with a standardised feature importance value of over 0.5. For our simulations, the recurrence rate was fixed at approximately 2\%. However, slight fluctuations in the recurrence rate did occur, indicating that small variations in the recurrence rate conveys important information for time series parameter extraction using a random forest model. We also show that recurrence time features are collectively the next most important type of feature.
