# Candidate-selection-with-PNL
Candidate selection using machine learning models with natural language processing and Power BI

# Resume Keyword Extractor

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![NLTK](https://img.shields.io/badge/NLTK-3.5%2B-brightgreen)

## Overview

This Python project aims to streamline the candidate selection process by utilizing natural language processing (NLP) and machine learning techniques to extract keywords from candidate resumes. The extracted keywords are ranked using the TF-IDF (Term Frequency-Inverse Document Frequency) algorithm to create a tag cloud, making it easier for recruiters to identify the most relevant candidates for a specific job opening.

## TF-IDF Algorithm

The TF-IDF algorithm is a crucial component of this project. It works as follows:

1. **Term Frequency (TF)**: It measures the frequency of a term (word) within a document (resume). It is calculated as the number of times a term appears in a document divided by the total number of terms in that document.

2. **Inverse Document Frequency (IDF)**: It measures how unique or rare a term is across all documents in the corpus (collection of resumes). It is calculated as the logarithm of the total number of documents divided by the number of documents containing the term.

3. **TF-IDF Score**: The TF-IDF score of a term in a document is calculated by multiplying its TF and IDF values. It represents the importance of a term in a specific document relative to the entire corpus.

## NLTK (Natural Language Toolkit)

This project utilizes the NLTK library, a powerful NLP library in Python, for the extraction of keywords from resumes. Here's how it works:

1. **Tokenization**: NLTK is used to tokenize the text in each resume, breaking it down into words and punctuation.

2. **Stopword Removal**: Common stopwords (e.g., "and," "the," "in") are removed from the tokenized text to focus on meaningful keywords.

3. **Stemming/Lemmatization**: NLTK provides tools for stemming (reducing words to their base form) or lemmatization (reducing words to their dictionary form) to further refine the keywords.

4. **TF-IDF Calculation**: NLTK is used in conjunction with other Python libraries to calculate the TF-IDF scores for each keyword in each resume.

## Project Structure

The project consists of the following files:

- `resume_keyword_extractor.ipynb`: A Jupyter Notebook containing the Python script for extracting keywords from resumes and creating the tag cloud using the TF-IDF algorithm.
- `power_bi_report.pbix`: A Power BI report for visualizing the extracted keywords and tag cloud.
- `sample_resumes/`: A folder containing sample resumes for testing and demonstration purposes.

## Getting Started

To get started with this project, follow these steps:

1. Clone this repository to your local machine.

2. Open the `resume_keyword_extractor.ipynb` Jupyter Notebook and run the cells to extract keywords and create the tag cloud.

3. Use the `power_bi_report.pbix` file to visualize the results and make data-driven decisions during the candidate selection process.

## Dependencies

- Python 3.7+
- NLTK 3.5+
- Other Python libraries as listed in the Jupyter Notebook.

## Acknowledgments

This project was inspired by the need to simplify the candidate selection process for recruiters. We thank the open-source community for their contributions to NLTK and other NLP libraries.

Feel free to contribute, report issues, or provide feedback to enhance this project further.

Happy recruiting!
