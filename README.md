# Fake-News-Detection-Using-Feature-Extraction

**Data Source**

Wang, William. (2017). "Liar, Liar Pants on Fire": A New Benchmark Dataset for Fake News Detection

**Information about the Dataset**

The dataset that we used for this project is called the LIAR dataset. It was created by Mr. William Yang from UC Santa Barbara.

The dataset is described as a benchmark dataset for fake news detection by the author. It has a total of 14 attributes and more than 10,000 instances. 

The dataset contained three files in .tsv format that included train, test and validation files. The train set and test set consists of 14 columns. Column 1 is the ID of the statement in the form of ([ID].json), Column 2 is the label. Column 3 is the statement under scrutiny. Column 4 is the subject(s). Column 5 is the name of the speaker. Column 6 is the speaker’s job title. Column 7 is the state information. Column 8 gives the speaker’s party affiliation. Column 9 gives the counts when the speaker has been previously truthful. Column 10 gives the number of times the speaker has given out false information. Column 11 gives the number of times when the speaker has spoken half-truths. Column 12 gives the count of mostly true instances of the speaker. Column 13 gives the counts of when the speaker has been caught giving out fake information(pants-on-fire counts). And finally, the column 14 gives the context, which includes the venue or location of the speech/statement).
**Prerequisites**

Python 3
Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy, scipy.
Python 3: https://www.python.org/downloads/
Anaconda: https://www.anaconda.com/download/

**Methodology used**

The project is based on extracting features from the LIAR dataset to understand how well each of the features created can enhance the prediction accuracy of the model.

We also developed unigram, bigram, trigram and fourgram models from our training set to see how well it performs on the test set and to see how well it describes the data.

 The features that we have developed are: a feature that counts the number of stopwords in every statement, multiple features related to each tag in the Penn treebank. 
 
 The dataset also comes with a few features like the truth counts, speaker name, state, etc. We will also be testing our features using more than one classifier to understand how  each classifier performs on our data and features.
 
 **Algorithms Used**
 
 KNN, Random Forest, Decision Tree, Logistic Regression, SVM, Multilayer Perceptron NN, Naive Bayes and Stochastic Gradient
 
**Evaluation**

The evaluation of the models was done using accuracy, recall, precision and F1 score 

**Results**

Random Forest works the best with all the features including existing and newly developed features. It gave an accuracy of 72.92% and an F1 score of 0.789. The second best classifier was Decision Tree. It gave an accuracy of 71.1% and an F1 score of 0.774. 
