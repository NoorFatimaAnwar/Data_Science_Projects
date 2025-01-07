**Mental Health Status Predictor using Decision Tree**
This project aims to predict an individual's mental health status based on responses collected through a Google Form survey. It uses a Decision Tree Classifier to classify the mental health status as Moderate Concern, Stable, or High Concern.

**Project Overview**
The project involves:
**Dataset Collection**: Raw data collected through a Google Form survey containing responses about sleep, exercise, stress, mood, social interaction, and academic stress.
**Data Preprocessing**: Normalizing and cleaning the raw dataset to prepare it for machine learning.
**Model Development**: Using a Decision Tree algorithm to predict mental health status based on the preprocessed data.
Files in the Repository

**1. Raw Dataset** (raw_dataset.csv)
Contains the original responses collected through a Google Form survey.
Columns include:
Timestamp: Date and time of survey submission.
Hours of Sleep: Sleep duration per night.
Sleep Quality: Self-reported sleep quality.
Exercise Frequency: Weekly exercise habits.
Stress Level: Self-reported stress on a scale of 1–10.
Academic Stress: Frequency of academic stress.
Social Interaction: Frequency of interactions with friends/family.
Mood: Self-reported mood on a scale of 1–10.
Happiness Level: Overall happiness rating on a scale of 1–10.
Anxiety Symptoms: Frequency of anxiety symptoms.
Mental Health Status: Final self-reported mental health status.

**2. Preprocessed Dataset** (preprocessed_dataset.csv)
The cleaned and normalized version of the raw dataset.
Data has been scaled and converted into numerical values for better compatibility with machine learning models.

**3. Code (predictor.py)**
Python script containing the implementation of:
Data loading and preprocessing steps.
Decision Tree Classifier for prediction.
Evaluation metrics to assess model performance.

**How to Use**
Clone the Repository:

bash
Copy code
git clone https://github.com/yourusername/mental-health-predictor.git
cd mental-health-predictor

**Install Dependencies**: Make sure you have Python installed along with required libraries like pandas, scikit-learn, and numpy.

**Install dependencies using:**

bash
Copy code
pip install -r requirements.txt
**Run the Project:** 
Execute the predictor.py file to preprocess the data and build the Decision Tree model.
bash
Copy code
python predictor.py

**Results**
The model classifies mental health status into three categories:
Moderate Concern
Stable
High Concern
Key insights:
Features like sleep hours, stress levels, and social interaction heavily influence predictions.
Normalization improves the performance of the Decision Tree model.

**Future Improvements**
Incorporate more features for better accuracy.
Explore other classification algorithms to compare performance.
Enhance the dataset with more diverse responses.

Feel free to contribute by suggesting improvements or submitting a pull request! 😊
