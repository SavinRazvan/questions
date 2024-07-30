# Questions AI Project

## Project Description

The "Questions" project is part of Harvard's CS50 AI course. It focuses on developing an AI system capable of answering questions by performing document retrieval and passage retrieval from a text corpus. The AI utilizes term frequency-inverse document frequency (tf-idf) to identify relevant documents and passages in response to user queries. This project helps in understanding the implementation of natural language processing (NLP) and information retrieval techniques.

## Project Goal

The primary goal of this project is to implement a question-answering system that efficiently identifies and returns the most relevant passages from a set of documents. The system aims to enhance understanding of NLP and information retrieval techniques by leveraging tf-idf scoring.

## Implementation

The project is implemented in Python using the NLTK library. The main steps include:

1. **Loading Files**: Load all text files from a specified directory.
2. **Tokenization**: Convert documents into a list of words, filtering out punctuation and stopwords.
3. **Computing IDFs**: Calculate Inverse Document Frequency (IDF) values for each word in the corpus.
4. **Query Processing**: Tokenize and process user queries.
5. **Document Scoring**: Score documents based on tf-idf and identify top matches.
6. **Sentence Extraction and Scoring**: Extract sentences from top documents and score them based on query relevance.

## How to Use

1. **Setup Environment**: Ensure you have Python and NLTK installed. Download necessary NLTK data.
    ```sh
    pip install nltk
    ```

    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    ```

2. **Prepare Corpus**: Place your text files in a directory (e.g., `corpus`).

3. **Run the Project**: Call the `main` function with the corpus directory and queries.
    ```python
    path_to_corpus_directory = 'corpus'
    queries = [
        "What are the types of supervised learning?",
        "How do neurons connect in a neural network?",
        "When was Python 3.0 released?"
    ]
    main(path_to_corpus_directory, queries)
    ```

## Example Queries

- "What are the types of supervised learning?"
- "How do neurons connect in a neural network?"
- "When was Python 3.0 released?"

## Output

For each query, the system prints the most relevant answer along with the source document.

## More Information

For more details on the project, please visit the [CS50 AI Project page](https://cs50.harvard.edu/ai/2020/projects/6/questions/).

