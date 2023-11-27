# Exoplanet habitability class and ESI prediction
This project, developed in June 2023, focuses on the analysis and classification of the habitability of exoplanets based on various features. The primary goals include identifying habitable exoplanets and predicting the Earth Similarity Index (ESI) of different celestial bodies.

## Authors
David Mathas, Adam Pohle & Can Efe Gursoy - June 2023

# Packages Used:
Pandas and NumPy: For data manipulation and analysis.
Matplotlib and Seaborn: For data visualization.
Scikit-learn and Imbalanced-learn: For machine learning tasks, resampling, and model evaluation.
TensorFlow and Keras: For building and training neural network models.
Statsmodels: For statistical analysis.

# Data Loading and Preliminary Analysis
The project starts with loading the exoplanet dataset from 'phl_exoplanet_catalog_2019.csv'.
Initial exploratory data analysis involves checking missing values, removing irrelevant columns, and visualizing habitability proportions.
Meaningful variables are identified, and columns with 100% completeness are retained.

# Data Cleaning and Imputation
Non-meaningful variables and those with multicollinearity are excluded.
Missing values are imputed using mode imputation and KNN imputation.
The dataset is further processed, combining two habitable classes and modifying the 'HABZONE' variable.

# Resampling and Splitting Data
The dataset is split into training and testing sets.
SMOTE-ENN resampling is applied to address class imbalance in the training set.

# Application of Classification Algorithms

# K-Nearest Neighbors (KNN):
The KNN classifier is evaluated with different numbers of neighbors.
The classification report and confusion matrix provide insights into model performance.

# Neural Network (NN):
Hyperparameter optimization is performed using GridSearchCV.
The best model is built with TensorFlow and Keras.
The NN model is trained and evaluated, showcasing accuracy and confusion matrix.

# Numerical Prediction: Earth Similarity Index (ESI):
The project includes a numerical prediction task for ESI.
Regression models are built and evaluated for predicting ESI values.
Conclusion

This collaborative effort aims to contribute to the field of exoplanet analysis by combining machine learning techniques with astronomical data. The code and analysis provided here offer insights into the potential habitability of exoplanets and their Earth Similarity Index.

This project was part of the course Data Mining Techniques at the Vrije Universiteit Amsterdam (VU).
