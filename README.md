# Email Spam Classifier Using Machine Learning

An end-to-end Python-based Machine Learning project that classifies emails as either **Spam** or **Ham (Legitimate)**. This project demonstrates how to process text data and apply a classification algorithm to solve a real-world Natural Language Processing (NLP) problem.

## 🚀 Project Overview
Text-based communication often contains unsolicited or malicious content. This project builds a predictive pipeline that takes raw email text, extracts meaningful numerical features, and accurately classifies whether the email is safe or spam.

## 📊 Dataset
The project utilizes a dataset named `mail_data.csv`, which contains two primary columns:
- `Category`: The target label (`spam` or `ham`).
- `Message`: The raw text content of the email.

## 🛠️ Tech Stack & Libraries
* **Python 3**
* **Jupyter Notebook** (Development environment)
* **Pandas & NumPy**: For data manipulation, handling missing values, and exploratory analysis.
* **Scikit-Learn (Sklearn)**:
  * `TfidfVectorizer`: To convert text data into a matrix of TF-IDF (Term Frequency-Inverse Document Frequency) features.
  * `train_test_split`: To split the data cleanly into training and testing sets.
  * `LogisticRegression`: The classification model used to train and make predictions.
  * `metrics.accuracy_score`: To evaluate the performance of the model.

## 📈 Workflow
1. **Data Preprocessing:** Handled null values and performed label encoding (`spam` $\rightarrow$ `0`, `ham` $\rightarrow$ `1`).
2. **Feature Extraction:** Transformed text messages into feature vectors using `TfidfVectorizer` (ignoring English stop words and converting to lowercase).
3. **Model Training:** Split the data into an 80/20 train-test ratio and trained a **Logistic Regression** model.
4. **Evaluation:** Evaluated the model using accuracy scores on both training and testing datasets to check for overfitting/underfitting.

## 💻 How to Run This Project
1. Clone this repository or download the files.
2. Ensure you have Anaconda or Python installed along with the required libraries:
   ```bash
   pip install numpy pandas scikit-learn
