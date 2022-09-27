# How to Clean Text Like a Boss for NLP in Python

One of the most common tasks in Natural Language Processing (NLP) is to clean text data.  In order to maximize your results, it's important to distill you text to the most important root words in the corpus.  This post will show how I typically accomplish this.  The following are general steps in text preprocessing:

* **Tokenization**: Tokenization breaks the text into smaller units vs. large chunks of text. We understand these units as words or sentences, but a machine cannot until they’re separated. Special care has to be taken when breaking down terms so that logical units are created. Most software packages handle edge cases (U.S. broke into the US and not U and S), but it’s always essential to ensure it’s done correctly.
* **Cleaning**: The cleaning process is critical to removing text and characters that are not important to the analysis. Text such as URLs, noncritical items such as hyphens or special characters, web scraping, HTML, and CSS information are discarded.
* **Removing Stop Words**: Next is the process of removing stop words. Stop words are common words that appear but do not add any understanding. Words such as “a” and “the” are examples. These words also appear very frequently, become dominant in your analysis, and obscure the meaningful words.:
* **Spelling**: Spelling errors can also be corrected during the analysis. Depending on the medium of communication, there might be more or fewer errors. Official corporate or education documents most likely contain fewer errors, where social media posts or more informal communications like email can have more. Depending on the desired outcome, correcting spelling errors or not is a critical step.
* **Stemming and Lemmatization**: Stemming is the process of removing characters from the beginning or end of a word to reduce it to their stem. An example of stemming would be to reduce “runs” to “run” as the base word dropping the “s,” where “ran” would not be in the same stem. However, Lemmatization would classify “ran” in the same lemma.

The following is a script that I’ve been using to clean a majority of my text data.  

Read more here: https://www.dataknowsall.com/textcleaning.html
