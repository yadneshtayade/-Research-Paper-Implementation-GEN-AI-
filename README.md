# Adaptive-RAG: Question Complexity-Based Retrieval-Augmented Generation

This project presents a simplified implementation of **Adaptive-RAG**, based on the research paper *“Adaptive-RAG: Learning to Adapt Retrieval-Augmented Large Language Models through Question Complexity”* published at NAACL 2024.

Adaptive-RAG is a Retrieval-Augmented Generation (RAG) approach that selects an appropriate question-answering strategy according to the complexity of the input query. Instead of applying the same retrieval method to every question, it uses three different strategies:

- **No Retrieval (A):** Answers simple questions directly using the language model.
- **Single-Step Retrieval (B):** Retrieves relevant information once for moderately complex questions.
- **Multi-Step Retrieval (C):** Performs iterative retrieval for complex questions requiring information from multiple sources.

The project was implemented using Python and Google Colab. It demonstrates the adaptive routing mechanism, evaluates question-complexity classification, and visualizes strategy distribution and execution-time comparisons.

The experimental output includes a routing accuracy of 40% on a small test set of five questions. The results highlight the basic working principle of adaptive retrieval while identifying areas for improvement.

**Technologies Used:** Python, Google Colab, Pandas, NumPy, Matplotlib, and Scikit-learn.

**Future Improvements:** Larger datasets, a trained complexity classifier, advanced document retrieval, improved answer evaluation, and real-time performance analysis.

**Research Paper:** https://aclanthology.org/2024.naacl-long.389/
