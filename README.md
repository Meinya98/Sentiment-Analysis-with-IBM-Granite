# Sentiment Analysis with IBM Granite
Application's reviews sentiment analysis with IBM Granite 3.3 Instruct model. A classification problem 
### Project Overview
- Background: Reviews are used to improve anything, in this case is a mobile application
- Problems:
  - Reviews were not used effectively because it is not classified, only based on "star" rating
  - Some users are not giving reviews correctly (5 star but bad review)
- Approach: Use AI (IBM Granite) for reviews classification in sentiment analysis
- Purpose: To classify reviews for generating insights and actionable points for further refining the application
### 1. Dataset
Dataset used is from [Kaggle](https://www.kaggle.com/datasets/ahmadseloabadi/tix-id-app-reviews-from-google-play-store/data)
### 2. Insights & Findings
1. The negative reviews are dominating, mostly with 1 - 2 star rating (as expected). But, some has 5 star rating, indicating a mislabel or sarcastic/fake reviews
2. Given the model was not consistent in the output, the prompt has to be evaluated. The reviews has to be translated to english first. Examples must be given explicitly to prevent mislabels and unknown labels
- This was confirmed by violinplot that some 4-5 scores are labeled "N/A" or "Mixed"
3. Given the multiple "RunTime Error" occured, the underlying problem has to be investigated (from the server?) or try to run in batch
### 3. Recommendations
1. Dig deeper into the reason why the reviews were flagged as "negative" to further evaluate the application, and also the “mixed” and “N/A” reviews to see why the mistakes happen from the model
2. Try reevaluating after refining the prompt to see the difference
3. If multiple errors are still occurring, contact the developer or support
### 4. AI Support Explanation
AI model used: [IBM Granite 3.3 Instruct](https://replicate.com/ibm-granite/granite-3.3-8b-instruct) \
This model was used for classify the reviews as "positive", "negative", or "mixed"
