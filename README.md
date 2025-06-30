AI-ML-Task5

1. Import Libraries

          Loads essential tools:
                > pandas, numpy – data handling
                > matplotlib, seaborn – visualizations
                > sklearn – machine learning models & evaluation tools

2. Loading and Exploring the Dataset

         > The dataset heart.csv is loaded using pandas.
         > Functions like .describe(), .info(), and .isnull().sum() help summarize the dataset.
         > This step confirms that the dataset is clean and ready for modeling (no missing values).


3. Preparing the Data

         > The target column (which indicates heart disease presence) is separated from the feature columns.
         > The dataset is split into training (80%) and testing (20%) sets using train_test_split.
         > This ensures we train the model on one part and test its performance on unseen data.

4. Decision Tree Classifier

         > A basic decision tree is trained using the training data.
         > Predictions are made on the test set, and model performance is evaluated using:
                     > Accuracy
                     > Classification report (precision, recall, f1-score)
                     > Confusion matrix (visualized with seaborn.heatmap)
         > The full tree is visualized using plot_tree(), showing the structure of decision rules.

5. Pruned Decision Tree

         > A simplified decision tree is trained with a limited depth (max_depth=3).
         > This avoids overfitting and makes the tree easier to interpret.
         > Its performance is also evaluated and visualized.

6. Random Forest Classifier

         > A Random Forest model is trained, which is an ensemble of many decision trees.
         > It provides better accuracy and robustness by averaging results from multiple trees.
         > Again, accuracy and classification report are printed.

7. Feature Importance

         > The model shows how important each input feature (like age, cholesterol) is in predicting heart disease.
         > A bar plot visualizes these importances, giving insights into which features matter most.

8. Cross-Validation

         > 5-fold cross-validation is performed on both the pruned decision tree and the random forest.
         > This tests the model’s performance across different subsets of the data, ensuring it’s reliable and consistent.




