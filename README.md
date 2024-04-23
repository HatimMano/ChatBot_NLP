# School Chatbot Adventure: Doc2Vec Magic !

## Let's Dive In
Welcome to our school chatbot adventure! Our chatbot is here to help you with school questions using Doc2Vec magic !

## Getting Ready
Make sure you have these tools ready in your Python kit:
- pandas
- nltk
- gensim
- scikit-learn
- langdetect

## The Data
Our treasure trove lies in an Excel file named `Dataset_EFREI_en.xlsx`. Inside, you'll find questions and answers straight from our school's website.

## Getting Things Right
We prepped the data by:
- Making everything lowercase
- Removing stuff like links and emojis
- Getting rid of punctuation
- Cutting it into pieces
- Cleaning up common words
- Simplifying words

## The Magic Begins
Our chatbot uses Doc2Vec to find similar questions for each query. It's like finding twins for every question!

## Testing Time
We threw some questions at our chatbot to see how it does. If it wasn't sure about an answer (less than 50% sure), it gave a little heads up.

## The End Result
Our chatbot's pretty good with questions from our school stuff. It tries its best with new questions too, but sometimes it's not so sure. Still, it's a handy helper for school stuff!


## There are two questions from outside the dataset
1) Relevant question:
Question asked: Give me information about deadlines for applications.
Question twin: What be the deadline to apply for A overlord program ?
Similarity: 98.6%
Answer: students can apply throughout the year, and preferably before may 15th, to secure a place in our graduate program. be aware that some of our programs have limited availability; it is therefore recommended to apply early.

2) Irrelevant question:
Question asked: question completely irrelevant ?
Question "twin": Do I need to submit test scores such as GRE/GMAT ?
Similarity: 22.8%
Answer: We are sorry, we didn't understand your question.
