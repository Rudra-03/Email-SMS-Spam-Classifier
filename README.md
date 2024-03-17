
# Email/SMS Spam Classifier
This project aims to classify email or SMS messages into two categories: spam or not spam (ham). It utilizes natural language processing techniques along with machine learning to achieve this classification.





## Installation
To run this project, ensure you have Python installed on your system. Then, follow these steps:

    1. Clone this repository to your local machine:
    
        git clone https://github.com/Rudra-03/Email-SMS-Spam-Classifier.git

    2. Navigate to the project directory:

        cd Email-SMS-Spam-Classifier

    3. Install the required dependencies using pip:

        pip install -r requirements.txt

    
## Usage

After installing the dependencies, you can run the application using Streamlit. Streamlit provides a convenient way to create interactive web applications for machine learning projects.

To start the application, execute the following command in your terminal:

    streamlit run app.py

Once the application is running, you will see a text area where you can enter your email or SMS message. Click on the "Predict" button to classify the message as spam or not spam.

## How it Works

The classification process involves the following steps:

    1. Preprocessing: The input message undergoes preprocessing, which includes converting the text to lowercase, tokenizing it into words, removing non-alphanumeric characters, and stemming the words using the Porter stemming algorithm.

    2. Vectorization: The preprocessed message is then transformed into a numerical representation using TF-IDF vectorization. This step converts the text into a vector of numerical values, which can be used as input for machine learning models.

    3. Prediction: The vectorized input is fed into a pre-trained machine learning model, which predicts whether the message is spam or not spam.

    4. Display: Finally, the application displays the prediction result, indicating whether the message is classified as spam or not.
## Files

    1. app.py: Python script containing the Streamlit application code, including preprocessing, vectorization, prediction, and user interface.

    2. requirements.txt: File listing the dependencies required to run the project, including Streamlit, NLTK, and scikit-learn.

    3. vectorizer.pkl: Pickle file containing the pre-trained TF-IDF vectorizer used for text vectorization.
    
    4. model.pkl: Pickle file containing the pre-trained machine learning model used for classification.
## Acknowledgements

- This project was developed using Streamlit, NLTK, and scikit-learn libraries.
- The machine learning model was trained using a dataset of labeled email/SMS messages.
- Special thanks to the developers of Streamlit, NLTK, and scikit-learn for their contributions to the field of machine learning and natural language processing.