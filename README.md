# Text-Classification---NLP
Assignment for the NLP course at An-Najah National University
----
In this assignment, the goal is to build a Naïve Bayes classification model that is able to predict the class (category) of an unseen document correctly out of 91 classes. Given the following datasets.
  - A training dataset: a collection of 91 folders whose names represent the class of the contained documents, i.e., the class of a specific document is the name of the folder holding this file. That means, all the documents are labeled.
  - A test dataset: this dataset has an organization similar to what is mentioned for the training dataset, i.e., the documents in the test sets are labeled and ready for evaluation purposes.
  
Follow the following steps that helps building a good classification model:
1.	Word Tokenization: splitting the text into uni-gram tokens.
You can either use you own tokenization methodology or the Stanford tokenizer: http://nlp.stanford.edu/software/tokenizer.html:

2.	Token normalization: use Porters’ Stemmer to return a token back to its base.
Java-based class for Porter’s Stemmer can be found here:
https://github.com/stanfordnlp/CoreNLP/blob/master/src/edu/stanford/nlp/process/Stemmer.java

3.	Vocabulary set extraction.

4.	Estimation of model parameters.
     - Estimate the prior distribution of the Naïve Bayes Classifier at each class.
     - Estimate the likelihood of each word in the training dataset for each class
     - Handle Zero probabilities using Add-1 Laplacian Smoothing and

6.	Document classification: predict the sentiment of each document in the test dataset using the model built in step 4.

7.	Model evaluation: Macro-averaged F1-score.

8.	EXTRA: think of new features that can be included into the Naïve Bayes Classifier, which contribute to improve the system performance.
