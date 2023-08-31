# E-commerce-Sentiment-Analysis-with-Amazon-Review-Data

<h6>
  The files PreProcessing_DF_with_NLP.ipynb and Processing_text_data_to_Dataframe.ipynb are files that are being updated and a project with a Larger dataset is being made on my end. The File Base_code_on_small_Dataset.ipynb is the project made over small dataset. 
</h6>
<br>
<h3>Exploratory Data Analysis</h3>
The project takes in a dataset from Kaggle of 4000 rows and 8 Columns of training data and 1000 rows testing data. There are initially 3 classes for classification. The 3 classes are Positive, Neutral and Negative. The column 'review.text' is used for classification. The dataset Majorly comprises of Positive Data points(3749) and the Neutral is converted into negative data since either customer likes the product or doesnt like the product. 

The following image displays the bias in the dataset towards positive comments.
<h3> The Training data</h3>

![sb_countplot_train_data](https://github.com/meetshingala7/E-commerce-Sentiment-Analysis-with-Amazon-Review-Data/assets/123167152/41f2fe1a-df6e-45d7-859a-fe63644766dc)

<h3> The Testing data</h3>

![sb_countplot_test_data](https://github.com/meetshingala7/E-commerce-Sentiment-Analysis-with-Amazon-Review-Data/assets/123167152/53f60746-3f74-485b-bc62-75a017620dae)

<h6>The project I am working as mentioned above has equal spread</h6>

<br>
1. There are a total of 23 Unique Categories which the dataset is made up from. <br>
2. There are 6541 unique words in the dataset. <br>
3. There are 6528800 total words in the dataset. <br>

<h3>Pre-Processing</h3><br>
The NLP techniques used were:<br>
1. Tokenization (using nltk.tokenize)<br>
2. Removal of all Non-Ascii Values like Umlats etc.<br>
3. Convert all the tokens to lowercase characters.<br>
4. Remove all the punctuation marks from text data.<br>
5. Removal of the stopwords from that dataset.<br>
6. Removal of all the digits.<br>

Here, I used the Snow Stemmer from sklearn.stem.SnowballStemmer


| Models |Accuracy with TFIDF vectorizer  | Accuracy with CV vectorizer |
| ------------- | ------------- | ------------- |
| Multinomial Naive-Bayes | 94.59%  | 93.69%  |
| Support Vector Machine | 94.39%  | 94.19%  |
| K-Nearest Neighbours | 94.29% | 93.79% |
| Multi layer Perceptron | 95.09% | 94.19% |
| Random Forest Classifier | 93.69% | 93.69% |


The Table of Precision

|Model                   | Precision with TFIDF Vectorizer | Precision with CountVectorizer|
| ------------- | ------------- | ------------- |
|Multinomial Naive-Bayes | 0.8779                   | 0.9366                  |
|Support Vector Machine  | 0.9409                   | 0.9386                  |
|K-Nearest Neighbours                     | 0.9307                   | 0.9307                  |
|MLP                     | 0.9414                   | 0.9415                  |
|Random Forest           | 0.8778                   | 0.8778                  |

The Table of Recall


|Model                   | Recall with TFIDF Vectorizer | Recall with CountVectorizer |
| ------------- | ------------- | ------------- |
|Multinomial Naive-Bayes | 0.9369                   | 0.9459                  |
|Support Vector Machine  | 0.9439                   | 0.9419                  |
|K-Nearest Neighbours    | 0.9429                   | 0.9429                  |
|Multi layer Perceptron                     | 0.9449                   | 0.9459            |
|Random Forest Classifier          | 0.9369                   | 0.9369       |


I ran the model for 100 Nearest Neighbours for the data in KNN 
The accuracy plot for KNN with TFIDF Vectorizer
![TFIDF_ACC_KNN](https://github.com/meetshingala7/E-commerce-Sentiment-Analysis-with-Amazon-Review-Data/assets/123167152/3163160a-ac84-435a-9b13-b48098963bf1)

The accuracy plot for KNN with CV Vectorizer

![CV_ACC_KNN](https://github.com/meetshingala7/E-commerce-Sentiment-Analysis-with-Amazon-Review-Data/assets/123167152/0518b578-e334-43b0-a042-3f7ea85ead3d)
