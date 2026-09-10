# **AG18261 - 7AAVDH26 - Semantic Spaces in Breaking Bad**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WGShhxDVzdUTqFe7ZMo6xALNJq8DlEvO#scrollTo=0v8bSbX4BhQN)

## **Project Overview**

This project applies Distributional Semantics to television transcripts to examine the socio-linguistic divergence between Breaking Bad’s two protagonists: Walter White and Jesse Pinkman. By computationally modeling their dialogue, the study investigates how distinct class backgrounds shape their conceptualizations of the drug trade and capital.

### **Research Questions**
1. How do the semantic networks of core occupational terms (e.g., "business", "cook") differ between Walter and Jesse, and to what extent do these structural shifts reflect their distinct class identities?
2. Using Orthogonal Procrustes alignment, what is the semantic distance of the concept of "money" between the two characters' embedding models, and how do their semantic neighborhoods reveal contrasting moral motivations?

### **Methodology**
The computational pipeline adapts techniques from the 7AAVDH26 module. Raw dialogue was pre-processed and lemmatized using spaCy, followed by the training of independent Word2Vec models. To accommodate small-scale spoken dialogue, hyperparameters were manually tuned. The two semantic spaces were then mapped into a shared coordinate system using Orthogonal Procrustes alignment, with trajectories and neighborhoods visualized via PCA (assisted by the adjustText library to resolve label overlap).

## **Data Source**
Breaking Bad Script directly scrapped from Forever Dreaming. The data has about 5596 dialogs (observations) in total with 5 variables which are: - actor - text (which is the dialog itself) - season - episode - title of the episode.

**Link:** https://www.kaggle.com/datasets/mexwell/breakingbad-script

**Important information:** If you are a fan then you would know that the series has a total of 5 seasons. Unfortunately, the transcripts data available online has labels attached to each dialog until episode 6 of season 3.
