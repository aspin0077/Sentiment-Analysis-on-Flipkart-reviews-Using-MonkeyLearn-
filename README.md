# Sentiment-Analysis-on-Flipkart-reviews-Using-MonkeyLearn-
This is my mini-project for my degree of M.Sc Data Analytics

I. INTRODUCTION
As there is large volume of data in the world, individuals are proposed to
develop a framework that can distinguish and classify data based on opinions.
Sentiment analysis (opinion mining) can be considered as the one of the major
application of Natural Language Processing (NLP). We are looking forward to
sentiment in product reviews using MonkeyLearn API[7]. We have used web
scraping method to retrieve product reviews from Flipkart website which is used
as dataset in this experiment. Finally, we compare the sentiment reviews, so that
decision making will be lot easier for the user regarding purchasing of the
product.
Web Scraping means extracting information from websites by parsing the
HTML of the webpage[8]. Parsing a HTML webpage is really easy in Python.
You can get the relevant information you need using just a few lines of code in
Python. As Flipkart is a famous one the product reviews from this website is
considered for scrapping.
Text communication is one of the most popular forms of day today
conversion. We chat, message, tweet, share status, email, write blogs, share
opinion and feedback in our daily routine. All of these activities are generating
text in a significant amount, which is unstructured in nature. In this area of the
online marketplace and social media, it is essential to analyse vast quantities of
data, to understand people’s opinion.
NLP enables the computer to interact with humans in a natural
manner. It helps the computer to understand the human language and derive
meaning from it. NLP is applicable in several problematic from speech
recognition, language translation, classifying documents to information
extraction[6].
Opinion mining also known as sentiment analysis technique
implements various algorithms to analyse the corpus of data and make sense out
of it. This technique helps to identify the orientation of a sentence thereby
recognising the element of positivity or negativity in it. Automated opinion mining
can be implemented through a machine learning based approach. Opinion mining
uses natural language processing to extract the subjective information from the
data (in this case its customer reviews[2]).
2
i. Objectives
There is an increase in demand for e-commerce with people
preferring online purchasing of goods and products. The e-commerce websites
are loaded with large volume of data. Also, social media helps a great deal in
sharing of this information. This has greatly influenced consumer habits all over
the world. Due to the vivid reviews provided by the customers, there is a feedback
environment being developed for helping customers buy the right product and
guiding companies to enhance the features of product suiting consumer’s
demand[3]. The only disadvantage of availability of this huge volume of data is
its diversity and its structural non-uniformness.
The customer finds it difficult to precisely find the review for a
particular feature of a product that they intend to buy. Also, there is a mixture of
positive and negative reviews thereby making it difficult for customer to find a
cogent response. Also these reviews suffer from spammed reviews from
unauthenticated users. So to avoid this confusion and make this review system
more transparent and user friendly we propose a technique to extract feature
based opinion from a diverse pool of reviews, segregate it with respect to the
aspects of the product and further classifying it into positive and negative reviews
using machine learning based approach. The objectives of this work are to:
 Perform web scraping of product reviews from Flipkart[8].
 Perform sentiment analysis of the web scrapped product
reviews[1].
3
II. BACKGROUND
i. Scraped Product Reviews
Scraping Customer Reviews from Flipkart[8] can be useful for
 Getting complete review details that you can’t get with
python.
 Monitoring customer opinion on products that you sell or
manufacture using Data Analysis.
 Create Flipkart Review Datasets for Educational Purposes
and Research.
Requests, is one of the packages in Python that made the language
interesting. Requests is based on Python’s urllib2 module. Requests gets the web
page for you, but you need to parse the HTML from the page to retrieve the data.
That is done by BeautifulSoup. Some use lxml to parse the HTML, but in this
work BeautifulSoup is used.
ii. Data Pre-processing
The first step should be cleaning the data in order to obtain
better features. We will achieve this by doing some of the basic pre-processing
steps on our data[6]. Some text pre-processing steps are,
 Lower casing
 Punctuation removal
 Stop words removal
 Frequent words removal
 Rare words removal
 Spelling correction
iii. Sentence Extraction
Once you have identified, extracted, and cleansed the content
needed for your use case, the next step is to have an understanding of that content.
In many use cases, the content with the most important information is written
down in a natural language (such as English, German, Spanish, Chinese, etc.) and
not conveniently tagged. To extract information from this content you will need
to rely on some levels of text mining, text extraction, or possibly full-up natural
language processing (NLP) techniques[5].
4
 Tokenization
 Stemming
 Lemmatization
iv. Classification
Text classification[4] is the process of assigning predefined
tags or categories to unstructured text. It's considered one of the most useful
Natural Language Processing (NLP) techniques because it's so versatile and can
organize, structure and categorize pretty much anything to deliver meaningful
data and solve problems.
CLASSIFICATION ALGORITHMS
The classification[6] step usually involves a statistical model like Naïve
Bayes, Logistic Regression, Support Vector Machines, or Neural Networks.
 Naïve Bayes:
A family of probabilistic algorithms that uses Bayes Theorem to
predict the category of a text.
 Linear Regression:
