# SpamSense, Spam SMS Detection System: A Machine Learning-Based Approach
SpamSense is an intelligent SMS filtering system that leverages natural language processing and machine learning techniques to accurately classify text messages as spam or legitimate communications, helping users avoid unwanted and potentially harmful messages.

## Task Objectives

- Build a machine learning system for SMS spam detection
- Implement text preprocessing techniques including lowercasing, tokenization, stopword removal, and stemming
- Create a custom NLTK classifier wrapper for scikit-learn models
- Train a Naive Bayes classifier on SMS data
- Evaluate model performance using accuracy, precision, recall, and F1-score
- Save and load models for future use

## Steps to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/username/SpamSMSDetection.git
cd SpamSMSDetection
```

### 2. Set Up a Virtual Environment

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Prepare the Dataset

- Ensure the `spam.csv` file is placed in the `data` directory in the root directory
- The dataset should contain SMS messages labeled as 'spam' or 'ham'

### 5. Train the Model

```bash
cd src
python main.py
```

This will:
- Load and preprocess the SMS data
- Train a Naive Bayes classifier
- Evaluate the model's performance
- Save the trained model and vectorizer to the `models` directory

### 6. Test the Model

Return to the project root directory and run the test script:

```bash
# From the project root
cd ..
python test.py
```

This will:
- Load the saved model and vectorizer
- Test the model on example SMS messages
- Display the classification results

## 7. Run the Application

After testing the model, you can use the interactive application to classify your own SMS messages.

### **Usage:**
Run the following command from the project root:

```bash
python application.py
```
This will:
- Load the saved model and vectorizer
- Start an interactive command-line interface
- Allow you to enter SMS messages for real-time classification
- Display whether each message is classified as spam or legitimate
- Continue until you type 'exit' to quit the application

## 8. Run the Web Application

After testing the model with the command-line interface, you can use the web application for a more user-friendly experience.

### **Usage:**
Run the following commands from the project root:

```bash
python app.py
```
Open a browser interface at http://127.0.0.1:5000

### 9. Deactivate the Virtual Environment

When finished, deactivate the virtual environment:

```bash
deactivate
```

### Dataset:

The SMS Spam Collection is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages, tagged acording being ham (legitimate) or spam.
The files contain one message per line. Each line is composed by two columns: v1 contains the label (ham or spam) and v2 contains the raw text.

https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset?resource=download



---