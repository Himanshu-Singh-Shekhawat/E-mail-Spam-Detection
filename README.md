**E-mail-Spam-Detection**

Email is one of the very important tool for communication. To have effective communication, spam filtering is one of the important feature.

**➲ Project description**
Email spam detection system is used to detect email spam using Machine Learning technique called Natural Language Processing and Python, where we have a dataset contain a lot of emails by extract important words and then use naive classifier we can detect if this email is spam or not.

**➲ Prerequisites**
This is list of required packages and modules for the project to be installed :

1. Python
2. Pandas
3. Numpy
4. Scikit-learn
5. NLTK

**➲ The Dataset**
Human activites dataset contain about 5728 record which is a sample of an email
and a target column "type" which describe the state of an email spam or not.

Dataset features and target :

Dataset head :

**➲ Outline Sections**

• Created a model that detect spam messages.
• Collected data from various resources.
• Performed Data Cleaning,EDA,Text Preprocessing.
• Model building - Used various M.L. algorithm to check model accuracy and precision. Then Evaluation and Improvement.

**➲ Data Cleaning**
Let’s Analyze the Data take a look at the email message content and have a basic understanding of the data

Ham
This looks like a normal email reply to another person, which is not difficult to classified as a ham.

Spam
One of the spam training data does look like one of those spam advertisement email in our junk folder.

## Visualization

1. Wordcloud:-
Wordcloud is a useful visualization tool for you to have a rough estimate of the words that has the highest frequency in the data that you have.
<img  alt="Coding" width="500" src="https://miro.medium.com/max/720/1*QcsZSm5Bj4Vo-6DTJUizwQ.webp">

From this visualization, you can notice something interesting about the spam email. A lot of them are having high number of “spammy” words such as: free, money, product etc. Having this awareness might help us to make better decision when it comes to designing the spam detection system.

<img  alt="Coding" width="500" src="https://miro.medium.com/max/720/1*yJ-ODGRYXoUIiVatjKMlRg.webp">

One important thing to note is that word cloud only displays the frequency of the words, not necessarily the importance of the words. Hence it is necessary to do some data cleaning such as removing stopwords, punctuation and so on from the data before visualizing it.

## N-grams model visualization

Another technique of visualization is by utilizing bar chart and display the frequency of the words that appear the most. N-gram means that how many words you are considering as a single unit when you are calculating the frequency of words.
<img  alt="Coding" width="400" src="https://miro.medium.com/max/720/1*4r0AUyzW6qG0YJReV6vEEA.webp">

## Train Test Split
It is important to split your data set to training set and test set, so that you can evaluate the performance of your model using the test set before deploying it in a production environment.

One important thing to note when doing the train test split is to make sure the distribution of the data between the training set and testing set are similar.

What it means in this context is that the percentage of spam email in the training set and test set should be similar.

<img  alt="Coding" width="400" src="https://miro.medium.com/max/720/1*gf8EwdBiWdxZHY4j1r9wqA.webp">

<img  alt="Coding" width="400" src="https://miro.medium.com/max/640/1*d1gosJDGJmD5i9l6mW9Gzw.webp">

**➲ Data Preprocessing**

## Text Cleaning

Text Cleaning is a very important step in machine learning because your data may contains a lot of noise and unwanted character such as punctuation, white space, numbers, hyperlink and etc.

Some standard procedures that generally use are:

convert all letters to lower/upper case
removing numbers
removing punctuation
removing white spaces
removing hyperlink
removing stop words such as a, about, above, down, doing and the list goes on…
Word Stemming
Word lemmatization


1. Word stemming — Stemming algorithms work by removing the end or the beginning of the words, using a list of common prefixes and suffixes that can be found in that language.
2. Word Lemmatization — Lemmatization is utilizing the dictionary of a particular language and tried to convert the words back to its base form. It will try to take into account of the meaning of the verbs and convert it back to the most suitable base form

## Feature Extraction
Our algorithm always expect the input to be integers/floats, so we need to have some feature extraction layer in the middle to convert the words to integers/floats.

There are a couples ways of doing this, and today I am going to introduce:

CountVectorizer
TfidfVectorizer

1. CountVectorizer :- First we need to input all the training data into CountVectorizer and the CountVectorizer will keep a dictionary of every word and its respective id and this id will relate to the word count of this word inside this whole training set

2. TfidfVectorizer :- Word counts are good but can we do better? One issue with simple word count is that some words like ‘the’, ‘and’ will appear many times and they don’t really add too much meaningful information.So another popular alternative is TfidfVectorizer. Besides of taking the word count of every words, words that often appears across multiple documents or sentences, the vectorizer will try to downscale them.

## Precision & Recall 
precision is evaluating, when a model predict something as positive, how accurate the model is. On the other hand, recall is evaluating how well a model in finding all the positive samples.

**➲ Contact**

E-mail : himanshusinghshekhawat8@gmail.com

LinkedIn : https://www.linkedin.com/in/himanshu-singh-shekhawat-2b5450154
