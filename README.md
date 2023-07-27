# E-commerce-Sentiment-Analysis-with-Amazon-Review-Data

<h6>
  The files PreProcessing_DF_with_NLP.ipynb and Processing_text_data_to_Dataframe.ipynb are files that are being updated and a project with a Larger dataset is being made on my end. The File Base_code_on_small_Dataset.ipynb is the project made over small dataset. 
</h6>
<br>
<h3>Exploratory Data Analysis</h3>
The project takes in a dataset from Kaggle of 4000 rows and 8 Columns of training data and 1000 rows testing data. There are initially 3 classes for classification. The 3 classes are Positive, Neutral and Negative. The column 'review.text' is used for classification. The dataset Majorly comprises of Positive Data points(3749) and the Neutral is converted into negative data since either customer likes the product or doesnt like the product. 
<br>
![image](https://github.com/meetshingala7/E-commerce-Sentiment-Analysis-with-Amazon-Review-Data/assets/123167152/7758f81d-43b0-4030-ab00-2a710917d154)>
<br>
1. There are a total of 23 Unique Categories which the dataset is made up from.
2. There are 6541 unique words in the dataset.
3. There are 6528800 total words in the dataset.

<h3>Pre-Processing</h3>
The NLP techniques used were:
1. Tokenization (using nltk.tokenize)
2. Removal of all Non-Ascii Values like Umlats etc.
3. Convert all the tokens to lowercase characters.
4. Remove all the punctuation marks from text data.
5. Removal of the stopwords from that dataset.
6. Removal of all the digits.

<>
