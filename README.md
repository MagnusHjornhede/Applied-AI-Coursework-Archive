This repository contains coursework and experiments from my Master's studies in Applied Artificial Intelligence at Luleå University of Technology.

Topics explored include:

- machine learning algorithms
- data analysis
- computer vision
- neural networks

  

# Applied Artificial Intelligence — Notebooks

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Python](https://img.shields.io/badge/Python-3.11-blue)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-orange)
![Status](https://img.shields.io/badge/Status-Active-success)

A collection of **AI/ML notebooks** working with the fundamentals of applied artificial intelligence —  
covering **data handling, modeling, evaluation, visualization, and explainability**.

---

## Notebooks Overview

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

---

### [UnsupervisedLearning_SelfOrganizingMaps.ipynb](./UnsupervisedLearning_SelfOrganizingMaps.ipynb)

**Summary**  

- **Objective**  
  **Self-Organizing Maps (SOMs)** — an **unsupervised neural network** model that projects high-dimensional data into a **two-dimensional grid**, preserving the topology of input relationships.  

- **Datasets**  
  Two datasets are explored:  
  - **Zoo (UCI dataset)** — categorical animal features (17 attributes, 7 classes).  
    This dataset serves as a conceptual starting point to show how SOMs cluster structured data.  
    Animals with similar traits — such as mammals, birds, or fish — naturally form neighboring clusters on the SOM grid, demonstrating **topological preservation**.  
  - **MNIST (handwritten digits)** — 28×28 grayscale images, used to extend SOMs to image data and visualize how digits self-organize into distinct clusters.  

- **Approach**  
  The SOM learns through competitive learning, adjusting neighboring neuron weights to reflect input similarity.  
  Different grid sizes (20×20, 40×40, 80×80) are tested to study the effect of network resolution on clustering quality.  

- **Results**  

  | Grid Size | Train Accuracy | Test Accuracy |
  |:-----------:|:---------------:|:--------------:|
  | 20×20 | 72.0 % | 78.0 % |
  | 40×40 | 96.0 % | 94.0 % |
  | 80×80 | 98.0 % | — |

  Larger grids captured finer feature variations, improving the model’s ability to organize and separate clusters.  

**Key Takeaways**  
- The Zoo dataset illustrates how SOMs group similar entities through feature-based proximity.  
- The MNIST dataset demonstrates how the same principle scales to complex, high-dimensional image data.  
- SOMs reveal structure in unlabeled data, providing both visualization and clustering in one interpretable framework.  

---

### [NeuralNetwork_Backpropagation_MNIST.ipynb](./NeuralNetwork_Backpropagation_MNIST.ipynb) — *Artificial Neural Networks (ANNs) and Backpropagation*  

**Summary**  

- **Objective**  
   **Fully connected feed-forward neural network** learning through **backpropagation** to classify handwritten digits from the **MNIST dataset**.  

- **Dataset**  
  - **MNIST** — 60 000 training and 10 000 test samples of 28×28 grayscale digits (0–9).  
  - Each image is flattened into 784 inputs; labels represent the digit classes.  

- **Approach**  
  - Implemented a three-layer ANN (784-100-100-10).  
  - Compared different **learning rates** and activation functions (Sigmoid vs ReLU).  
  - Training performed for 70 epochs using gradient descent and error backpropagation.  
  - Performance tracked through training / test error per epoch.  

- **Results**  
  - Initial error ≈ 0.90 → final ≈ 0.02.  
  - Corresponds to about **97–98 % classification accuracy** on MNIST test data.  
  - Lower learning rates improved stability; ReLU accelerated convergence.  

**Key Takeaways**  
- Backpropagation enables neural networks to learn complex nonlinear mappings by propagating errors backward.  
- Learning rate selection balances speed and stability.  
- Even a simple fully connected ANN achieves near-state-of-the-art accuracy on MNIST without convolutional layers.  

---

### [RecurrentNeuralNetworks_SentimentAnalysis.ipynb](./RecurrentNeuralNetworks_SentimentAnalysis.ipynb)

**Summary**  

- **Objective**  
  **Recurrent Neural Networks (RNNs)** used for modeling sequential data.  
  The task focuses on **sentiment classification**, where the model predicts whether a movie review expresses a positive or negative opinion.  

- **Dataset**  
  - **IMDB Movie Reviews** — 25 000 labeled reviews for training and 25 000 for testing.  
  - Each review is represented as a sequence of word indices with a fixed vocabulary size (≈ 10 000 words).  

- **Approach**  
  - Implemented a simple **RNN-based classifier** trained using backpropagation through time (BPTT).  
  - Compared multiple runs to evaluate model stability and sensitivity to initialization.  
  - Performance tracked across epochs, measuring accuracy on the validation and test sets.  

- **Results**

  | Run | Accuracy (%) |
  |:---:|:-------------:|
  | 1 | 81.9 |
  | 2 | 84.1 |
  | 3 | 84.0 |
  | 4 | 84.5 |
  | 5 | 84.6 |
  | 6 | 84.9 |
  | 7 | 84.3 |
  | 8 | 84.3 |
  | 9 | 81.6 |
  | 10 | 82.7 |

  **Average Accuracy:** ≈ **83.7 %**

**Key Takeaways**  
- RNNs process sequences step by step, retaining context through hidden states.  
- They excel at **temporal or linguistic tasks** where word order and dependency matter.  
- Variability between runs highlights the stochastic nature of training sequential models.  

---

### [GrowingSelfOrganizingMap_GSOM.ipynb](./GrowingSelfOrganizingMap_GSOM.ipynb) — *Growing Self-Organizing Map (GSOM)*  

**Summary**  

- **Objective**  
  This notebook extends the concept of Self-Organizing Maps (SOMs) by implementing a **Growing Self-Organizing Map (GSOM)** — a dynamic neural network that **expands its structure** based on data complexity.  
  The goal is to show how GSOMs automatically adapt their grid size to represent data more efficiently.  

- **Dataset**  
  - **Zoo (UCI dataset)** — categorical animal features (17 attributes, 7 classes).  
  - Chosen for its clear feature-based separations (e.g., mammals, birds, fish) and suitability for visualizing GSOM node growth.  

- **Approach**  
  - Start with a minimal SOM grid (typically 2×2).  
  - Allow nodes to **grow dynamically** when the accumulated error in a region exceeds a threshold (the Growth Threshold).  
  - Each new node inherits nearby weights and adjusts over multiple iterations to preserve topology.  
  - Visualize how clusters form and how the network grows to represent all data categories.  

- **Results**  

  | Growth Threshold | Final Node Count | Observed Clusters |
  |:----------------:|:----------------:|:------------------|
  | 0.4 | 9 | Partial structure, underfit |
  | 0.2 | 16 | Clear category clusters |
  | 0.1 | 25 | Overfitting tendency, dense map |

  Lower thresholds allow finer granularity but may create redundant nodes.  
  The 0.2 configuration offered the best balance between topology preservation and interpretability.  

**Key Takeaways**  
- GSOMs improve on SOMs by **automatically growing** in regions with high data variance.  
- They reveal **data structure adaptively**, avoiding the need to predefine map size.  
- Useful for **exploratory analysis**, where cluster counts or topology are unknown.  

