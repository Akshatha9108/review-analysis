App link: https://review-analysis.streamlit.app/
---

# Customer Sentiment Analyzer

## Overview

The Customer Sentiment Analyzer is a machine learning application designed to analyze customer reviews and determine their sentiment. This tool is built using Python and leverages natural language processing techniques to classify reviews as either positive or negative. The application is implemented using Streamlit for an interactive web interface.

## Project Components

- **`app.py`**: The main Streamlit application script that provides the user interface for inputting reviews and displaying sentiment predictions.
- **`flipkart_reviews_dataset.csv`**: A dataset of customer reviews from Flipkart used for training and evaluation.
- **`model.sav`**: The trained machine learning model saved using `joblib` for sentiment classification.
- **`tfidf.sav`**: The saved TF-IDF vectorizer used for converting text data into numerical features.
- **`Sentiment_Analysis.ipynb`**: Jupyter Notebook for exploratory data analysis, model training, and evaluation.
- **`README.md`**: Documentation file that provides an overview of the project and instructions for usage.
- **`requirements.txt`**: List of Python packages and dependencies required to run the project.

## Installation

To run the Customer Sentiment Analyzer, you need to set up a Python environment and install the necessary dependencies. Follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/customer-sentiment-analyzer.git
   cd customer-sentiment-analyzer
   ```

2. **Create and Activate a Virtual Environment**:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows use `env\Scripts\activate`
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Streamlit Application**:
   ```bash
   streamlit run app.py
   ```

## Usage

1. Open the Streamlit app in your browser (usually accessible at `http://localhost:8501`).
2. Enter a customer review into the text input field.
3. Click the "Predict sentiment" button to analyze the sentiment of the review.
4. The application will display whether the review is positive or negative based on the model's prediction.

## Components Explained

- **Text Cleaning Function (`text_clean`)**: Processes and cleans the input text to prepare it for sentiment analysis, including lowercasing, removing special characters, and lemmatizing words.
- **Prediction Function (`predict`)**: Uses the trained model and TF-IDF vectorizer to classify the sentiment of the cleaned review.
- **Streamlit Interface (`app.py`)**: Provides a user-friendly interface for inputting reviews and displaying results.

## Dependencies

The project requires the following Python packages:

- `streamlit`
- `joblib`
- `pandas`
- `numpy`
- `nltk`
- `re`
- `scikit-learn` (for model and vectorizer)

Install all dependencies using the `requirements.txt` file.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or issues, please contact akshatha7011@gmail.com 

---

Feel free to adjust the content to better fit your project specifics or personal preferences!
