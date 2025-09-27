## Implementing solutions using Python - part 1
# Problem 1:  Write an ELIZA-style chatbot that can hold conversations along the lines of the following conversation. The parentheses provide options of input.
1. Person: Where am I?
• Bot: Next to me.
2. Person: (How did I come here?) (What brought me here?) (What am I doing here?)
• Bot: You have been selected by the Matrix.
3. Person: (Who is the matrix?) (Who is this Matrix you are talking about?) (What are you talking about?)
• Bot: It is the future.
4. Person: (anything else)
• Bot: Things will become clearer soon

# Problem 2: Author attribution using the n-gram language model
Authorship attribution is the problem of identifying the author of a given document by looking at other writings by the
same author.
For example, given two works by William Shakespeare and two by Jane Austen, try to identify the potential author of a
sentence that didn’t appear in any of the works given.
One way of tackling this problem is to learn two n-gram models, one for Shakespeare and one for Austen as shown
below. Then look up the probabilities of all the n-grams in the new sentence and multiply them to end up with the
total likelihood of the sentence. 

# Problem 3: Fake versus real news classification using naive Bayes
Given a dataset of real and fake news, we will implement a Naive Bayes classifier and test it. In this task we are
going to lookup various suggested libraries to achieve the steps mentioned below.
Data summary
• Data: fake_or_real_news.csv
• Columns: index, title, text, label
• The label column indicates whether the text is ‘FAKE’ or ‘REAL’
Requirements
1. Load and inspect the data (we can use Pandas).
2. Split the data into 70% training and 30% testing data.
3. Compute the bag-words on the training data (we can use NLTK or scikit-learn).
4. Use the same vocabulary in the training data to compute the bag-words of the text in testing data.
5. Train a naive Bayes classifier on the training data (we can use NLTK or scikit-learn).
6. Test the accuracy of the fitted model accuracy and confusion matrix on the testing data (we can use scikit-learn).
