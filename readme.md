# Laptop Price Prediction

This project is build to predict the price range of the laptop by analysing the configuration and specifications details.

Following steps are invloved in the project:
* Data Exploration and Visualization
* Exploratory Data Analysis and Data Cleaning
* Model Building (Linear, Lasso, Ridge, Decision Tree, Random Forest)
* Hyperparameter tuning the best resulting model (Decisiton Tree, Random Forest)
* Creating the Pickle file of the best performing model
* Building the UI for deploying the model

## Data Preparation for Modeling
* Extracted new informative features from the existing feature(containing text information) for accurate predictions. (Example: Touchscreen, IPS feature were created from Screen Resolution)
* Performed log distribution on target feature to convert it into gaussian distribution.
* New Feature namely PPI was created using the values of Screen Resolution and Display Size.
* Multicollinearity issues were solved using feature engineering technique.
* Used Column Transformer class to perform one hot encoding on the categorical features without disturbing the numerical features.
* Created a pipeline for feature transformation using column transformer and training the model on the dataset.

## Moedling
* Trained and tested various algorithm for R2 value and Mean Absolute Error.
* Performed hyperparameter tuning for Random Forest and Decision Tree algorithm by finding the effective aplha values of subtrees using cost complexity pruning path function.
* Created the Pickle File of the model for intergrating it with UI to perform real time predictions of the laptop price.



