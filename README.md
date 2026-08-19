# Sentiment Analysis on University & Internship Reviews

## SafeX Solutions — Week 2 Task 2

A Natural Language Processing (NLP) project that analyzes university course and internship feedback using VADER sentiment analysis.

The system processes 300 sample reviews, classifies them as Positive, Neutral, or Negative, and extracts common keywords and themes to identify areas of satisfaction and improvement.

---

## 📌 Project Overview

Universities and organizations receive a large amount of open-text feedback from students and interns.

Manually reviewing every comment can be time-consuming. This project demonstrates an automated NLP pipeline that analyzes textual feedback and provides useful insights about sentiment and common themes.

The pipeline uses **VADER Sentiment Analysis** to classify feedback and uses keyword frequency and TF-IDF to identify important terms and themes.

---

## 🎯 Objectives

The main objectives of this project are:

- Analyze student and internship feedback automatically
- Clean and preprocess textual reviews
- Perform sentiment analysis using VADER
- Classify reviews into Positive, Neutral, and Negative categories
- Extract common keywords from feedback
- Identify important themes using TF-IDF
- Analyze sentiment across different feedback categories
- Visualize sentiment and keyword patterns
- Generate findings from the analyzed feedback

---

## 📊 Dataset

The dataset contains **300 sample reviews** related to university courses and internship experiences.

The dataset was created for educational and demonstration purposes.

### Dataset Columns

| Column | Description |
|---|---|
| `review_id` | Unique identifier for each review |
| `category` | Feedback category |
| `review` | Original feedback text |

### Categories

The reviews cover different feedback areas, including:

- Course
- Instructor
- Assignments
- Projects
- Learning Material
- Internship
- Mentorship
- Communication

---

## 🔄 Project Pipeline

```text
Raw Feedback
     ↓
Data Cleaning
     ↓
Text Preprocessing
     ↓
Tokenization
     ↓
Stopword Removal
     ↓
VADER Sentiment Analysis
     ↓
Positive / Neutral / Negative
     ↓
Keyword Extraction
     ↓
TF-IDF Theme Analysis
     ↓
Visualization
     ↓
Key Findings

```

---

## 🧹 Text Preprocessing

The review text was cleaned and prepared for analysis using several preprocessing techniques.

The preprocessing steps include:

Converting text to lowercase
Removing URLs
Removing punctuation and special characters
Removing extra whitespace
Tokenizing the text
Removing common English stopwords

A separate cleaned_review column was created while preserving the original review text.

## 🤖 Sentiment Analysis

The project uses VADER (Valence Aware Dictionary and sEntiment Reasoner) for sentiment analysis.

VADER generates a compound sentiment score ranging from -1 to +1.

The sentiment classification was performed using the following thresholds:

Compound Score	Sentiment
>= 0.05	Positive
-0.05 to 0.05	Neutral
<= -0.05	Negative

Each review receives:

A compound sentiment score
A sentiment label

The final analyzed dataset contains the sentiment information for all 300 reviews.

## 🔎 Keyword Analysis

Common keywords were extracted separately from positive and negative reviews.

This helps identify frequently discussed topics and provides additional information beyond the overall sentiment score.

Positive Keywords

The most frequently occurring words in positive reviews were analyzed to identify areas that students and interns responded positively to.

Negative Keywords

The most frequently occurring words in negative reviews were analyzed to identify potential problems and areas for improvement.

## 📚 TF-IDF Theme Analysis

TF-IDF (Term Frequency-Inverse Document Frequency) was used to identify important terms within the review dataset.

TF-IDF helps determine which words are particularly informative rather than simply counting how frequently a word appears.

The highest-scoring terms were used to identify common themes in the feedback.

## 📈 Visualizations

The project includes several visualizations to make the results easier to understand.

1. Number of Reviews by Category

Shows how the 300 reviews are distributed across different feedback categories.

2. Distribution of Review Length

Shows the distribution of reviews based on the number of words.

3. Overall Sentiment Distribution

Shows the number of Positive, Neutral, and Negative reviews.

4. Percentage of Reviews by Sentiment

Shows the percentage distribution of Positive, Neutral, and Negative reviews.

5. Sentiment Distribution by Category

Compares sentiment across different feedback categories.

6. Top Keywords in Positive Reviews

Shows the most frequently occurring keywords in positive reviews.

7. Top Keywords in Negative Reviews

Shows the most frequently occurring keywords in negative reviews.

8. Positive Review Themes

A word cloud showing frequently occurring terms in positive feedback.

9. Negative Review Themes

A word cloud showing frequently occurring terms in negative feedback.

10. TF-IDF Themes

Shows the most important terms identified using TF-IDF analysis.

## 📁 Project Files

The repository contains:

Google Colab Notebook — Complete sentiment analysis pipeline
Original Dataset — 300 sample reviews before analysis
Analyzed Dataset — Reviews with preprocessing and sentiment analysis results
Output Visualizations — Graphs and visualizations generated during the analysis
README.md — Project documentation

## 🛠️ Technologies Used
Python
Pandas
NumPy
NLTK
VADER Sentiment Analysis
Scikit-learn
Matplotlib
Seaborn
WordCloud
Google Colab

## 📌 Key Findings

The analysis of 300 reviews was used to identify:

Overall sentiment distribution
Sentiment differences across feedback categories
Common keywords in positive reviews
Common keywords in negative reviews
Frequently occurring positive and negative themes
Important terms identified using TF-IDF

The detailed findings and visual results are available in the Google Colab notebook and output visualizations included in this repository.

## 💡 Business / University Value

This pipeline can help universities and organizations analyze open-text feedback more efficiently.

It can be applied to:

Student course feedback
Instructor feedback
Assignment and project feedback
Internship feedback
Mentorship feedback
Communication feedback

For SafeX Solutions, a similar approach could be applied to internship feedback to identify common positive and negative areas and support improvements based on feedback.

## ⚠️ Dataset Note

The 300 reviews used in this project are sample reviews created for educational and demonstration purposes. They do not represent actual SafeX Solutions internship feedback or real university student responses.

## 👩‍💻 Author

Saliha Bibi
