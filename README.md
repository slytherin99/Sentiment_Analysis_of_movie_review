# Sentiment_Analysis_of_movie_review

## Problem Statement

To predict the sentiment of the Hindi movie reviews after translation into English (using Google Translate) using Natural Language Processing.
Input: A set of hindi movie reviews.
Output: Sentiment Analysis as
                 Pos=1, Neg=0


Source of Training Data:

 https://www.kaggle.com/nltkdata/movie-review?select=movie_review.csv
 https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

 Source of Testing Data:

  https://github.com/shubham721/Sentiment-Analysis-On-Hindi-Reviews/blob/master/neg_hindi.txt
 https://github.com/shubham721/Sentiment-Analysis-On-Hindi-Reviews/blob/master/pos_hindi.txt

### install googletrans using pip
!pip install googletrans
### Importing the necessary libraries
import googletrans
from googletrans import Translator

## Preprocessing


Stemming : Used to cut down the common prefixes and suffixes used in words.

Lemmatization : Grouping together the different inflected forms of a word so they can be analysed as a single item. Basically, it links words with similar meaning to one word

*We removed unnecessary data using nltk:
 
Stopwords : Commonly used word (such as “the”, “a”, “an”, “in”) 

Punctuation : Removing all the punctuation marks such as “ , . etc

Null values : Removed all the rows with null values.

Count Vectorization: Counting the number of occurrences each words appears in the dataset.
 
Tf-idf ( frequency–inverse document frequency): Numerical statistic that is intended to reflect how important a word is to a document in a collection 


## Scope

1. Improving Accuracy by more preprocessing of Dataset. Also by implementing our Features like N-gram for better results. 

2. Training our model in such a way so that it can understand emojis and detect sarcasm.

3. Divide our sentiment into more classes like (neutral , somewhat positive, somewhat negative)

## Citations

[1]https://www.oreilly.com/library/view/applied-text-analysis/9781491963036/ch04.html
[2]https://towardsdatascience.com/text-classification-using-k-nearest-neighbors-46fa8a77acc5
[3]https://www.oreilly.com/library/view/applied-text-analysis/9781491963036/ch04.html
[4]https://www.youtube.com/watch?v=ZeQgNhc0vag
[5]https://github.com/shubham721/Sentiment-Analysis-On-Hindi-Reviews
[6]https://medium.com/analytics-vidhya/neural-machine-translation-for-hindi-english-sequence-to-sequence-learning-1298655e334a
[7]https://towardsdatascience.com/google-translate-api-for-python-723093c2144b

