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


🚀 Deployment

📥 Input new employee data

- New employee information is entered directly as a dictionary or a DataFrame.

🧼 Convert categorical columns to numeric format

- Categorical variables like Education, Gender, City, and EverBenched are converted using One-Hot Encoding (get_dummies()).

🧩 Align columns with what the model expects

- Check if any columns used during training are missing in the new data; if so, add them with default value 0.

- Make sure the column order matches the training data.

📏 Scale the data using the same scaler

- Use the StandardScaler instance that was fit during training to transform the new data accordingly (without saving/loading from disk).

🧠 Make predictions using the trained ANN model

- Feed the scaled data into the trained ANN model to get predictions (whether the employee will leave or not).

📋 Add the prediction to the results

- Append the prediction (e.g., a leaveornot column with values 0 or 1) to the original data to present the final result.
