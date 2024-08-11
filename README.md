# Harry Potter Book Recommendations
 Can I give you good book recommendations based on your favourite Harry Potter book?
 
 ## Overview
 In this project, I aim to create book recommendations based off the opinion a person has on a Harry Potter Book. This involves collecting the reviews from GoodReads by Webscraping, carrying out Sentiment Analysis on these Reviews, carrying out Topic Modelling on the Reviews, combining these to identify suitable books for you!
 
 
### Table Of Contents:
* [WebScraping](#1)
* [Sentiment Analysis](#2)
* [Topic Modelling](#3)
* [Book Recommendations](#4)

> Note: I have included my presentation slides (from 05/07/24) as a pdf in this repository. The results shown in here may be different to the other files in this repository, since different results are produced when the cells are rerun.

## **1** WebScraping <a class="anchor" id="1"></a>
To WebScrape the reviews from GoodReads, I used **BeautifulSoup** and **Selenium**. 

The WebScraping files are not included in this repository beacause I had to alter my data collection method slightly due to some issues I encountered. 

## **2** Sentiment Analysis <a class="anchor" id="2"></a>
The plan was to use sentiment analysis to identify a users favourite book, however, due to the issues I had with the data collection, I collected fewer reviews than expected. So instead I decided to carry out the analysis to find out how much the user likes a particular book. 

I made use of **VADER**, which is a pre-trained sentiment analysis model, specialised for analysing social media texts. It provided me with _polarity scores_ which I used to gauge the user's sentiment.

_Read more about VADER in this [article](https://medium.com/@rslavanyageetha/vader-a-comprehensive-guide-to-sentiment-analysis-in-python-c4f1868b0d2e)_

## **3** Topic Modelling <a class="anchor" id="3"></a>
I applied the **Latent Dirichlet Allocation (LDA)** method for topic modeling and used **PyLDAvis** to visualize the results.
To assess the quality of the topic modeling, I calculated the _coherence score_ and used a script to identify the model with the maximum coherence score.

_Read more about LDA in this [article](https://towardsdatascience.com/latent-dirichlet-allocation-lda-9d1cd064ffa2)_

## **4** Book Recommendations <a class="anchor" id="4"></a>
I currently have not made a book recommendation engine. In order to make this I will have to:
 1. Combine the sentiment analysis an topic modelling to create a user profile that shows their likes and dislikes
 2. Collect data on other books
 3. Identify topics in the other books
 4. Create the engine!!
