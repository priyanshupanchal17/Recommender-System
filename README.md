Product Sales Recommendation & Sentiment Analysis

📌 Project Overview

This project aims to build a hybrid recommendation system combining content-based filtering and collaborative filtering to provide personalized product recommendations. Additionally, it performs sentiment analysis on customer reviews using BERT and visualizes product ratings interactively.

🚀 Features

🔹 Hybrid Recommendation System

Content-Based Filtering: Uses product descriptions, categories, and user preferences.

Collaborative Filtering: Leverages user-item interaction data to suggest products.

🔹 Sentiment Analysis on Reviews

Utilizes BERT-based NLP models to classify customer sentiments.

Maps ratings to sentiment categories (e.g., 1⭐ → "Very Negative", 5⭐ → "Very Positive").

🔹 Interactive Data Visualization

Scatter plot visualization of products based on sentiment.

Identification of top-rated products.

📂 Dataset Structure

Column Name

Description

product_id

Unique ID for each product

product_name

Name of the product

category

Product category

discounted_price

Discounted price of the product

actual_price

Original price before discount

discount_percentage

Discount percentage

rating

Average rating (float)

rating_count

Number of ratings received

review_content

User-generated review text

user_id

Unique ID for each user

review_id

Unique ID for each review

sentiment

Predicted sentiment from BERT

expected_sentiment

Sentiment mapped from ratings

🛠️ Tech Stack

Programming Language: Python 🐍

Libraries:

pandas, numpy → Data manipulation

scikit-learn → Machine learning models

transformers (BERT) → Sentiment analysis

matplotlib, seaborn, plotly → Data visualization

📊 Implementation Steps

1️⃣ Data Preprocessing

Convert ratings to numeric and remove null values.

Apply math.floor() to round ratings down.

Map star ratings to sentiment labels.

2️⃣ Sentiment Analysis

Use a pre-trained BERT model for classifying reviews.

Store results in the sentiment column.

3️⃣ Hybrid Recommendation System

Implement Content-Based Filtering using TF-IDF.

Apply Collaborative Filtering using the Surprise library.

Combine both using a weighted approach (alpha parameter).

4️⃣ Interactive Visualization

Create a scatter plot of products grouped by sentiment.

Highlight highly rated products.

🎯 How to Run the Project

Clone the repository:

git clone https://github.com/your-repo-url
cd your-repo-folder

Install dependencies:

pip install -r requirements.txt

Run the analysis script:

python main.py

📌 Future Enhancements

Improve sentiment accuracy with fine-tuned BERT.

Incorporate real-time product trends in recommendations.

Implement a multi-objective optimization to balance profitability and diversity.

👨‍💻 Developed by: [Your Name]📅 Project Date: [Month, Year]
