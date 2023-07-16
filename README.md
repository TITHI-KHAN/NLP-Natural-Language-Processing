# NLP (Natural Language Processing)

# Feature Extraction

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/ed71dc6b-2ae0-48b3-ab0f-d5fa97b02e7b)

It converts the text data into numerical data -> Feature extraction for text. 

Individual numerical value will be generated for each word and it will be represented by a vector later on.  A set of numeric vector will represent a sentence.

# Beautiful Soap Tool

Beautiful Soup is a library that makes it easy to scrape information from web pages. It sits atop an HTML or XML parser, providing Pythonic idioms for iterating, searching, and modifying the parse tree.

# Text Processing in NLP

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/c30ded4d-9c85-410d-a458-fc113fba74f5)

Corpus-> Lots of text. Ex: Wikipedia, Text data of website, Text data of Google, etc.

**Type of Tokens:**

1. Word tokens
2. Character tokens
3. Sentence tokens
4. Named entity tokens
5. Part-of-speech (POS) tags
6. Sub-word tokens

**1. Word Tokenization:** (Mostly used)

I love Bangladesh.

Each one will be considered a different word and we will get individual token. I -> a word, love ->a word, Bamngladesh ->a word.

**2. Character tokens:**

I love Bangladesh.

I -> a character.
l -> a character.
o -> a character.
v -> a character.
e -> a character.
B -> a character.
a -> a character.
n -> a character.
g -> a character.
l -> a character.
a -> a character.
d -> a character.
e -> a character.
s -> a character.
h -> a character.

**3. Sentence tokens:**

I love Bangladesh.

Here, we only have 1 sentence. So, 1 token.

**4. Named entity tokens:**

I love Bangladesh.

Bangladesh - > 1 token. Because, this is a name. 

This method will only recognize name(s) from chunk or full text. 

**5. Part-of-speech (POS) tags:**

It will only match the part of speech.

**6. Sub-word tokens:**

I love Bangladesh.

Bangladesh -> Bang (sub-word)

in-depth -> in (sub-word)

# Text Preprocessing

Stemming and Lemmatization are Text Normalization (or sometimes called Word Normalization) techniques in the field of Natural Language Processing that are used to prepare text, words, and documents for further processing. Stemming and Lemmatization have been studied, and algorithms have been developed in Computer Science since the 1960s. We will learn about Stemming and Lemmatization in a practical approach covering the background, some famous algorithms, applications of Stemming and Lemmatization, and how to stem and lemmatize words, sentences, and documents using the Python nltk package which is the Natural Language Tool Kit package provided by Python for Natural Language Processing tasks.

The text might be in Banglish or some of them are in Bangla and some of them are in English, then there are lots of preprocessing tools for this.

In preprocessing, there are some common words that needs to be removed. Unnecessary letter (noise) can be removed. Text can also be normalized (Ex: Lemmatization, Word Net Lemmatizer, Dawson, N-Gram, Stemming, etc.). The most famous ones are Lemmatization and Stemming.

**Word Normalization:**

The morphological ending or beginning of a word or the same type of word will be removed and the number of similar types of words will increase. Then, those will be tokenized.

 Love & Loving -> both are Love related. If we consider them individually, then Love-1, Love-2. Even if we consider Good & Best individually, their meanings are almost same. So, Good-1 & if the value of Best is 1, then it would also be better. That means, its priority is high and it has more frequency than others.

**Tokenization:**

I love Bangladesh. 

In this case, they will be separated and each will be considered a token. Each token will have a different id. This token & id will be mapped. 

The token will be taken again from Feature Hashing. These will take place in an iterative way. 

After preprocessing, the text will be taken as input and based on those data, we will do feature extraction. Then, we will convert into numeric format (feature extraction).
 
**Stemming:**

Stemming is the process of reducing a word to its word stem that affixes to suffixes and prefixes or to the roots of words known as a lemma. Stemming is important in natural language understanding (NLU) and natural language processing (NLP). When a new word is found, it can present new research opportunities. For example -

