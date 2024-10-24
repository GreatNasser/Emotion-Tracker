# Emotion Tracker with AI Sentiment Analysis (Text-based)

## Introduction
The **Emotion Tracker** tool is a Python-based solution that uses artificial intelligence (AI) to analyze the emotions embedded in text entries. It helps users track and understand their emotional state over time based on daily journal entries. The app processes the text, providing sentiment analysis that categorizes the text into positive, negative, or neutral emotions, offering deeper insights into mood fluctuations.

---

## Key Features
- **Text-based Sentiment Analysis**: The app analyzes the provided text to determine whether the emotions expressed are positive, negative, or neutral.
- **Emotion Tracking**: Tracks mood changes based on journal entries provided in plain text.
- **Statistical Reporting**: Generates statistical reports that show emotional trends over time.
- **Integration with Other Mental Health Tools**: Provides insights that can be integrated with tools like **Headspace** and **Calm** to support emotional well-being.

---

## Installation Guide

To set up the tool, follow these steps:

1. **Install Python** (version 3.7 or higher).
   Download and install Python from [python.org](https://www.python.org/downloads/).

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/emotion-tracker.git
   cd emotion-tracker
pip install nltk textblob matplotlib
python analyze.py journal.txt
{
  "date": "2024-10-25",
  "entry": "I had a great day today, everything went well.",
  "sentiment": "Positive",
  "sentiment_score": 0.8
}
from textblob import TextBlob

def analyze_sentiment(text):
    blob = TextBlob(text)
    return blob.sentiment.polarity

text = "I had a wonderful day!"
sentiment_score = analyze_sentiment(text)
if sentiment_score > 0:
    print("Positive")
elif sentiment_score < 0:
    print("Negative")
else:
    print("Neutral")
