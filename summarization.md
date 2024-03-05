## About the dataset
- Scraped customer reviews on e-bidet toilet seat of different brands selling on Amazon. 
- The dataset contains total 3633 entries with 3627 non-null entries.
- 
## Sentiment analysis

**1. Distribution of Polarity Scores**
![image](https://github.com/anbui-da/sentiment-analysis-on-e-bidet-toilet-seat/assets/58675665/988eca23-03f1-40ac-960b-95022840e828)

- Central tendency:  The distribution of polarity scores seems to be centered around a value slightly above 0, indicating a general trend towards positive sentiment in the dataset.
- Skewness: There is a visible skew in the data towards the positive side (right skew), which suggests that there are more positive reviews than negative ones.
- Sentiment spread: The spread of the polarity scores from negative to positive indicates a range of sentiments in the reviews. However, the concentration of scores towards the middle suggests that extreme sentiments (both highly positive and highly negative) are less common.
- For business implications, the histogram suggests that the majority of customers are generally satisfied with their experience, but there is still a significant proportion of neutral and some negative experiences that could be explored further to understand areas for product improvement.
  
**2. Proportion of Sentiment**
![image](https://github.com/anbui-da/sentiment-analysis-on-e-bidet-toilet-seat/assets/58675665/f766ba97-63c0-48e5-8fc3-820b48b8982a)
- Positive sentiment accounted for 80% of the customer reviews, meanwhile negative and neutral experiences accounted for 12.3% and 6.9% respectively. In overall, customers seem to have positive experience while using electric bidets so far. But the negative sentiments represent an opportunity for the company to identify common issues or pain points that could be addressed to improve the overall customer experience.

**3. Word cloud**
- A word cloud frequently recurring word in large size and less occuring word in a small size.
  
![image](https://github.com/anbui-da/sentiment-analysis-on-e-bidet-toilet-seat/assets/58675665/715cb18b-d757-4cfe-8dc2-15bf073d58e5)

- It can be seen that most occuring keywords such as **seat, water, remote, use, easy, install** refers to the user experience during their installation and usage. However, these keywords might involve any positive, negative or neutral experience, which requires the business to deep dive into customer reviews for better understanding.

  
**4. Extracting most common n-grams**
- To analyze the text data to find common 4-grams, which can be indicative of recurring themes or phrases in the text, and to visualize these common elements to aid in data interpretation and insights.

![image](https://github.com/anbui-da/sentiment-analysis-on-e-bidet-toilet-seat/assets/58675665/49d54737-4ca3-42a8-8341-80d5a7538f17)

- Product features like heated seat and warm water, or user experience during the installation phase are the most frequent patterns.

## LDA model

