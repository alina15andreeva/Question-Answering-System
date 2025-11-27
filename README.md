# Question Answering System (RAG) - Kaggle Competition

This repository contains my solution notebook for the **Question-Answering System** Kaggle competition.  
The task follows a modern **Retrieval-Augmented Generation (RAG)** pipeline consisting of:

- **Retriever** — selects the most relevant passages for a question.  
- **Generator** — produces a natural-language answer using the retrieved passages.

The goal is to build an end-to-end system that retrieves relevant documents and generates accurate answers, evaluated jointly using Precision, Recall, and BLEU.

---

## Competition

- **Kaggle:** *Question-Answering System*  
- **Task:** Build a RAG-style pipeline to answer questions using a large collection of text passages.
- **Inputs:**  
  - **Questions**  
  - **Document pool** of passages  
- **Outputs:**  
  - `relevant_passage_ids` — retrieved passages (Retriever)  
  - `answer` — generated text (Generator)

---

## Evaluation

The final score is the **mean of three metrics**:

1. **Precision (Retriever)**  
   Measures how many retrieved passages were actually relevant.  

2. **Recall (Retriever)**  
   Measures how many relevant passages were successfully retrieved.  

3. **BLEU (Generator)**  
   Measures how close the generated answer is to the true answer.

**Final score = (Precision + Recall + BLEU) / 3**

---

## Repository Structure

```text
Question-Answering-System/
├── Question-Answering System Kaggle.ipynb          # Full system: retrieval, generation, tuning, evaluation, submission
└── README.md                                       # Project documentation (this file)
