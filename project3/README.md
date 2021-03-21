# Problem Statement
In 2020, Covid-19 has greatly impacted many countries which resulted in mulitple countries going into lockdown where physical stores are force to shut their doors and many businesses moved online. As such, ecommerce sales skyrocketed and account for [101% of all growth in retail in US](https://www.digitalcommerce360.com/article/us-ecommerce-sales/)<br><br>
As many small businesses does not have the necessary resources nor expertise to setup and manage their own website, online platform such as Etsy and Shopify are able to provide an effective platform to help these businesses quickly and easily transit into ecommerce. Despite both website seemingly provide the same service, it is in fact 2 different kindly of ecommerce platform. Etsy is an online market place where most transaction will occur there, while Shopify is a webstore platform that help to build a website for an online business.
<br><br>
The objective of this project is to create a classification model to help effectively categorize the subreddit post for Etsy and Shopify and discover what are the main differences to help small businesses select the most effective platform for themselves. It would also give an understand the main focus of our client so as to effectively channel our market strategies to increase Etsy market share.

# Executive Summary

## Webscrapping notebook
In this notebook, we will scrapping from Etsy subreddit and Shopify subreddit

## Modeling notebook
In this notebook, we will be creating a few classification models and selecting one which give the best prediction to evalute on
### Content
- [Model Selection](#Model-Selection)
 - [CountVectorizer with Logistic Regression](#CountVectorizer-with-Logistic-Regression)
 - [TF-IDF Vectorizer with Logistic Regression](#TF-IDF-Vectorizer-with-Logistic-Regression)
 - [Count Vectorizer with Multinomial Naive Bayes](#Count-Vectorizer-with-Multinomial-Naive-Bayes)
 - [TF-IDF Vectorizer with Multinomial Naive Bayes](#TF-IDF-Vectorizer-with-Multinomial-Naive-Bayes)
- [Model comparision](#Model-comparision)
- [Etsy Impactful Word(s)](#Etsy-Impactful-Word(s))
- [Shopify Impactful Word(s)](#Shopify-Impactful-Word(s))
- [Evaluation of model](#Evaluation-of-model)
 - [Model 'Etsy' Prediction](#Model-'Etsy'-Prediction)
 - [Model 'Shopify' Predicition](#Model-'Shopify'-Predicition)
- [Conclusion and Recommendation](#Conclusion-and-Recommendation)

# Conclusion and Recommendation
From our model, it shows that the post for Etsy are from both the seller and buyer while post for Shopify are mainly by the seller. Additionally, as Etsy is a creative marketplace which focus on handmade, vintage and craft supplies, there were indication of this focus by some of the key words having relation with art and craft.

There are a few recommendation that we proposed to distinguish Etsy from our competitor and certain area of focus for us to effectively channel our marketing strategies.

First recommendation is to focus on promotion of our client product. From the misclassified post which were under Etsy but predicted to be Shopify, it can be seen that most of these post are focus on promoting their own product in different platform. However, as Etsy has our own platform where we have a huge built in audience, it would be an effective platform to enable publicity and attracting traffic flow to our client stores.

Another area of focus could be to provide an effective channel for buyer to source for seller which can customize products that they are looking for. Given that Etsy effectiveness in supporting and promoting extraordinary items, from unique handcrafted piece to vintage treasure. It would be helpfully to allow seller to have a listing of crafting service which would give buyers the opportunity to find and get these personalize items.

By targeting these area of needs, stakeholder will be able to improve the user experience of both the seller and buyer and thus increasing the number of users for Etsy.
