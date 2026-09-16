# Amazon Customers Sentiment Analysis

## 📌 Project Overview

This project analyzes Amazon customer reviews to understand customer sentiment, feedback patterns, and satisfaction levels.

The project uses customer review text from multiple Amazon product categories and classifies reviews into three sentiment categories:

- Positive
- Neutral
- Negative

The analysis also examines sentiment distribution across product categories and generates insights that can help identify areas for product and customer-experience improvement.

---

## 🎯 Project Objectives

The project focuses on the following objectives:

1. Analyze Amazon product reviews dataset.
2. Clean and preprocess review text data.
3. Perform sentiment classification into Positive, Neutral, and Negative.
4. Identify patterns in customer feedback and ratings.
5. Visualize sentiment distribution and trends.
6. Generate insights for product improvement and customer satisfaction.

---

## 📂 Dataset

The dataset contains Amazon customer reviews from the following product categories:

- 📚 Books
- 📖 Ebooks
- 🛒 Grocery
- 💎 Jewellery
- 💻 PC

The individual datasets were combined into a single DataFrame for analysis.

### Dataset Files

- `amazon_books_Data.csv`
- `amazon_ebook_Data.csv`
- `amazon_grocery_Data.csv`
- `amazon_jwellery_Data.csv`
- `amazon_pc_Data.csv`

---

## 🔄 Project Workflow

```text
Amazon Review Datasets
        ↓
Load and Combine Data
        ↓
Data Exploration
        ↓
Review Text Cleaning
        ↓
Stopword Removal
        ↓
Sentiment Classification
        ↓
VADER Sentiment Analysis
        ↓
TF-IDF Feature Extraction
        ↓
Logistic Regression
        ↓
Model Evaluation
        ↓
Sentiment Visualization
        ↓
Category-wise Analysis
        ↓
Customer Satisfaction Insights
```

## Data Preprocessing

The review text was cleaned before performing sentiment analysis.

The preprocessing steps include:

Converting text to lowercase
Removing HTML tags
Removing URLs
Removing numbers
Removing punctuation and special characters
Removing extra spaces
Removing English stopwords

A new column called clean_review was created containing the processed review text.

## Sentiment Analysis

The project classifies customer reviews into three sentiment categories:

Sentiment	Description
Positive	Reviews expressing favorable opinions
Neutral	Reviews expressing neither strongly positive nor negative opinions
Negative	Reviews expressing unfavorable opinions

VADER (Valence Aware Dictionary and sEntiment Reasoner) was used to determine sentiment from the review text.

The compound sentiment score was classified as:

Compound Score >= 0.05  → Positive
Compound Score <= -0.05 → Negative
Otherwise                → Neutral
Sentiment Distribution

The sentiment analysis produced the following distribution:

Sentiment	Reviews	Percentage
Positive	376	75.2%
Neutral	66	13.2%
Negative	58	11.6%
Total	500	100%

The majority of the analyzed reviews were classified as Positive.

## Machine Learning Model
TF-IDF

TF-IDF (Term Frequency-Inverse Document Frequency) was used to convert the cleaned review text into numerical features.

The model uses:

Maximum features: 10,000
Unigrams and bigrams
Sublinear TF scaling
Logistic Regression

Logistic Regression was used as the supervised machine learning classifier.

The dataset was divided into:

80% Training data
20% Testing data

Stratified splitting was used to preserve the distribution of sentiment classes.

Class balancing was applied to the training data because the sentiment classes were imbalanced.

## Model Evaluation

The Logistic Regression model achieved approximately:

75% Accuracy

The classification report was also used to evaluate:

Precision
Recall
F1-score

Accuracy should be interpreted together with these metrics because Positive reviews represent the majority of the dataset.

## Visualizations

The project includes visualizations to understand customer sentiment and feedback.

## Sentiment Distribution

A sentiment distribution chart shows the number of Positive, Neutral, and Negative reviews.

## Category-wise Sentiment

Sentiment percentages are compared across:

Books
Ebooks
Grocery
Jewellery
PC
Confusion Matrix

A confusion matrix is used to compare the actual and predicted sentiment classes from the Logistic Regression model.

Customer Feedback and Rating Patterns

The project analyzes customer feedback across different product categories.

Category-wise sentiment analysis helps identify differences in customer responses to different types of products.

Negative reviews can be examined to identify recurring problems and areas requiring improvement.

Neutral reviews can indicate opportunities to improve the customer experience.

Positive reviews can help identify product features and experiences that customers appreciate.

Product Improvement and Customer Satisfaction Insights

The sentiment analysis provides useful information for understanding customer satisfaction.

Positive reviews represent the largest portion of the analyzed customer feedback.
Negative reviews can be examined to identify recurring customer complaints.
Neutral reviews can reveal areas where customers may have mixed or moderate opinions.
Category-wise sentiment analysis helps identify differences in customer feedback between product categories.
Positive feedback can help identify product features and experiences that customers value.
Negative feedback can help businesses identify areas for product and service improvement.
Customer sentiment can be used to support decisions related to product quality and customer experience.
## Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
NLTK
Scikit-learn
VADER Sentiment Analysis
TF-IDF
Logistic Regression
Google Colab
Jupyter Notebook
Project Structure

Amazon-Customers-Sentiment-Analysis/
│
├── Amazon_Customers_Sentiment_Analysis.ipynb
├── README.md
│
└── dataset/
    ├── amazon_books_Data.csv
    ├── amazon_ebook_Data.csv
    ├── amazon_grocery_Data.csv
    ├── amazon_jwellery_Data.csv
    └── amazon_pc_Data.csv
    
## How to Run the Project
Step 1: Clone the Repository
git clone https://github.com/your-username/Amazon-Customers-Sentiment-Analysis.git
Step 2: Open the Notebook

Open:

Amazon_Customers_Sentiment_Analysis.ipynb

using Google Colab or Jupyter Notebook.

Step 3: Upload the Dataset

Upload the Amazon review dataset files when prompted.

Step 4: Run the Notebook

Run the notebook cells sequentially to perform:

Dataset loading
Data exploration
Text preprocessing
Sentiment analysis
TF-IDF feature extraction
Logistic Regression
Model evaluation
Sentiment visualization
Category-wise analysis
Customer satisfaction insights
Key Findings
The dataset contains 500 Amazon customer reviews.
Positive sentiment accounts for 75.2% of the reviews.
Neutral sentiment accounts for 13.2% of the reviews.
Negative sentiment accounts for 11.6% of the reviews.
The sentiment distribution indicates that positive feedback is the largest category in the analyzed dataset.
Category-wise analysis provides a way to identify areas with relatively higher negative or neutral feedback.
Customer reviews provide useful information for understanding satisfaction and identifying opportunities for improvement.

## Conclusion

This project demonstrates the use of Natural Language Processing and Machine Learning techniques to analyze Amazon customer reviews.

The analysis classifies customer feedback into Positive, Neutral, and Negative sentiments and examines sentiment patterns across different product categories.

The resulting insights can help understand customer satisfaction, identify negative feedback, and highlight opportunities for product and customer-experience improvement.


## Project Highlights
Amazon Customer Review Analysis
Multi-category Review Dataset
Text Cleaning and Preprocessing
VADER Sentiment Analysis
Positive / Neutral / Negative Classification
TF-IDF Feature Extraction
Logistic Regression
Sentiment Visualization
Category-wise Sentiment Analysis
Customer Feedback Analysis
Customer Satisfaction Insights
