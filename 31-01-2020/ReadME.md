The Jupyter Notebook contains functionalities of four types of stemmers:
  1. Porter Stemmer: It is probably the simplest of the four stemmer and the earliest one as well. Suprisingly, it still worked for words
     such as dying, tying, lying but not for similar 'ying' word such as vying. So, it is rule based but also probably looks up from a very
     small dictionary of common words.
  2. Lancaster Stemmer: It performed well for words like trying, crying, laziness in for which the Porter Stemmer failed and failed for
     words for which the Porter Stemmer worked like tying, lying, dying, etc.
  3. Regex Stemmer: It is exactly what its name suggests. It jst checks for the matches of the given regular expression. It works well for 
     words which have just a suffix attached to the stem.
  4. Snowball Stemmer: It probably is the most advanced of the stemmers but suprisingly it gave exactly the same results as the Porter
     Stemmer for the words that were tested.
     
Along with that lemmatization was also done using the WordNetLemmatizer. Lemmatization refers to morphological analysis of words in order
to remove inflectional endings only and to return the base or dictionary form of a word, which is known as the lemma.
The results from the WordNetLemmatizer were satisfactory.

Finally simple count vectorization was performed using the count vectorizer available with scikit-learn. Vectorization basically refers to 
converting the text into a set of vectors based on its features so as to compare it with other similar vectors obtained from other texts as
well aa perform mathematical operations on it to gain a deeper knowledge.