A very well-known algorithm in statistics used to predict some value
(Y) given a set of features (X).
 Support Vector Machines:
A non-probabilistic model which uses a representation of text
examples as points in a multidimensional space. These examples are
mapped so that the examples of the different categories (sentiments)
belong to distinct regions of that space.. Then, new texts are mapped
onto that same space and predicted to belong to a category based on
which region they fall into.
 Deep Learning:
A diverse set of algorithms that attempts to imitate how the human
brain works by employing artificial neural networks to process data.
5
III. PROPOSED WORK
i. Block Diagram:
The block diagram of the proposed system is given in figure 1.
Figure.1 Block diagram of the proposed system
ii. Methodology:
a) Scraped Product Reviews
Requests, is one of the packages in Python that made the language
interesting. Requests is based on Python’s urllib2 module. Requests gets the web
page for you, but you need to parse the HTML from the page to retrieve the data.
That is done by BeautifulSoup. Some use lxml to parse the HTML, but in this
work BeautifulSoup is used.
b) Data Pre-processing
 Punctuation removal
As it doesn’t add any extra information while treating
text data.
 Stop words removal
Stop words (or commonly occurring words) should be
removed from the text data.
6
 Frequent words removal
We just removed commonly occurring words in a
general sense.
 Rare words removal
We removed the most common words, this time let’s
remove rarely occurring words from the text. Because
they’re so rare.
c) Sentence Extraction
To extract information from this content you will need to rely
on some levels of text mining, text extraction, or possibly full-up natural language
processing (NLP) techniques.
 Tokenization
It will make each words separate in a sentence.
 Stemming
Stemming refers to the removal of suffices by a simple
rule-based approach.
 Lemmatization
It makes use of the vocabulary and does a
morphological analysis to obtain the root word.
d) Classification
Below, we're going to focus the most common text
classification task of sentiment analysis,
 Product Sentiment Analysis[3]
This machine learning tool can provide insights by automatically
analysing product reviews and separating them into tags: Positive, Neutral and
Negative. By using sentiment analysis to structure product reviews, you can,
 Understand what your customers like and dislike about your
product.
 Compare your product reviews with those of your
competitors.
 Get the latest product insights in real-time, 24/7.
 Save hundreds of hours of manual data processing.
