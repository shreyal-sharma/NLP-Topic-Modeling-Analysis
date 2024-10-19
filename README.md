# NLP-Based Topic Analysis of Transcripts

This project employs Natural Language Processing (NLP) techniques to extract popular themes or topics from a dataset of participant-generated transcripts using unsupervised learning. The primary tool for topic modeling is Latent Dirichlet Allocation (LDA), combined with TF-IDF vectorization for effective text representation.

## Objectives

- Perform language detection to filter transcripts.
- Vectorize the transcripts using TF-IDF to capture term importance.
- Implement LDA for unsupervised topic modeling.
- Evaluate the model’s performance using perplexity and identify optimal topics.
- Present the top themes derived from the transcripts.

## Installation

To run this analysis, ensure you have Python installed on your machine. You will also need the following libraries:

```bash
pip install pandas langdetect scikit-learn matplotlib openpyxl
```

# Usage

## Data Preparation
- Ensure you have a dataset in Excel format (`master-file.xlsx`) with a column named `transcript` containing the text data to analyze.

## Language Detection
- The code detects the language of each transcript and filters for English transcripts.

## TF-IDF Vectorization
- Transcripts are converted into a document-term matrix using TF-IDF, highlighting the importance of words.

## Topic Modeling with LDA
- The LDA model is applied to the document-term matrix to extract a specified number of topics.
- The code displays the distribution of topics across the documents and identifies the most relevant words for each topic.

## Perplexity Analysis
- The model’s performance is evaluated through perplexity, which helps determine the optimal number of topics.
