# NLP (Natural Language Processing)

# Feature Extraction

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/ed71dc6b-2ae0-48b3-ab0f-d5fa97b02e7b)

# Text Processing in NLP

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/c30ded4d-9c85-410d-a458-fc113fba74f5)

**Type of Tokens:**

1. Word tokens
2. Character tokens
3. Sentence tokens
4. Named entity tokens
5. Part-of-speech (POS) tags
6. Sub-word tokens

# Text Preprocessing

Stemming and Lemmatization are Text Normalization (or sometimes called Word Normalization) techniques in the field of Natural Language Processing that are used to prepare text, words, and documents for further processing. Stemming and Lemmatization have been studied, and algorithms have been developed in Computer Science since the 1960s. We will learn about Stemming and Lemmatization in a practical approach covering the background, some famous algorithms, applications of Stemming and Lemmatization, and how to stem and lemmatize words, sentences, and documents using the Python nltk package which is the Natural Language Tool Kit package provided by Python for Natural Language Processing tasks.

**Stemming:**

Stemming is the process of reducing a word to its word stem that affixes to suffixes and prefixes or to the roots of words known as a lemma. Stemming is important in natural language understanding (NLU) and natural language processing (NLP). When a new word is found, it can present new research opportunities. For example -

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/110ab908-30b0-4fa5-aa21-806a4308883a)

▪ Porter Stemmer(): The Porter stemming algorithm (or 'Porter stemmer’) removes the commoner morphological endings from words in English.
▪ Lovins Stemmer
▪ Dawson Stemmer
▪ Krovetz Stemmer
▪ Xerox Stemmer
▪ N-Gram Stemmer
▪ Snowball Stemmer
▪ Lancaster Stemmer

**Lemmatization:**

Lemmatization usually refers to doing things properly with the use of a vocabulary and morphological analysis of words, normally aiming to remove inflectional endings only and to return the base or dictionary form of a word, which is known as the lemma.

▪ Word Net Lemmatizer
▪ Spacy Lemmatizer
▪ TextBlob
▪ Gensim Lemmatizer
▪ TreeTagger

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/a02bd504-eb8b-4716-9878-3faa60cf48cf)

**Stemming Vs. Lemmatization:**

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/afbf5914-e5d8-44b0-9b72-1575f2095558)

# Vectorizer

Feature transformation: Transformation of data to improve the accuracy of the algorithm.
Feature selection: Removing unnecessary features.
Feature extraction: The transformation of raw data into features suitable for modeling.

**Types of Vectorizer:**

▪ Bag of Words: Count Vectorizer
▪ TF-IDF Vectorizer
▪ Word2Vec
▪ Global Vectors for Word Representation

**Count Vectorizer (Mathematical architecture):**

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/918b25d2-b7ac-4787-80dd-dc8e9d0eb5ad)

**TF-IDF Vectorizer (Mathematical architecture):**

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/0e3c242f-1157-487b-b18d-7e8aca77822e)

**Differences (TF-IDF Vs. Count):**

▪ TF-IDF is better than Count Vectorizers because it not only focuses on the frequency of words present in the corpus but also provides the importance of the words. The term "df" is called document frequency which means in how many documents the word “subfield” is present within the corpus.

❑ Can TF IDF Be Negative?
❑ No. The lowest value is 0. Both term frequency and inverse document frequency are positive numbers.

▪ In AI inference and machine learning, sparsity refers to a matrix of numbers that includes many zeros or values that will not significantly impact a calculation.

**Word2Vec:**

Word2vec is a Neural Network that processes text by “vectorizing” words. Its input is a text corpus and its output is a set of vectors: feature vectors that represent words in that corpus. 

![image](https://github.com/TITHI-KHAN/NLP/assets/65033964/48f646b0-f4ac-427b-af58-d3f3d53de773)
