# Business Understanding

Apple would like to evaluate public sentiment about its products as compared to its competitor, Google. Social media is one area in which we can obtain feedback about our products. The sentiment expressed on social media can spread quickly and influence purchasing decisions for many consumers. Paying human raters to do this is expensive, especially when dealing with the sheer number of social media posts in existence. Here, we would like to build a model which can use Tweets to predict the nature of public sentiment about Apple products as compared to those of Google, use our insights to make improvements to our products so that we can positively influence perception of the company and by extension, increase market share and revenue, all in the most cost-effective manner possible.

# Data Understanding

Our dataset of over 9,000 Tweets is sourced from CrowdFlower via data.world. Humans rated Tweet sentiment as positive, negative, or neither (neutral).  There is a significant class imbalance in the the majority of Tweets are labeled as neutral.

# Data Preparation

I checked for and dealt with duplicate and null values, cleaned text of links, non-alphanumeric characters, etc.

# Exploratory Data Analysis

Our company and products ranked highest among products and brands mentioned.

<img width="3958" height="2978" alt="Product" src="https://github.com/user-attachments/assets/f9a73592-2a36-4477-854a-c8d2a034411f" />

Even so, Android was among the most frequently mentioned words within positive sentiment Tweets.

<img width="3984" height="2613" alt="words" src="https://github.com/user-attachments/assets/5584e0d4-b429-4b4a-8159-8b481e1e1741" />

# Modeling and Evaluation

The Random Forest Model correctly predicted Tweet sentiment 71% of the time, and performed best on the majority class.

<img width="2806" height="2943" alt="rf_confusion_matrix" src="https://github.com/user-attachments/assets/8b884a33-4838-4e90-a005-e4be35e448be" />

# Conclusions

The Random Forst model demonstrates the best performace with a weighted average precision score of .71, correctly predicting Tweet sentiment 71% of the time.

## Limitations

The limited amount of data is not ideal for modeling and additional data collection, particularly for the minority class, is warranted to improve the model.

Selection bias - Twitter data only may not be representative of overall sentiment since a small portion of the consumer market actually tweets. Data collection from other social media platforms and/or consumer surveys might be more informative.

## Recommendations

Deploy a Random Forest model to predict Tweet sentiment rather than paying raters to rate Tweets, giving the company the ability to evaluate public perception in a more cost-effective manner.

Collect more data, particularly from the minority class in order to improve the model.

Evaluate public excitement regarding Android versus our competitor product.

## Next Steps

Additional data collection

Monitoring and validating new data on a continual basis is essential, to ensure the model is refined when needed to maintain its efficacy.