![image](https://github.com/TITHI-KHAN/NLP-Natural-Language-Processing/assets/65033964/bbdd51e7-0973-4b9e-b5a0-bfe7bd429a5b)

Here, **wait** -> after stemming, it works as the representative and this actual word can either belong to the dictionary or not. Sometimes, we get **chang** instead of change. Even though it does not belong to the dictionary, it works as a representative after stemming.

▪ **Porter Stemmer():** 

The Porter stemming algorithm (or 'Porter stemmer’) removes the commoner morphological endings from words in English. The Porter stemming algorithm, also known as the Porter stemmer, is a popular stemming algorithm used to remove common morphological endings from English words. Stemming is the process of reducing a word to its base or root form, which can help improve information retrieval, text analysis, and natural language processing tasks.

▪ **Lovins Stemmer:**

The Lovins stemmer is another stemming algorithm that focuses on removing various types of suffixes from words. It was developed by J. C. Lovins and is based on a set of transformation rules.

▪ **Dawson Stemmer:**

The Dawson stemmer is an algorithm developed by R.C. Dawson. It is a rule-based stemming algorithm that aims to remove common English suffixes from words.

▪ **Krovetz Stemmer:**

The Krovetz stemmer is a stemming algorithm designed specifically for information retrieval applications. It is an extension of the Porter stemmer and incorporates additional rules to handle various linguistic patterns.

▪ **Xerox Stemmer:**

The Xerox stemmer, also known as the Xerox Incremental Parser, is a rule-based stemmer developed at Xerox PARC. It uses a set of rules and patterns to strip common suffixes from English words.

▪ **N-Gram Stemmer:**

The N-Gram stemmer is a statistical algorithm that utilizes n-grams, which are contiguous sequences of n items (typically letters), to identify common word stems. It focuses on capturing the statistical patterns of word endings.

▪ **Snowball Stemmer:**

The Snowball stemmer, also known as the Porter2 stemmer, is an extension of the original Porter stemmer. It supports multiple languages and provides improved stemming performance compared to the Porter stemmer.

▪ **Lancaster Stemmer:**

The Lancaster stemmer is an aggressive stemming algorithm developed at Lancaster University. It applies a set of rules to remove both prefixes and suffixes from English words, often resulting in very aggressive stemming.

**Lemmatization:**

Lemmatization usually refers to doing things properly with the use of a vocabulary and morphological analysis of words, normally aiming to remove inflectional endings only and to return the base or dictionary form of a word, which is known as the lemma.

It also normalizes like the stemming but after normalization, the representative word belongs to a dictionary. 

▪ Word Net Lemmatizer (Mostly used)
▪ Spacy Lemmatizer
▪ TextBlob
▪ Gensim Lemmatizer
▪ TreeTagger

**WordNet Lemmatizer:** 

The WordNet Lemmatizer is a lemmatization tool that is commonly used in NLP tasks. It maps words to their base or dictionary form based on WordNet's lexical database. It takes into account the word's part of speech (POS) to determine the appropriate lemma.

**SpaCy Lemmatizer:** 

SpaCy is a widely-used NLP library that provides a lemmatization tool. It uses rule-based methods and knowledge from large corpora to perform lemmatization. SpaCy's lemmatizer takes into consideration the word's POS and dependency relationships within the sentence to generate the lemma.

**TextBlob Lemmatizer:**

TextBlob is a Python library built on top of NLTK (Natural Language Toolkit). It offers various NLP functionalities, including a lemmatizer. TextBlob's lemmatizer utilizes WordNet's lemmatization capabilities and provides an easy-to-use interface for lemmatizing words.

**Gensim Lemmatizer:**

Gensim is a popular library primarily used for topic modeling and document similarity tasks. It also includes a lemmatizer module that can be utilized for lemmatizing words. Gensim's lemmatizer is based on the pattern package and provides lemmatization functionality.

**TreeTagger:**

TreeTagger is a linguistic tool that performs part-of-speech tagging, named entity recognition, and lemmatization. Developed by Helmut Schmid, it supports several languages and employs statistical methods for lemmatization based on hidden Markov models.

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/a02bd504-eb8b-4716-9878-3faa60cf48cf)

**Stemming Vs. Lemmatization:**

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/afbf5914-e5d8-44b0-9b72-1575f2095558)

# Vectorizer

**Feature transformation:** Transformation of data to improve the accuracy of the algorithm. Converting data into numerical format. Ex: One-hot Encoding, Label Encoder, etc.

**Feature selection:** Removing unnecessary features.

**Feature extraction:** The transformation of raw data into features suitable for modeling.

**Types of Vectorizer:**

▪ Bag of Words: Count Vectorizer
▪ TF-IDF Vectorizer
▪ Word2Vec
▪ Global Vectors for Word Representation
▪ BnVec (Bangla Feature Extractor)

**Count Vectorizer (Mathematical architecture):**

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/918b25d2-b7ac-4787-80dd-dc8e9d0eb5ad)

At first, we will separate the unique words. Then, we will create features with those unique words. Afterwards, we will count their presence or frequency (how many times they are there?) in each sentence. The counts of the words will be in the index number and the indexing will start from 0. 

This is bad bad. -> bad=2
This is bad. -> bad=1

It will count row wise. It will separate the sentence and row. There can be multiple lines in a single row. 

This does not always provide good result. 

**TF-IDF Vectorizer (Mathematical architecture):**

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/0e3c242f-1157-487b-b18d-7e8aca77822e)

TF - Term Frequency 
IDF - Inverse Document Frequency
TF-IDF Vectorizer -> TF * IDF

**TF** = How many times it is present? / Total Word
Ex: This is good and awesome. 
This: 1/5

**IDF**: 

This is good and awesome. 
This is bad.

How many times 'This' is present in the total data?
2 times.



**Differences (TF-IDF Vs. Count):**

▪ TF-IDF is better than Count Vectorizers because it not only focuses on the frequency of words present in the corpus but also provides the importance of the words. The term "df" is called document frequency which means in how many documents the word “subfield” is present within the corpus.

❑ Can TF IDF Be Negative?
❑ No. The lowest value is 0. Both term frequency and inverse document frequency are positive numbers.

▪ In AI inference and machine learning, sparsity refers to a matrix of numbers that includes many zeros or values that will not significantly impact a calculation.

**Word2Vec:**

Word2vec is a Neural Network that processes text by “vectorizing” words. Its input is a text corpus and its output is a set of vectors: feature vectors that represent words in that corpus. 

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/48f646b0-f4ac-427b-af58-d3f3d53de773)

**Global Vectors for Word Representation (GloVe):** 

GloVe is an algorithm for generating word embeddings, which are vector representations of words in a high-dimensional space. These embeddings capture semantic and syntactic relationships between words. GloVe utilizes global word co-occurrence statistics to learn word embeddings that encode meaningful relationships between words. It has been widely used in various NLP tasks, such as word similarity, document classification, and machine translation.

**BnVec (Bangla Feature Extractor):**

BnVec is a specialized feature extractor for the Bengali (Bangla) language. It is designed to generate word embeddings specifically for Bengali words. Similar to GloVe, BnVec creates vector representations that capture semantic information and relationships among Bengali words. These embeddings can be utilized in various NLP tasks specific to the Bengali language, such as text classification, sentiment analysis, or Bengali language understanding.
