# MULTIMODAL_RAG
This is a multimodal RAG using CLIP model for embeddings form Hugging Face. To generate the context OPEN AI is used. 

CLIP Embeddings for Multimodal- https://huggingface.co/docs/transformers/en/model_doc/clip

ChatGPT 4.1 for answer generation.

Text extraction from pdf using FITZ

FAISS as vectorstore

**System Architecture**

<img width="1591" height="710" alt="image" src="https://github.com/user-attachments/assets/2ece88d5-c99b-4e2e-8c94-53dfa8eaf4f5" />

**Input pdf**- Comparsion of few shot learning models

<img width="920" height="808" alt="image" src="https://github.com/user-attachments/assets/03b5c1f9-cf6b-4cb6-ba20-38685063170c" />


**Output**

Query: Which is the worst performing model from the graph?
--------------------------------------------------

Retrieved 1 documents:
  - Image from page 0


Answer: The **worst performing model** from the graph is **ResNet50** (the green curve). It consistently has the lowest average score (%) across all numbers of labeled training examples per class compared to the other named models (Linear Probe CLIP, BiT-M (ImageNet-21K), and SimCLRv2).
======================================================================

Query: What is the average score for Linear Probe CLIP model when the number of labeled training examples per class is 8?
--------------------------------------------------

Retrieved 1 documents:
  - Image from page 0


Answer: When the number of labeled training examples per class is **8**, the **average score for the Linear Probe CLIP model** is approximately **68%** (as read from the purple line at the mark corresponding to 8 on the x-axis).
======================================================================
