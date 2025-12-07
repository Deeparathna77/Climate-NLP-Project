# Climate Change Comments Analysis using NLP

This project focuses on analyzing public comments related to climate change, mainly taken from NASA’s climate discussion data. The goal of the project is to understand how people feel about climate-related topics by using Natural Language Processing (NLP), sentiment analysis, and topic modeling.

The project includes data cleaning, text preprocessing, visualizations, sentiment classification using machine learning, and topic extraction using LDA. All analysis is done in Python using Jupyter Notebook.

---

## Project Overview

The dataset contains around 522 comments. These comments include people’s opinions, questions, statements, and reactions to climate-related information.  
To work with the data effectively, it first goes through cleaning steps such as removing punctuation, converting to lowercase, removing stopwords, and lemmatization.

After cleaning the text, the comments are analyzed to understand what people commonly talk about and how they feel about climate change.

---

## What This Project Covers

1. **Data Preprocessing**
   - Cleaning the text by removing special characters
   - Tokenizing sentences and words
   - Removing stopwords
   - Lemmatizing words

2. **Exploratory Data Analysis**
   - Basic dataset inspection
   - Word frequency checks
   - WordCloud to see the most used words
   - Visualizations of sentiment distribution

3. **Sentiment Analysis**
   - Used TF-IDF for converting text into numerical features
   - Logistic Regression model for classification
   - The model predicts whether a comment is Positive, Neutral, or Negative
   - Final accuracy achieved was around 65%

4. **Topic Modeling (LDA)**
   - Helps identify the main themes people are discussing
   - Extracted 5 major topics
   - Topics include global warming, CO₂ emissions, climate data, environmental concerns, and temperature patterns

5. **Model Saving**
   - The sentiment model and TF-IDF vectorizer are saved using joblib
   - These can be reused later without retraining

---

## Folder Structure

```
Climate-NLP-Project/
│
├── data/
│   └── NASAClimateComments.csv
│
├── models/
│   ├── logistic_sentiment_model.joblib
│   └── tfidf_vectorizer.joblib
│
├── outputs/
│   ├── wordcloud.png
│   ├── sentiment_distribution.png
│   └── confusion_matrix.png
│
├── Climate_NLP_Project.ipynb
├── Climate_NLP_Project.html
└── README.md
```

---

## Tools and Libraries Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn
- Gensim
- WordCloud
- Jupyter Notebook

---

## Summary of Results

The sentiment analysis model performed reasonably well given the small dataset. Neutral comments were detected with good accuracy, while negative comments were harder because there were fewer of them in the dataset.

The LDA topic modeling gave a clear idea of the main areas being discussed, such as NASA climate data, global warming, carbon dioxide levels, and environmental changes.

---

## How to Run the Project

1. Download or clone the project:
```
git clone https://github.com/YourUserName/Climate-NLP-Project.git
```

2. Install the required libraries:
```
pip install -r requirements.txt
```

3. Open the notebook:
```
jupyter notebook Climate_NLP_Project.ipynb
```

---

## Author

Deeparathna  
BSc Computer Science  
IG College, Trichy

---

## Notes

This project was created as part of an academic learning exercise.  
The goal is to explore NLP methods and understand how text data can be used to study climate-related discussions.
