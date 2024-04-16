# neural-network-challenge-1
Module 18 Challenge

## Objective:
The code aims to build, train, and evaluate a neural network model to predict credit rankings using student loan data.

## Steps:

1. **Data Loading**: 
   - The code begins by loading student loan data from a CSV file hosted online.

2. **Data Preprocessing**:
   - The target variable (`credit_ranking`) is separated from the features (`X`).
   - The features are scaled using `StandardScaler` to normalize the data.

3. **Model Architecture**:
   - A Sequential neural network model is initialized.
   - Two hidden layers with ReLU activation functions are added.
   - An output layer with a sigmoid activation function is added for binary classification.

4. **Model Compilation**:
   - The model is compiled with binary cross-entropy loss and the Adam optimizer.
   - The accuracy metric is used to evaluate the model during training.

5. **Model Training**:
   - The model is trained using the training data (`X_train_scaled` and `y_train`) for 50 epochs.

6. **Model Evaluation**:
   - The trained model is evaluated using the test data (`X_test_scaled` and `y_test`).
   - Test loss and accuracy are printed to assess model performance.

7. **Predictions**:
   - The model is used to make predictions on the test data.
   - Predictions are rounded to binary values (0 or 1) based on a threshold of 0.5.

8. **Evaluation Metrics**:
   - Classification report is printed, which includes precision, recall, F1-score, and support for each class.
   - These metrics provide a detailed assessment of model performance on the test data.

## Result:
The result of running the code includes:
- Test loss and accuracy of the trained model.
- Classification report showing precision, recall, F1-score, and support for each class.
- The model file (`student_loans.keras`) is saved for future use.

## Acknowlegements:
I extend my gratitude to academic instruction, DataCamp, and the Stack Overflow community for their invaluable contributions to this project. Academic instruction provided the foundational knowledge and guidance essential for tackling data analysis challenges, while DataCamp's interactive courses and hands-on exercises significantly enhanced my skills and techniques. Moreover, the Stack Overflow community's wealth of discussions and solutions offered insights, problem-solving approaches, and best practices crucial for overcoming obstacles encountered during development. Together, these sources have played a pivotal role in shaping my understanding and proficiency in data analysis, for which I am sincerely thankful.