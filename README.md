# NLP-Project-Using-Enron-Emails-Dataset

Dataset: https://www.cs.cmu.edu/~./enron/ (May 7 2015 version)

The dataset 'maildir' referenced above must be downloaded into the same directory as the 'NLP Project Using Enron Emails Dataset.ipynb' notebook.

In the notebook 'NLP Project Using Enron Emails Dataset V3.ipynb' I will detail my steps to perform NLP tasks from the starting point of an unstructured dataset containing raw text in the form of emails.

The hypothesis for the final classifier is as follows:

It is possible that the tone of emails changes depending on the relationship between the senders and receivers. Specifically, you might expect emails sent externally (e.g. to clients) would be written in a more formal way than emails sent internally to colleagues who know each other well. The main aim of this notebook is to build a classifier, using deep learning, capable of predicting whether an email was sent internally or not from an extract of the email text-body.

This was chosen as a single example to highlight the kinds of powerful insights that a company may be able to find within their staff emails. From this example, a company who wishes to ensure a culture of consistent professionalism from all employees, even when talking internally, could use the classifier to flag employees who are overly informal when sending emails to external persons (indicated low specificity) or internally (indicated by high sensitivity). This would work by passing a sample of an individual employee's emails through the classifier to find their personal scores.

A binary classifier of internally (only) vs externally viewed emails was created using an RNN which achieved a test accuracy of 0.97.

The files for the neural network configuration and corresponding weights are now included, to be used as a starting point for future work on this project ('Enron_RNN.json' and 'Enron_RNN_weights.h5').

The notebook is dependent on the following:

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
