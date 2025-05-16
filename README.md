# Prediction-of-Emp-Churn-Using-ANN

🔧 Preprocessing Steps


🧹 Data Cleaning:

- Handled missing values and checked data consistency before further processing.

🧬 Categorical Encoding:

- Transformed categorical variables into numeric using Label Encoding and One-Hot Encoding depending on the nature of the feature.

📊 Feature Separation:

- Identified and separated categorical and numerical features to apply appropriate transformations.

📏 Feature Scaling:

- Applied StandardScaler to normalize numerical features for faster and more stable model training.

🎯 Target Preparation:

- Converted the target variable into binary format suitable for binary classification with neural networks.


🏗️ Modeling with Artificial Neural Network (ANN)

🧱 Model Architecture: -Built a deep learning model using Keras Sequential API:

- Input layer matching feature dimensions

-
- Hidden layers with ReLU activation

- Dropout layers to prevent overfitting

- Output layer with Sigmoid activation for binary classification

🎛️ Hyperparameter Tuning with Optuna:

- Used Optuna to find optimal values for:

- Number of hidden layers and neurons

- Activation functions

- Learning rate

- Batch size and number of epochs

🧪 Model Training & Evaluation: -Trained the optimized ANN using best hyperparameters. Evaluated performance using:

- Accuracy

- Precision, Recall, F1-Score

- ROC-AUC
