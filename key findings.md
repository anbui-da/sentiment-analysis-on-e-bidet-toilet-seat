## Data collection
- Scraped customer reviews on e-bidet toilet seat of different brands selling on Amazon. 
- The dataset contains total 3633 entries with 3627 non-null entries.

## Sentiment analysis
- Applied Textblob library to calculate the polarity scores and classified categorized sentiment.
  
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
- Not only that, keywords related to product design were also mentioned a lot such as "auto open-closed lid", "seat&cover soft close", "nozzle position".
- Brand name should be considered carefully since keywords related to it also occurred frequently such as "company stand behind product". 

## LDA model
### Findings:
The results from LDA model has identified 7 distinct topics from the dataset:

**Topic 0 - Product Installation and Customer Service**
- Keywords: product, unit, work, customer, install, easy, service, vovo, issue, new
- Interpretation: This topic seems to focus on the general product quality and customer service. It mentions the ease of installation ("easy", "install"), working state of the product ("work", "issue"), and aspects of customer service ("customer", "service"). The mention of "vovo" could indicate a specific brand or product model.

**Topic 1 - Installation Process and Components**
- Keywords: seat, water, valve, installation, hose, install, fit, tank, line, instruction
- Interpretation: This topic is likely discussing the mechanical and technical details involved in installing the bidet seat. It includes parts like "valve", "hose", "tank", "line", and references to the "installation" process and "instruction".

**Topic 2 - Features and Usage**
- Keywords: seat, water, remote, button, feature, light, setting, work, use, get
- Interpretation: The emphasis here is on the features and functionality of the bidet seat ("remote", "button", "feature", "light", "setting") and user interaction with the product ("use", "get").

**Topic 3 - Specific Features and User Feedback**
- Keywords: s7a, heated_seat_warm_water, drawing, lcd, write, robot, coolest, horrible, yikes, heart
- Interpretation: This topic appears to cover specific features or models (e.g., "s7a", "heated_seat_warm_water"), with some emotional responses to the product ("coolest", "horrible", "yikes") and possibly design aspects ("drawing", "lcd").

**Topic 4 - Comfort and Hygiene**
- Keywords: seat, water, use, get, warm, easy, love, clean, bathroom, work
- Interpretation: Focusing on the comfort and hygiene aspects ("warm", "clean"), positive user experiences ("love", "easy"), and general use within the bathroom environment.

**Topic 5 - Longevity and Maintenance**
- Keywords: year, working, new, month, stopped, replacement, product, issue, problem, started
- Interpretation: Discussing product longevity and issues encountered over time ("year", "month", "stopped", "problem"), maintenance needs ("replacement", "working"), and potentially the lifecycle of the product ("new", "started").

**Topic 6 - Product Quality and Purchasing Experience**
- Keywords: seat, unit, measurement, team, cover, 1000, crack, product, amazon, plastic
- Interpretation: This topic may relate to customer experiences with product quality ("crack", "plastic"), purchasing or customer support teams ("team"), and potentially the shopping experience ("amazon").

The LDA analysis reveals that while there are many positive aspects to the product, there are also specific areas that the company need attention such as customer service, installation guidance, product features, and addressing quality concerns.
