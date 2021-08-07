# Cluster_BERT_Embeddings

To cluster papers in Physics by subfield each paper is embedded in a sentence vector, then all are clustered by K-means.  

Abstracts scraped from arXiv. Dataset balanced by removing abstracts in over represented categories. A modified version of BERT called sentence-BERT created by Nils Reimers and Iryna Gurevych is fine-tuned. The model parameters are imported with Hugging Face's transformers library and fine-tuned using PyTorch Lightning. Finally, K-Means clustering attempts to reproduce the original category partitions.

The Adjusted Rand Index compares the similarity of two clusterings. A score of 43 was reached. To increase performance, the clustering algorithm could be directly integrated into the objective function of the embedding model. This way the model learns to represent papers in a structure more amenable to the clustering algorithm.
