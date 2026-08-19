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
- Generate actionable insights from feedback

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

🧹 Text Preprocessing

The review text was cleaned and prepared for analysis using several preprocessing techniques.

The preprocessing steps include:

Converting text to lowercase
Removing URLs
Removing punctuation and special characters
Removing extra whitespace
Tokenizing the text
Removing common English stopwords

A separate cleaned_review column was created while preserving the original review text.

🤖 Sentiment Analysis

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

The final analyzed dataset therefore contains the sentiment information for all 300 reviews.

🔎 Keyword Analysis

Common keywords were extracted separately from positive and negative reviews.

This helps identify frequently discussed topics and provides additional information beyond the overall sentiment score.

Positive Keywords

The most frequently occurring words in positive reviews were analyzed to identify areas that students and interns responded positively to.

Negative Keywords

The most frequently occurring words in negative reviews were analyzed to identify potential problems and areas for improvement.

📚 TF-IDF Theme Analysis

TF-IDF (Term Frequency-Inverse Document Frequency) was used to identify important terms within the review dataset.

TF-IDF helps determine which words are particularly informative rather than simply counting how frequently a word appears.

The highest-scoring terms were used to identify common themes in the feedback.

📈 Visualizations

The project includes several visualizations to make the results easier to understand.

1. Overall Sentiment Distribution

Shows the number of Positive, Neutral, and Negative reviews.

2. Sentiment Distribution by Category

Compares sentiment across different feedback categories.

3. Positive Keywords

Shows the most frequently occurring keywords in positive reviews.

4. Negative Keywords

Shows the most frequently occurring keywords in negative reviews.

5. Positive Review Themes

A word cloud showing frequently occurring terms in positive feedback.

6. TF-IDF Themes

Shows the most important terms identified using TF-IDF analysis.
