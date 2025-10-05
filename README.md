# Applied Artificial Intelligence — Notebooks 

This repository contains core techniques in applied AI/ML — data handling, modeling, evaluation, and explainability.

---

## Repository Structure

```bash
.
├─ DataPrep_and_Baseline_Modeling_Iris.ipynb
├─ HighDimensional_Embeddings_CaseStudy.ipynb
├─ LanguageIdentification_HyperdimensionalVectors.ipynb
├─ D7041E_lab4.ipynb
├─ D7041E_lab5.ipynb
├─ D7041E_lab6.ipynb
└─ README.md  ← you are here
```

---

## Notebooks

### [DataPrep_and_Baseline_Modeling_Iris.ipynb](./DataPrep_and_Baseline_Modeling_Iris.ipynb)

**Summary**

- **Supervised vs. Unsupervised Learning**  
  Both labeled and unlabeled approaches are explored: from predicting outcomes with known targets to finding natural groupings in raw data.  

- **Machine Learning Workflow**  
  The process follows path: preparing the data, fitting models, validating results, and checking how well they hold up on unseen samples.  

- **Core Algorithms**  
  Using classic methods such as linear regression, logistic regression, and decision trees to show different ways of handling prediction and classification problems.  

- **Performance Metrics**  
  Results are measured with accuracy, precision/recall, R², and MAE, giving a balanced view of model strengths and weaknesses.  

**Key Takeaways**
- Core algorithms provide different trade-offs in interpretability and flexibility.  
- Proper evaluation metrics are critical to judge model quality.  

---

### [HighDimensional_Embeddings_CaseStudy.ipynb](./HighDimensional_Embeddings_CaseStudy.ipynb) — *Word Embedding*

**Summary**

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

### [LanguageIdentification_HyperdimensionalVectors.ipynb](./LanguageIdentification_HyperdimensionalVectors.ipynb) — *Hyperdimensional Computing*

**Summary**

- **Objective**  
  This experiment applies **hyperdimensional computing** to **language identification**.  

- **Approach**  
  Sentences from 20 European languages are encoded as **10 000-dimensional bipolar vectors**, and each language’s average vector forms a unique centroid fingerprint.  

- **Classification**  
  New sentences are compared against all centroids using **cosine similarity** to predict which language they belong to.  

- **Performance**  
  The model reaches about **76.8 % accuracy**, showing that simple high-dimensional representations can effectively distinguish languages without deep learning.  

**Key Takeaways**  
- High-dimensional vectors capture subtle structural differences between languages.  
- Cosine similarity provides a lightweight yet effective decision rule.  
- Hyperdimensional methods demonstrate how symbolic and statistical ideas meet in modern AI.  

### [UnsupervisedLearning_SelfOrganizingMaps.ipynb](./UnsupervisedLearning_SelfOrganizingMaps.ipynb) — *Self-Organizing Maps (SOMs)*  

**Summary**  

- **Objective**  
  This lab introduces **Self-Organizing Maps (SOMs)** — an **unsupervised neural network** model that projects high-dimensional data into a **two-dimensional grid**, preserving the topology of input relationships.  

- **Datasets**  
  Two datasets are explored:  
  - **Zoo (UCI dataset)** — categorical animal features (17 attributes, 7 classes).  
    This dataset serves as a conceptual starting point to show how SOMs cluster structured data.  
    Animals with similar traits — such as mammals, birds, or fish — naturally form neighboring clusters on the SOM grid, demonstrating **topological preservation**: similar inputs end up near each other on the map.  
  - **MNIST (handwritten digits)** — 28×28 grayscale images, used to extend SOMs to image data and visualize how digits self-organize into distinct clusters.  

- **Approach**  
  The SOM learns through competitive learning, adjusting neighboring neuron weights to reflect input similarity.  
  Different grid sizes (20×20, 40×40, 80×80) are tested to study the effect of network resolution on clustering quality.  

- **Results**  
  | Grid Size | Train Accuracy | Test Accuracy |
  |:-----------:|:---------------:|:--------------:|
  | 20×20 | 72.0 % | 78.0 % |
  | 40×40 | 96.0 % | 94.0 % |
  | 80×80 | 98.0 % | ------ |

  Larger grids captured finer feature variations, improving the model’s ability to organize and separate clusters.  

**Key Takeaways**  
- The Zoo dataset illustrates how SOMs group similar entities through feature-based proximity.  
- The MNIST dataset demonstrates how the same principle scales to complex, high-dimensional image data.  
- SOMs reveal structure in unlabeled data, providing both visualization and clustering in one interpretable framework.  
