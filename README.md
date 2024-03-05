Machine Learning Final Project: Sentence Similarity Detection and Evaluation

This README provides an overview of the final project, focusing on the development of a model for identifying sentence similarity and evaluating its performance using various metrics.

Project Overview

The objective of this project is to develop a robust model capable of determining the similarity between two sentences. The project involves feature extraction, data preprocessing, model selection, and evaluation using multiple metrics.

Features Description

The model considers a range of features to capture the structural aspects of sentences, including:

- Word Count Difference: Measures the difference in the number of words between sentences.
- Word Overlap: Counts the common words between sentences.
- Word Union: Determines the count of unique words in two sentences.
- n-Gram Overlap (2-Gram and 3-Gram): Calculates the overlap of n-grams between sentences.
- Numbers Overlap: Counts the occurrence of numbers in sentences.
- Capitalized Words Overlap: Identifies the occurrence of capitalized words in sentences.
- Cosine Similarity Score: Computes the cosine similarity score between sentences.
- BLEU (Bilingual Evaluation Understudy): Measures the similarity of machine-translated text to reference translations.
- NIST (Normalized Information Retrieval Metric): Calculates n-gram co-occurrence statistics.
- METEOR: Scores machine translation hypotheses by aligning them to reference translations.
- Levenshtein Distance: Measures the similarity between two strings by counting the number of deletions, insertions, or substitutions required to transform one string into another.

Data Preprocessing

Data preprocessing involved:

- Identifying bad lines: Handling formatting issues in the dataset.
- Working with sentences: Standardizing sentences by converting to lowercase, tokenizing, removing stopwords, and lemmatizing words.
	- StandardScaler(): Standardizing feature vectors for Multi-Layer Perceptron (MLP) model training.

Libraries Utilized

The project utilized various Python libraries:

- NLTK: Used for data preprocessing and feature extraction.
- Pandas: Employed for data manipulation and analysis.
- Sklearn: Utilized for model creation, feature scaling, and evaluation.
- Re: Used for regular expression operations.
- Math: Utilized for mathematical operations and matrix manipulations.
- Seaborn and Matplotlib: Employed for data visualization.
- Numpy: Used for parameter tuning in MLP.

Algorithms Tested

The project tested the Multi-Layer Perceptron (MLP) algorithm:

MLP - Multi-Layer Perceptron:
- Parameters tuned using GridSearchCV.
- Best parameters obtained for solver, alpha, hidden layer sizes, and random state.
- Logistic activation function yielded the best score.
- Achieved an F1 score of 0.87 on the dev set.

Experience and Lessons
Key insights and learnings from the project:

- Handling large datasets and understanding the importance of data preprocessing.
- Exploration of neural networks, transitioning from confusion to understanding with the help of sklearn's MLP implementation.
- Learning about new evaluation metrics such as NIST score and METEOR for sentence similarity assessment.
- The significance of feature selection and parameter tuning in model performance optimization.

This README provides an overview of the project, outlining its objectives, methodologies, and outcomes. For further details, refer to the project documentation and code implementation.
