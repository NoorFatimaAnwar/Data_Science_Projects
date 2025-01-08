**Fake Reviews Detection System**
This project focuses on identifying fake reviews in e-commerce platforms using natural language processing (NLP) and machine learning techniques. By preprocessing raw review data and applying advanced classification algorithms, the system effectively distinguishes between genuine (CG) and fake reviews.

**Project Overview**
**Objectives:**
Detect fake reviews to enhance product reliability on e-commerce platforms.
Use preprocessing techniques to clean and analyze text data for meaningful insights.
Implement a voting classifier combining multiple algorithms for robust performance.

**Files in the Repository**
**1. Raw Dataset (fake_reviews_dataset.csv)**
Source: **Kaggle**
Contains the original data with the following columns:
Category: Product category.
Rating: Product rating.
Label: Indicates whether the review is genuine (CG) or fake.
Text: Full review text provided by users.

**2. Preprocessed Dataset (preprocessed_df.csv)**
Cleaned and transformed data ready for model training.
Additional columns include:
Cleaned Text: Reviews after removing stopwords, punctuation, and unnecessary characters.
Cleaned Text Length: Word count of the cleaned review.
Sentiment: Sentiment score based on review content.
Length Z-Score: Z-score of review length for statistical insights.

**3. Code File: fakeReviewsDetection_01.py**
Implements all preprocessing steps, including:
Stopword removal
Lemmatization
Sentiment analysis
Feature engineering (e.g., length z-scores)
Outputs the preprocessed dataset.

**4. Code File: fakeReviewsDetection_02.py**
Handles model training and testing using a Voting Classifier that combines:
Decision Tree
SVM
Logistic Regression
Linear Regression
Includes evaluation metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.

**How to Use**
**Clone the Repository:**
bash
Copy code
git clone https://github.com/yourusername/fake-reviews-detection.git
cd fake-reviews-detection

**Install Dependencies**: Ensure Python and required libraries (pandas, numpy, scikit-learn, nltk) are installed.
bash
Copy code
pip install -r requirements.txt

Run Preprocessing: Execute fakeReviewsDetection_01.py to preprocess the raw dataset:
bash
Copy code
python FakeReviewsDetection_01.py

Train and Test the Model: Use fakeReviewsDetection_02.py to train the model and evaluate its performance:
bash
Copy code
python FakeReviewsDetection_02.py

**Results**
The system effectively classifies reviews as genuine or fake using a Voting Classifier.
Preprocessing Insights:
Cleaned text significantly improves classification accuracy.
Features like sentiment scores and text length enhance model performance.
Model Performance:
Metrics such as accuracy, precision, recall, and F1-score are evaluated to ensure robustness.

**Future Enhancements**
Expand the dataset for better generalization across various product categories.
Explore deep learning models like LSTMs or transformers for enhanced text understanding.
Integrate the system into a web application for real-time review analysis.
