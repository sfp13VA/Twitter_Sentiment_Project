# Business Understanding
Apple would like to evaluate public sentiment about its products as compared to its competitor, Google. Social media is one area in which we can obtain feedback about our products. The sentiment expressed on social media can spread quickly and influence purchasing decisions for many consumers. Paying human raters to do this is expensive, especially when dealing with the sheer number of social media posts in existence. Here, we would like to build a model which can use Tweets to predict the nature of public sentiment about Apple products as compared to those of Google, use our insights to make improvements to our products so that we can positively influence perception of the company and by extension, increase market share and revenue, all in the most cost-effective manner possible.
# Data Understanding

## Data Understanding
Our dataset of over 9,000 Tweets is sourced from CrowdFlower via data.world. Humans rated Tweet sentiment as positive, negative, or neither (neutral).

# Exploratory Data Analysis

The data shows our company and producs generate a lot of chatter on Twitter.
<img width="3028" height="2072" alt="Product" src="https://github.com/user-attachments/assets/0686bb50-1617-4625-8577-1b6c231bca74" />

Even so, Google's Android ranke din the most frequent words contained in Tweets with positive sentiment, while our products did not rank in the top 15 words at all.
<img width="3054" height="2160" alt="words" src="https://github.com/user-attachments/assets/84e5b711-fe36-4221-80d0-e26622c26884" />


# Modeling and Evaluation
We found that a Random Forest binary classifier produced the best modeling result.
<img width="2304" height="2043" alt="rf_confusion_matrix" src="https://github.com/user-attachments/assets/a6517f72-9493-4b1a-8648-8ccea5b58a59" />


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

