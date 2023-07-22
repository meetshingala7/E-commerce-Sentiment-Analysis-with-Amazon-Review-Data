# E-commerce-Sentiment-Analysis-with-Amazon-Review-Data

This is available in the Base_Code_on_small_dataset.ipynb (5000 Rows of Data)<br>
I am currently scaling the code up to around 36,00,000 rows of data

The various Pre-Processing techniques used:
1. Tokenize
2. Removing all non-ascii characters (like Umlats)
3. Convert all characters to lower case characters
4. Remove all the punctuation marks in the dataset
5. Remove all the stopwords in the data set
6. Remove all the digits from the data set

Few other tasks that are also performed
1. Finding all the unique words
2. Finding total number of words
3. Finding the count of negative label and positive label

I also applied 3 stemmers:
1. Snowball Stemmer
2. Porter Stemmer
3. Lancaster stemmer 
To do a comparitive study

The Ray_demo.py file is an attempt on using Ray with the Pre-Processing techniques.
Using the ray library in the code for 1 particular code-block reduces the execution time to 46.195361%
The code block seperates that text that will be used for text classification from the whole line of text.
