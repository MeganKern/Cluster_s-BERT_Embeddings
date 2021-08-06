# Cluster_BERT_Embeddings

Final Product:

Paper abstract -> Sentence Embedding ->  Category ---- rewrite in sentences


Abstracts scraped from arXiv. Dataset balenced by removeing abstracts in overrepresented category tags. A modified version of BERT called sentence-BERT created by Nils Reimers and Iryna Gurevych is finetuned. The model parameters are imported with hugging Face's transformers library and fine-tuned useing PyTorch Lightining. Finialy K-Means clustering attempts to reproduce the origional abstract category partition.
