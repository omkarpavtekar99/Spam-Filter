**# Spam Filter Project**

**# Project Overview**

The Spam Filter Project is designed to classify emails as either "spam" or "ham" (not spam) using a machine learning approach. The project leverages a Logistic Regression model trained on a dataset of labeled emails. The emails are first preprocessed and transformed into feature vectors using TF-IDF (Term Frequency-Inverse Document Frequency), a common technique in natural language processing (NLP) for converting text data into numerical features.

**# Key Components**

**- Dependencies:**

- The project utilizes several libraries, including numpy, pandas, scikit-learn, for data handling, feature extraction, model building, and evaluation.

**- Data Collection and Preprocessing:**

- The dataset, mail_data.csv, contains email messages categorized as "spam" or "ham".
- Data is loaded into a Pandas DataFrame, where null values are replaced with empty strings.
- The data is then labeled, with "spam" emails marked as 0 and "ham" emails marked as 1.
- The dataset is split into training and testing sets for model evaluation.

**# Label Encoding:**

- The target labels (Category) are encoded as integers (0 for spam and 1 for ham).
- The messages (Message) serve as input features, while the encoded labels (Category) act as the target variable.

**#Feature Extraction:**

- TF-IDF Vectorization is employed to convert the text data into numerical feature vectors, making it suitable for model training.
- The vectorized data is then used to train a Logistic Regression model.

**# Model Training:**

- A Logistic Regression model is trained using the feature vectors from the training data.
- The model is evaluated on both training and test datasets, achieving high accuracy on both.

**#Model Evaluation:**

- The model's accuracy on the training data is approximately 96.70%, while on the test data, it is around 96.59%.
- These results indicate that the model is highly effective at distinguishing between spam and ham emails.

**# Building a Predictive System:**

- A predictive system is created where new email messages can be inputted and classified as either "spam" or "ham" using the trained Logistic Regression model.

**# Usage**

To use the spam filter:

**Data Preparation:**

- Ensure that your dataset is in a CSV format similar to mail_data.csv with Category and Message columns.

**Training the Model:**

- Use the provided notebook to preprocess your data, extract features using TF-IDF, and train the Logistic Regression model.

**Predicting New Data:**

- Input new email messages into the predictive system to determine if they are spam or ham.

**#Installation**

To run the project, ensure you have the following Python packages installed:
```
pip install numpy pandas scikit-learn
```

**#Conclusion**

The Spam Filter Project demonstrates a straightforward yet effective approach to email classification using machine learning techniques. By following the steps in the notebook, users can build and deploy their own spam detection system.
