# SUPERVISED-LEARNING_1
This script explores supervised learning using decision trees for classification tasks. It utilizes the classic "Golf" dataset to predict whether or not someone will play tennis based on weather conditions.

Data Analysis and Visualization

The code defines sample weather data (outlook, temperature, humidity, wind) and corresponding labels (play tennis or not) for 14 instances.

Data Preprocessing

Label encoding is applied to convert categorical features (outlook, temperature, humidity, wind, play) into numerical representations for the decision tree model.
Decision Tree Model

Model Definition and Training:

A decision tree classifier is created using sklearn.tree.DecisionTreeClassifier.
The model is trained on the encoded features and labels.
Feature Importance:

The .feature_importances_ attribute reveals the importance of each feature in making predictions. Higher values indicate greater influence on the decision-making process.
Prediction:

The code demonstrates how to use the trained model to predict the play decision for a new data point (Overcast, Mild, Normal, Strong).
classifier.predict_proba provides probability distributions over labels, allowing for a more nuanced understanding of the prediction.
Evaluation:

Cross-validation with 5 folds is used to evaluate the model'sgeneralizability. The code calculates average accuracy across folds.
Visualization:

While not explicitly shown, the code can be used to visualize the decision tree using sklearn.tree.plot_tree. Analyzing this tree structure can provide insights into the decision-making logic.
Random Forest Classifier

Model Definition and Training:

A Random Forest classifier is created using sklearn.ensemble.RandomForestClassifier. This ensemble method combines multiple decision trees for potentially better performance.
Hyperparameter Tuning (Optional):

The code includes a commented-out section referencing documentation for exploring hyperparameter tuning options. Tuning these parameters can influence model complexity and accuracy.
Evaluation:

Similar to the decision tree, the Random Forest is evaluated using 5-fold cross-validation, and average accuracy is reported.
Conclusion

This script demonstrates the fundamentals of decision trees and Random Forests for classification tasks. It explores feature importance, prediction, and evaluation using cross-validation. By comparing the performance of both models, you can gain insights into the potential benefits of ensemble methods.
