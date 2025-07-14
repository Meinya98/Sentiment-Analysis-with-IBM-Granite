# Sentiment Analysis with IBM Granite
Application's reviews sentiment analysis with IBM Granite 3.3 Instruct model. A classification problem 

### 1. Dataset
Dataset used is from [Kaggle](https://www.kaggle.com/datasets/ahmadseloabadi/tix-id-app-reviews-from-google-play-store/data)
### 2. Insights & Findings
1. The negative reviews are dominating, dig deeper into the "why" aspect for the review flagged with "negative"
2. Given the model was not consistent in the output, the prompt has to be evaluated. The reviews has to be translated to english first. Examples must be given explicitly to prevent mislabels
- This was confirmed by violinplot that some 4-5 scores are labeled "N/A" or "Mixed"
3. Given the multiple "RunTime Error" occured, the underlying problem has to be investigated (from the server?) or try to run in batch
### 3. Recommendations
1. Dig deeper into the reason why the reviews were flagged as "negative" to further evaluate the application
2. Try reevaluate after refining the prompt to see the difference
### 4. AI Support Explanation
AI model used: [IBM Granite 3.3 Instruct](https://replicate.com/ibm-granite/granite-3.3-8b-instruct) \
This model was used for classify the reviews as "positive", "negative", or "mixed"
