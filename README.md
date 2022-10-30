# Purpose
Predict the availability of rooms for reservation in USF’s library using Machine Learning

# Result
Built a machine learning model that can predict the availability of USF study room reservations accurately 94% of the time

# Technique used:
## Exploratory Data Analysis
- matplotlib, pandas, and seaborn to create graph the shows the correlation between variables.
- pd.groupby() to aggregate features to find pattern between variables

## Feature Engineering and Machine Learning
- Trained 11 classification models with default hyperparameters to shortlist promising model
- Automated the training and scoring process by writing a custom function named `train_and_score`
- Feature Engineering by creating polynomial features, interactions terms, and a new `floor` variable extracting from the `room` variable
- Combined feature engineering functions with sklearn's pipeline to quickly implement changes from the train set to the test set
- Built a custom transformer to add to the pipeline.
- Used k-fold cross validation instead of creating a validation set to utilize all the dataset for training
- Tuned Random Forest Classifier using the original data to improve the performance of the model and reach the accuracy score of 94% on the test set




