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
