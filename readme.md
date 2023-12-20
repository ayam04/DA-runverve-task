# **Data Analysis & Predictive Modeling of Customer's Data**

## Table of Contents
- [Web Scraping for Data Analysis](#web-scraping-for-data-analysis)
  - [Web Scraping](#web-scraping)
  - [Data Preprocessing](#data-preprocessing)
  - [Sentiment Analysis](#sentiment-analysis)
  - [Data Visualization](#data-visualization)
- [Predictive Modeling on Customer's Data](#predictive-modeling-on-customers-data)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Mutual Information Graphs](#mutual-information-graphs)
  - [Test and Train Model](#test-and-train-model)
  - [Validate Model](#validate-model)
- [Conclusion](#conclusion)
- [Libraries Utilized](#libraries-utilized)

## **Web Scraping for Data Analysis**

### **Web Scraping**
We utilized web scraping techniques to gather customer reviews and insights about Air India from [Airline Quality](https://www.airlinequality.com/airline-reviews/air-india/). Extracted data includes customer comments, ratings, and relevant information, compiled into the "Reviews Dataset" for further analysis like predicting customer buying behaviors or understanding sentiments towards Air India's services.

### **Data Preprocessing**
Data preprocessing involves cleaning, transforming, and integrating data to enhance its quality and suitability for analysis.

#### **Data Cleaning**
- Removed sentences before '|' in the dataframe.
- Eliminated special characters from the dataframe.

#### **Tokenization**
- Text was tokenized to meaningful pieces.
- Tokens were converted to tuples using POS Tagging and grouped into words through lemmatization.

## **Sentiment Analysis**
Analyzing digital text to determine emotional tones (positive, negative, neutral).

### **VADER**
- VADER (Valence Aware Dictionary for Sentiment Reasoning) provided sentiment scores based on words used.
- It's a rule-based sentiment analyzer that categorizes terms as positive, negative, or neutral.

## **Data Visualization**
Using graphics to represent complex data relationships.

### **via. Matplotlib**
Matplotlib, a comprehensive library, creates static, animated, and interactive visualizations.

![Matplotlib Visualization](https://github.com/nilayhangarge/IBM-CSRBOX-Internship-Project/assets/88373687/03e1d670-39bb-4c64-aedd-ccdeb2c39755.png)

### **via. WordCloud**
Wordcloud visually represents word frequency in a text, where size indicates frequency.

![WordCloud Visualization](https://github.com/nilayhangarge/IBM-CSRBOX-Internship-Project/assets/88373687/d3770498-5ab5-4707-a44d-5482123565ec.png)

# **Predictive Modeling on Customer's Data**

## **Exploratory Data Analysis**
- Understanding the data, gaining insights, and identifying patterns.
- Used Chardet library for UTF-8 encoded code, applied to CSV, and checked for null values.

## **Mutual Information Graphs**
- Visualizes feature relevance to the target variable, aiding feature selection.
- scikit-learn (sklearn) calculates MI_score correlation between attributes.

![MI Graphs](https://github.com/adityabasanti/IBM-CSRBOX-Internship-Project/assets/102895768/9206150b-b50a-4197-9957-0d917629a928.png)

## **Test and Train Model**
- Divided datasets into training and test sets for building and evaluating machine learning models.
- Used Min-Max Scaling for consistent scaling across features.

### **via. Random Forest Classifier & XGB Classifier**
Ensemble learning methods providing accurate and robust models.

## **Validate Model**
Assessed model performance on unseen data.

# **Conclusion**
**The Random Forest classifier with the top 6 features exhibited slightly higher accuracy than XGBoost. It effectively predicts customer satisfaction or target variables.**

## **Libraries Utilized**
- BeautifulSoup (bs4)
- Chardet
- Matplotlib
- Natural Language Toolkit (nltk)
- Numpy (np)
- Pandas (pd)
- Requests (re)
- Seaborn (sns)
- Scikit-learn (sklearn)
- VaderSentiment (SentimentIntensityAnalyzer)
- Warnings
- WordCloud
