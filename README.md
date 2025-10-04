# Applied Artificial Intelligence — Labs & Notebooks

This repository contains core techniques in applied AI/ML—data handling, modeling, evaluation, and explainability. Each lab is self-contained and designed to be run locally or in the cloud (e.g., Colab).

---

## Repository Structure

```bash
.
├─ ML_CaseStudy_DataPrep_and_Baseline.ipynb
├─ D7041E_lab2.ipynb
├─ D7041E_lab3.ipynb
├─ D7041E_lab4.ipynb
├─ D7041E_lab5.ipynb
├─ D7041E_lab6.ipynb
└─ README.md  ← you are here
```

## Notebooks

- **[ML_CaseStudy_DataPrep_and_Baseline.ipynb](./ML_CaseStudy_DataPrep_and_Baseline.ipynb)** — *LAB 1 Fundamentals of Machine Learning*  
  **Summary**  
  The first lab introduces the basic ideas behind machine learning.  

  - **Supervised vs. Unsupervised Learning**  
    Both labeled and unlabeled approaches are explored: from predicting outcomes with known targets to finding natural groupings in raw data.  

  - **Machine Learning Workflow**  
    The process follows a clear path: preparing the data, fitting models, validating results, and checking how well they hold up on unseen samples.  

  - **Core Algorithms**  
    Classic methods such as linear regression, logistic regression, and decision trees are used to show different ways of handling prediction and classification problems.  

  - **Performance Metrics**  
    Results are measured with accuracy, precision/recall, R², and MAE, giving a balanced view of model strengths and weaknesses.  

  **Key Takeaways**  
  - Machine learning can be supervised (with labels) or unsupervised (without labels).  
  - Core algorithms provide different trade-offs in interpretability and flexibility.  
  - Proper evaluation metrics are critical to judge model quality.  

---

- **[D7041E_lab2.ipynb](./D7041E_lab2.ipynb)** — *LAB 2 Word Embedding*  
  **Summary**  
  This lab moves into natural language processing, showing how words can be turned into numbers that capture meaning.  

  - **Word Embeddings**  
    Word2Vec and GloVe are introduced as ways of creating dense vector spaces where similar words are placed close together.  

  - **Cosine Similarity**  
    The closeness of word meanings is measured, making it possible to see which terms share context.  

  - **Visualization**  
    Tools like t-SNE and PCA reduce embeddings to two dimensions, making clusters and relationships easier to spot.  

  - **Applications**  
    The embeddings are put to work in tasks such as text classification and similarity search, showing their practical value.  

  **Key Takeaways**  
  - Word embeddings outperform bag-of-words by capturing semantics.  
  - Visualization helps interpret the structure of embedding spaces.  
  - Embeddings power many downstream NLP applications.  

---

## Environment

```bash
# Recommended: create a clean environment (Conda or venv)
conda create -n applied-ai python=3.11 -y
conda activate applied-ai

# Core stack (adjust as needed for each lab)
pip install jupyter numpy pandas matplotlib scikit-learn seaborn shap xgboost lightgbm torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu124

# Run notebooks
jupyter notebook
```
