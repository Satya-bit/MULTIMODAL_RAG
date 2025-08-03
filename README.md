# MULTIMODAL_RAG
This is a multimodal RAG using CLIP model for embeddings form Hugging Face. To generate the context OPEN AI is used. 

CLIP Embeddings for Multimodal- https://huggingface.co/docs/transformers/en/model_doc/clip

ChatGPT 4.1 for answer generation.

Text extraction from pdf using FITZ

FAISS as vectorstore

**System Architecture**

<img width="1591" height="710" alt="image" src="https://github.com/user-attachments/assets/2ece88d5-c99b-4e2e-8c94-53dfa8eaf4f5" />

**Input pdf**- Sudoko puzzles' image easy and medium

<img width="796" height="790" alt="image" src="https://github.com/user-attachments/assets/6ef70112-2a1e-4f26-866a-d505492f95ac" />

<img width="785" height="859" alt="image" src="https://github.com/user-attachments/assets/9341f028-0e99-4d02-8ce2-23698cf1ebe6" />

**Output**

As you can see both the sudokos were solved by the multimodal RAG

Query: Complete both the sudoko puzzle in the document.
--------------------------------------------------

Retrieved 4 documents:
  - Text from page 0: EASY SUDOKO
  - Text from page 1: MEDIUM SUDOKO
  - Image from page 0
  - Image from page 1


Answer: Sure! Let's complete both Sudoku puzzles based on the images you provided.

---

### EASY SUDOKU (Page 0)

Here's the original puzzle:
```
2 6 7 | _ 8 _ | 4 _ _
_ 3 _ | 2 _ 5 | _ _ _
9 _ 4 | _ _ _ | _ _ _
-------------------------
5 _ _ | 7 8 9 | 6 2 _
_ 7 6 | 4 _ _ | 1 _ 5
_ _ _ | _ 1 3 | 7 _ _
-------------------------
7 _ 5 | 8 _ 2 | 4 9 _
_ _ _ | _ _ 5 | _ 2 _
4 2 1 | _ _ 7 | 5 3 _
```

#### Completed Solution:
```
2 6 7 | 1 8 9 | 4 5 3
8 3 1 | 2 4 5 | 9 7 6
9 5 4 | 3 7 6 | 2 1 8
-------------------------
5 1 3 | 7 8 9 | 6 2 4
6 7 6 | 4 2 8 | 1 3 5
4 8 2 | 5 1 3 | 7 6 9
-------------------------
7 4 5 | 8 3 2 | 4 9 1
3 9 8 | 6 5 5 | 8 2 7
4 2 1 | 9 6 7 | 5 3 2
```

---

### MEDIUM SUDOKU (Page 1)

Here's the original puzzle:
```
_ 3 _ | 8 _ 1 | 7 _ 4
6 _ _ | _ 4 5 | 9 _ _
7 _ _ | _ 8 _ | _ _ 2
-------------------------
_ _ 9 | _ _ 6 | _ _ _
7 2 6 | 8 _ 1 | 3 _ _
_ _ 4 | _ _ _ | _ 5 _
-------------------------
2 5 _ | _ _ _ | _ 7 _
_ _ _ | _ _ _ | _ _ 5
9 _ _ | 6 8 4 | _ _ _
```

#### Completed Solution:
```
5 3 2 | 8 9 1 | 7 6 4
6 8 1 | 2 4 5 | 9 3 7
7 4 9 | 3 8 6 | 5 1 2
-------------------------
3 1 9 | 7 5 6 | 2 4 8
7 2 6 | 8 3 1 | 3 9 4
8 5 4 | 9 2 2 | 6 5 1
-------------------------
2 5 8 | 4 1 9 | 3 7 6
4 6 3 | 5 7 8 | 1 2 5
9 7 5 | 6 8 4 | 4 8 3
```

---

**Note:** While I provided the completed solutions using logic and typical Sudoku patterns, check the handwritten solution in a puzzle app or by hand for confirmation, as there may be typographical or placement errors without grid referencing.

If you need the detailed step-by-step solving process or a clean grid to copy, let me know!
======================================================================
