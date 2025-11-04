# Business Understanding
Apple would like to evaluate public sentiment about its products as compared to its competitor, Google. Social media is one area in which we can obtain feedback about our products. The sentiment expressed on social media can spread quickly and influence purchasing decisions for many consumers. Paying human raters to do this is expensive, especially when dealing with the sheer number of social media posts in existence. Here, we would like to build a model which can use Tweets to predict the nature of public sentiment about Apple products as compared to those of Google, use our insights to make improvements to our products so that we can positively influence perception of the company and by extension, increase market share and revenue, all in the most cost-effective manner possible.
# Data Understanding

## Data Understanding
Our dataset of over 9,000 Tweets is sourced from CrowdFlower via data.world. Humans rated Tweet sentiment as positive, negative, or neither (neutral).

# Exploratory Data Analysis
/Users/buzzardsroostimac/Documents/Flatiron/Phase_4/twitter_sentiment_project/Product.png 
/Users/buzzardsroostimac/Documents/Flatiron/Phase_4/twitter_sentiment_project/words.png 

# Modeling and Evaluation
We found that a Random Forest binary classifier produced the best modeling result.
/Users/buzzardsroostimac/Documents/Flatiron/Phase_4/twitter_sentiment_project/rf_confusion_matrix.png

# Conclusion
The Random Forst model demonstrates the best performace with a weighted average precision score of .71, correctly predicting Tweet sentiment 71% of the time.
Deploy a Random Forest model to predict Tweet sentiment rather than paying raters to rate Tweets, giving the company the ability to evaluate public perception in a more cost-effective manner.

Collect more data, particularly from the minority class in order to improve the model.

Evaluate public excitement regarding Android versus our competitor product.
## Limitations
The limited amount of data is not ideal for modeling and additional data collection, particularly for the minority class, is warranted to improve the model.

Selection bias - Twitter data only may not be representative of overall sentiment since a small portion of the consumer market actually tweets. Data collection from other social media platforms and/or consumer surveys might be more informative.
## Recommendations

## Next Steps
Additional data collection

Monitoring and validating new data on a continual basis is essential, to ensure the model is refined when needed to maintain its efficacy.

