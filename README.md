# NLP-Project-Using-Enron-Emails-Dataset

Dataset: https://www.cs.cmu.edu/~./enron/ (May 7 2015 version)

Dataset must be downloaded into same folder as this notebook for it to run unaltered.

In this notebook I will detail my steps taken to perform certain NLP tasks from the starting point of an unstructured dataset containing raw text in the form of emails.

The hypothesis for the final classifier is as follows:

It is possible that the tone of emails changes depending in the relationship between the senders and recievers. Specifically, you might expect emails sent externally (e.g. to clients) would be written in a more formal way that emails sent internally to colleagues who know each other well. The main aim of this notebook is to build a classifier using deep learning capable of predicting whether an email was sent internally or not from an extract of the email text-body. 

If successful, a company who wishes to ensure culture of consistent professionalism from all employees, even when talking internally, could use the classifier to flag employees who are overly informal when sending emails to external persons (indicated low specicifity) or internally (indicated by high sensitivity). This would work by passing a sample of individual employee's emails through the classifier to find their individual scores.

A binary classifier of internally (only) vs externally viewed emails was created using an RNN which achieved a test accuracy of 0.9.

Running the notebook is dependent on the following:

- numpy
- pandas
- tensorflow
- string
- spacy
- en_core_web_sm
- collections
- nltk
- tensorflow
- keras
- sklearn
- matplotlib
- seaborn
- PIL
- wordcloud
