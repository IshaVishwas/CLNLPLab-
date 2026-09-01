# Experiment 2: Basic Text Preprocessing

**Name:** Isha  
**SAP ID:** 500119683  

## Objective

To implement foundational text preprocessing techniques essential for Natural Language Processing by transforming raw textual data into structured tokens while removing noise.

## Procedure & Implementation

The experiment operates on raw text files and is divided into three core preprocessing stages, using built-in Python string operations, NLTK, and spaCy libraries.

1. **Text Cleaning (`2.1_text_data.txt`):**
   * Reading the raw text file using `open(file, 'r').read()`.
   * Calculating the frequency of uppercase characters using `isupper()`.
   * Converting the entire text corpus to lowercase using `str.lower()` for uniformity.
   * Identifying and removing punctuation marks using the `string.punctuation` module.
   * Identifying and removing numeric digits using `str.isdigit()`.
   * Normalizing whitespace by splitting and rejoining the text using `" ".join(str.split())`.

2. **Tokenization (`2.2_tokenization_data.txt`):**
   * **NLTK:** Using `nltk.word_tokenize` and `nltk.sent_tokenize` for word-level and sentence-level tokenization.
   * **spaCy:** Loading the `en_core_web_sm` model using `spacy.load()` to process the text and extract word and sentence tokens through the document object.
   * **Python Native:** Performing basic word tokenization using the `split()` method and sentence tokenization using regular expressions with `re.split()`.

3. **Stop Word Removal (`2.3_clean_data.txt`):**
   * Importing the English stop words list from `nltk.corpus`.
   * Converting the stop words list into a set using `set(stopwords.words('english'))`.
   * Tokenizing the lowercase input text using NLTK.
   * Filtering the tokens to remove words present in the stop words set.
   * Using `str.isalnum()` to ensure that punctuation tokens are excluded.
   * Displaying the stop words identified in the input corpus.

## Observations

| Preprocessing Stage | Method / Library | Action Performed | Result Output |
| :--- | :--- | :--- | :--- |
| **Text Cleaning** | Built-in Python (`string`) | Lowercasing, punctuation and digit removal | Normalized, cleaned text |
| **Whitespace Normalization** | Built-in Python (`split`, `join`) | Removal of redundant spaces | Normalized text corpus |
| **Tokenization (NLTK)** | `nltk.word_tokenize`, `sent_tokenize` | Word and sentence tokenization | Lists of words and sentences |
| **Tokenization (spaCy)** | `en_core_web_sm` model | Model-based text processing | Extracted word and sentence tokens |
| **Tokenization (Native)** | `str.split()`, `re.split()` | Whitespace and regex-based tokenization | Basic word and sentence token lists |
| **Stop Word Removal** | `nltk.corpus.stopwords` | Filtering common English stop words | Filtered alphanumeric tokens |

## Result Interpretation & Learnings

* **Pipeline Foundation:** The experiment demonstrates the fundamental preprocessing stages required before performing further Natural Language Processing tasks.
* **Effective Normalization:** The text cleaning stage normalizes raw text by converting it to lowercase and removing punctuation, digits, and unnecessary whitespace.
* **Tokenizer Comparison:** The tokenization stage demonstrates the differences between NLTK, spaCy, and basic Python-based tokenization approaches.
* **Dimensionality Reduction:** Removing stop words reduces the number of unnecessary tokens in the text corpus.
* **Clean Text Representation:** After preprocessing, the resulting tokens are cleaner and more suitable for further NLP tasks.
