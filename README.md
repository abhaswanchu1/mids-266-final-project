**Privacy Policy Understanding with NLP Techniques**

This repository contains the work for a natural language processing (NLP) project focused on enhancing the accessibility and interpretability of privacy policies. We tackle two distinct but related tasks: binary sentence classification to identify relevant privacy statements and span detection question answering (QA) to extract precise answers from policy texts.

Project Overview
Privacy policies are often lengthy and complex, making it challenging for users to understand how their data is collected, used, and shared. This project aims to bridge this gap by developing and evaluating machine learning models that can automatically process and interpret these documents.

We investigate the effectiveness of various traditional and state-of-the-art deep learning models, including domain-specific language models and large language models (LLMs) in few-shot settings, on two key tasks:

PrivacyQA (Binary Sentence Classification): Determining whether a given sentence from a privacy policy is "Relevant" or "Irrelevant" to a specific query or context. This task is particularly challenging due to significant class imbalance.

PolicyQA (Span Detection Question Answering): Extracting the exact textual span from a privacy policy that directly answers a given question. This requires precise understanding and boundary detection.

Datasets
The project utilizes two prominent datasets in the privacy NLP domain:

PrivacyQA: A dataset for binary sentence classification, where sentences are labeled as relevant or irrelevant to a query. This dataset is known for its class imbalance, with a majority of "Irrelevant" labels.

PolicyQA: A dataset for extractive question answering, where models must identify precise answer spans within privacy policy documents.

Models Evaluated
We evaluated a range of models to assess their performance across these tasks:

Traditional Baselines:

TF-IDF + Logistic Regression: A classic machine learning approach using TF-IDF features for classification.

Simple Embedding (Bag-of-Words + Linear SVC): Another traditional baseline leveraging Bag-of-Words embeddings with a Linear Support Vector Classifier.

Pre-trained Transformer Models:

BERT (not fine-tuned): A base BERT model to establish a baseline for transformer performance without task-specific fine-tuning.

legal-bert-small-uncased: A smaller BERT variant pre-trained specifically on legal texts, designed to capture domain-specific nuances.

roberta-large: A large, robustly optimized BERT model known for its strong general language understanding capabilities.

Large Language Model (LLM):

gpt-4.1-nano: A lightweight LLM evaluated in a few-shot learning setting to assess its zero/few-shot capabilities on these tasks.
Repository Structure


Contributors
[Abhas Wanchu]

Credit for PLU dataset: https://github.com/JFChi/PLUE.git