7
e) Score Computation
We can automate product review analysis with machine
learning. We can build our own text analysis model without needing to know how
to code or have experience in machine learning. From figure.2, we can see
MonkeyLearn API[7] will gives a tag of sentiment and its confidence level in
percentage.
Figure.2 Score computation using Monkeylearn.
8
IV. IMPLEMENTATION
i. Coding And Explanation:
This is the coding for importing required libraries for web scraping
and basic operations in database. Requests, is one of the packages in Python that
made the language interesting. Requests is based on Python’s urllib2 module.
Requests gets the web page for you, but you need to parse the HTML from the
page to retrieve the data. That is done by BeautifulSoup.
9
The above code is used to scrap a product review for a particular
product of DELL Vostro 3478 14” Laptop in FLIPKART[8]. Output is
showing the product reviews by the customers.
One of the most basic features we can extract is the number of words
in each review. The basic intuition behind this is that generally, the negative
sentiments contain a lesser amount of words than the positive ones.
This feature is also based on the previous feature intuition. Here, we
calculate the number of characters in each review. This is done by calculating the
length of the review.
10
We will also extract another feature which will calculate the average
word length of each review. This can also potentially help us in improving our
model. Here, we simply take the sum of the length of all the words and divide it
by the total length of the review:
Generally, while solving an NLP problem, the first thing we do is to
remove the stopwords. But sometimes calculating the number of stopwords can
also give us some extra information which we might have been losing before.
Here, we have imported stopwords from NLTK, which is a basic NLP library in
python.
11
The next step is to remove punctuation, as it doesn’t add any extra
information while treating text data. Therefore removing all instances of it will
help us reduce the size of the training data.
As we discussed earlier, stop words (or commonly occurring words)
should be removed from the text data. For this purpose, we can either create a list
of stopwords ourselves or we can use predefined libraries.
12
In statistics, a frequency distribution is a list, table or graph that
displays the frequency of various outcomes in a sample. Each entry in the table
contains the frequency or count of the occurrences of values within a particular
group or interval.
13
Frequency is a built-in function which comes under the statistical
category. The frequency distribution can be defined as a list of data or graph that
gives the frequency of various outcomes.
Previously, we just removed commonly occurring words in a
general sense. We can also remove commonly occurring words from our text data
first, let’s check the 10 most frequently occurring words in our text data then take
call to remove or retain.
Similarly, just as we removed the most common words, this time
let’s remove rarely occurring words from the text. Because they’re so rare, the
association between them and other words is dominated by noise. You can replace
rare words with a more general form and then this will have higher counts
14
Stemming refers to the removal of suffices, like “ing”, “ly”, “s”, etc.
by a simple rule-based approach. For this purpose, we will use PorterStemmer
from the NLTK library.
Lemmatization is a more effective option than stemming because it
converts the word into its root word, rather than just stripping the suffices. It
makes use of the vocabulary and does a morphological analysis to obtain the root
word. Therefore, we usually prefer using lemmatization over stemming.
15
Term frequency is simply the ratio of the count of a word present in
a sentence, to the length of the sentence. Therefore, we can generalize term
frequency as:
TF = (Number of times term T appears in the particular row) /
(number of terms in that row)
The intuition behind inverse document frequency (IDF) is that a
word is not of much use to us if it’s appearing in all the documents. Therefore,
the IDF of each word is the log of the ratio of the total number of rows to the
number of rows in which that word is present.
IDF = log(N/n),
Where, N is the total number of rows and n is the number of rows in
which the word was present.
16
We can see that the TF-IDF has penalized words like ‘don’t’, ‘can’t’,
and ‘use’ because they are commonly occurring words. However, it has given a
high weight to “disappointed” since that will be very useful in determining the
sentiment of the review.
17
A tag cloud (word cloud, or weighted list in visual design) is a
novelty visual representation of text data, typically used to depict keyword
metadata (tags) on websites, or to visualize free form text. Tags are usually single
words, and the importance of each tag is shown with font size or colour. This
format is useful for quickly perceiving the most prominent terms to determine its
relative prominence.
Our problem was to detect the sentiment of the review. So, before
applying any ML/DL models (which can have a separate feature detecting the
sentiment using the textblob library), let’s check the sentiment of the reviews.
18
Above, you can see that it returns a tuple representing polarity and
subjectivity of each review. Here, we only extract polarity as it indicates the
sentiment as value nearer to 1 means a positive sentiment and values nearer to -1
means a negative sentiment. This can also work as a feature for building a
machine learning model.
In this section using MonkeyLearn package we can analyse our data
of product reviews. For that first we want to sign up for free in MonkeyLearn
webpage[7] using our E-mail id. By that we can get Your_API_Key. Using that
we can easily classify our text data for product sentiment analysis.
By using that code and API we get the output of sentiment_tag and
confidence level.
19
V. EXPERIMENTS AND RESULTS
In this experiment, we show web-scrap review of DELL Vostro 3478
Laptop from Flipkart website[8]. Product reviews were extracted using web
scraping method which was implemented in Python 3(Jupyter Notebook) using
BeautifulSoup library, which was implemented in Windows 10 with an Intel®
Core™ i5-8th Gen. Processor (@3.00 GHz) and 4 GB RAM.
Figure. 3 Pie chart on reviews
In Figure.3, Pie chart on reviews, it shows a pie chart of the review
data which is the customer review of a Dell Vostro 3478 laptop on Flipkart page.
By this chat, we can conclude that for that particular product most of the
customers giving positive review.
Nearly 90% of customers raise the review as positive. By the
negative reviews we can propose an ideas for further manufacturing for that
laptop company.
20
VI. CONCLUSION AND FUTURE WORK
In this experiment, we have proposed scrap review data from the
Flipkart website, and makes classification based on customer reviews on
particular product of DELL Vostro 3478 Laptop. In this project, we compare
product reviews by MonkeyLearn API, so that decision making will be a lot easier
for the user regarding purchasing of the product.
Additionally, depending on time constraints, we also plan on
introducing a portal for laptop manufacturers to analyse the public perception of
their product over time and identify key areas where their product can be
improved.
For future work, we can implement this project on Google’s
TensorFlow, which is an open source framework for machine learning. And also
I have an idea to make a website for sentiment analysis by this code without
MonkeyLearn API (for that we should have real time structured data for training)
for text, audio data.
21
REFERENCES
Research Papers:
1. Mahek Merchant, Ricky Parmar (2016). Sentiment Analysis of Web Scraped
Product Reviews using Hadoop. Volume 4 Issue VIII, IC Value: 13.98 ISSN:
2321-9653.
2. Pratiksha Ashiwal, S.R.Tandan, Priyanka Tripathi, Rohit Miri (2016). Web
Information Retrieval Using Python and BeautifulSoup. Volume 4 Issue VI,
IC Value: 13.98 ISSN: 2321-9653.
3. Devendra Kamalapurkar, Ninad Bagwe, R. Harikrishnan, Salil Shahane, Mrs.
Manisha Gahirwal (2017). SENTIMENT ANALYSIS OF PRODUCT
REVIEWS. ISSN: 2277-9655.
URLs:
4. https://www.datacamp.com/community/tutorials/text-analytics-beginnersnltk
5. https://www.analyticsvidhya.com/blog/2018/02/the-different-methods-dealtext-
data-predictive-python/
6. https://medium.com/@bedigunjit/simple-guide-to-text-classification-nlpusing-
svm-and-naive-bayes-with-python-421db3a72d34
7. https://monkeylearn.com/api/v3/?python#create-classifier
Scraped product review webpage:
8. https://www.flipkart.com/dell-vostro-14-3000-core-i5-8th-gen-4-gb-1-tbhdd-
linux-2-gb-graphics-3478-
laptop/p/itmf4daar3urw6yr?pid=COMF4DAAMGHXCHXH&lid=LSTCO
MF4DAAMGHXCHXHH24PRM
