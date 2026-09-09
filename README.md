# 7AAVDH26 Final Project: Semantic Spaces in Breaking Bad

**Author:** AG18261
**Module:** 7AAVDH26 Advanced Computational Analysis for Digital Humanities, Cultural and Social Research

## Project Overview
This repository contains the code and dataset for a diachronic and character-based text analysis of the television series *Breaking Bad*. The project applies Distributional Semantics to explore how the core vocabulary of the illicit drug trade and interpersonal relationships structurally differs between the show's two protagonists: Walter White (middle-class chemist) and Jesse Pinkman (marginalized street youth). 

## Research Questions
1. **RQ1:** How do the semantic networks surrounding core trade terminology (e.g., "business", "cook") structurally differ in the linguistic spaces of Walter and Jesse? To what extent do these semantic shifts reflect their distinct class attributes and professional conceptualizations?
2. **RQ2:** Utilizing Orthogonal Procrustes alignment, what is the Euclidean distance of the concept of "money" between the two characters' embedding models? How does quantifying this divergence reveal their differing moral frameworks regarding survival versus the pursuit of absolute power?

## Methodology
The computational methodology strictly follows the techniques taught in the 7AAVDH26 module:
* **NLP Pipeline:** Tokenization, custom stopword removal, and lemmatization using `spaCy`.
* **Distributional Semantics:** Training independent `Word2Vec` neural word embedding models for each character using `gensim`.
* **Space Alignment:** Applying `scipy`'s Orthogonal Procrustes algorithm to align Jesse's semantic matrix to Walter's coordinate space for direct comparison.
* **Change Measurement & Visualization:** Calculating semantic shift magnitudes (Cosine Similarity) and Euclidean distances, followed by PCA dimensionality reduction to plot semantic trajectories.
