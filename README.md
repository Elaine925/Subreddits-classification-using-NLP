# Classifying r/VisitingHawaii and r/Europetravel Subreddits Using NLP

## Problem Statement

Reddit serves as a platform for various communities to converge around specific topics or interests. Among these communities are [r/VisitingHawaii](https://www.reddit.com/r/VisitingHawaii/) and [r/Europetravel](https://www.reddit.com/r/Europetravel/), which focus on sharing insights, tips, and experiences related to travel destinations in Hawaii and Europe. Understanding the distinctive traits and content preferences of these communities holds significance for content creators, marketers, and stakeholders within the travel industry.



## Data Dictionary


|Feature|Type|Description|
|---|---|---|
|**subreddit**|*object*|Subreddit source|
|**lemmatized_text**|*object*|Lemmatized text combined from subreddit posts title and self text|



## Executive Summary


### Project objective

By examining various text-based metrics and features in subreddits r/VisitHawaii and r/Europetravel, the goal is to differentiate between the two communities based on the contents of the posts.

### Methodology

The methodology involves several steps:
1. Data Cleaning:
    - Filtering non-text-based titles or self-text to focus on relevant textual content.
    - Removing URLs, HTML encoded characters, and emojis to ensure clean text data.
    
2. Exploratory Data Analysis (EDA):
    - Text normalization techniques are applied, including tokenization to retain only English letters.
    - Lemmatization is utilized for reducing words to their base forms while preserving word meaning.
    - Sentiment analysis is conducted to understand the emotional tone of the posts.
    - Frequency analysis is performed to identify commonly used words in each subreddit.
    
3. Train-Test Split:
    - The dataset is divided into training and testing sets to assess model performance accurately.
    
4. Vectorization Methods:
    - Both Count Vectorizer and TF-IDF Vectorizer are employed to convert the textual data into numerical vectors, capturing the frequency or importance of words in the documents.
 
5. Model Selection:
    - Several classification algorithms are utilized for model training, including Logistic Regression, Multinomial Naive Bayes, Random Forest Classification, and Support Vector Classifier (SVC).
    
6. Model Evaluation:
    - Each classification model is trained using the training data and evaluated using the testing data.
    - Model performance metrics such as training score, testing score, and accuracy is calculated to assess the effectiveness of each model.



### Key findings
All models performed admirably in distinguishing between 2 subreddits, with logistic regression and SVC with TF-IDF Vectorizer emerging as the top performers based on their high testing scores.




### Conclusion and Recommendations

#### Conclusion
Stakeholders in the travel industry, such as travel agencies, tour operators, and destination marketing organizations, can leverage insights from subreddit classification to tailor their content creation and marketing strategies. By understanding the preferences, interests, and concerns of users in r/VisitingHawaii and r/Europetravel, stakeholders can develop targeted campaigns and promotional materials that resonate with the target audience.By monitoring discussions, sentiment, and trends in both subreddits, stakeholders can gain valuable intelligence about consumer preferences, competitor strategies, and market dynamics. 


#### Recommendations
- Continuously refining and optimizing the classification models based on feedback and new data can improve accuracy and effectiveness.
- Integrating the subreddit classification models with real-time data sources, such as social media feeds, and travel forums etc, can provide up-to-date insights and actionable intelligence.
