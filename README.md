# Latent Semantic Analysis for Cross-Domain Research Paper Similarity

## Project Overview

This repository contains the complete source code and implementation for my MSc Advanced Computer Science dissertation titled **"Latent Semantic Analysis for Finding Similarity Between Words from Research Papers on the Same Topic from Different Domains"**. Conducted at the **University of Hertfordshire**, this research addresses a fundamental challenge in Information Retrieval (IR) and Natural Language Processing (NLP): accurately identifying semantic connections between academic texts that share conceptual ground but originate from distinct scientific disciplines.

## The Challenge & Solution

Traditional search algorithms often rely on exact keyword matching, which fails when different domains use disparate terminology to describe similar concepts (the vocabulary mismatch problem). To overcome this, this project implements **Latent Semantic Analysis (LSA)**, a mathematical technique that uncovers the hidden (latent) conceptual structure in unstructured text data. By moving beyond surface-level lexical matching, this system can detect deep semantic similarities between research papers regardless of domain-specific jargon.

## Technical Implementation

The solution is architected using **Python** and relies on a robust data science stack including **Scikit-learn**, **NLTK**, **NumPy**, and **Pandas**. The processing pipeline consists of four distinct stages:

1. **Advanced Preprocessing:** Raw text is ingested and subjected to rigorous cleaning pipelines. This involves tokenization, normalization, and the removal of stop-words using the **Natural Language Toolkit (NLTK)** to reduce noise and improve signal quality.
2. **Vectorization (TF-IDF):** Textual data is transformed into numerical vectors using **Term Frequency-Inverse Document Frequency (TF-IDF)**. This statistical weighting scheme highlights the most significant terms within documents while filtering out ubiquitous but uninformative words.
3. **Dimensionality Reduction (SVD):** The core LSA engine applies **Singular Value Decomposition (SVD)** to the high-dimensional TF-IDF matrix. This reduces the feature space, compressing the data to capture essential semantic relationships and effectively handling synonymy and polysemy.
4. **Semantic Similarity Metrics:** The system utilizes **Cosine Similarity** on the reduced vector space to compute precise similarity scores between documents, enabling the retrieval of conceptually related papers across disciplinary boundaries.

## Academic Context

This research was conducted under the supervision of Harpreet Singh and Dr. Na Helian as part of the **MSc in Advanced Computer Science** program, which I completed with **Distinction**.
