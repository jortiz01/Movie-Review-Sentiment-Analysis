# Movie-Review-Sentiment-Analysis

![sent_analy_intro](https://user-images.githubusercontent.com/66872947/200339949-92c6de57-25a1-40e4-934b-541271812d03.png)



First I load the training and test data for sentiment analysis. The training data has 40,000 rows and the test data has 5000.



![sent_analy_data](https://user-images.githubusercontent.com/66872947/200339990-60375054-6fa4-4435-94ec-072a445fa3e5.png)


Then I vectorize each word by unigrams utilizing SKLearns' CountVectorizor.


![sent_analy_uni](https://user-images.githubusercontent.com/66872947/200340012-f2e10495-fc4c-4786-9fcf-857178298e16.png)


Utilizing SKLearn's TfIdfTransformer, I utilized the texts' TF-IDF values for comparison to raw count values.


![sent_analy_uni_MNB](https://user-images.githubusercontent.com/66872947/200340030-7e8d6e43-1f8c-4713-a8a8-c21bc6f7c1d7.png)


Utilizing unigram TF-IDF values, Multinomial Naive Bayes predicted the correct sentiment label on the test data with 84.99% accuracy.


![sent_analy_bigram_tfidf_mnb](https://user-images.githubusercontent.com/66872947/200342347-74fbc772-c44a-45e8-9843-c0dc6da97ae3.png)


Utilizing bigram TF-IDF values, Multinomial Naive Bayes predicted the correct sentiment label on the test data with 87.4% accuracy.
