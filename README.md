# Applied Artificial Intelligence — Labs & Notebooks

This repository contains core techniques in applied AI/ML—data handling, modeling, evaluation, and explainability. Each lab is self-contained and designed to be run locally or in the cloud (e.g., Colab).

---

## Repository Structure

```bash
.
├─ D7041E_lab1.ipynb
├─ D7041E_lab2.ipynb
├─ D7041E_lab3.ipynb
├─ D7041E_lab4.ipynb
├─ D7041E_lab5.ipynb
├─ D7041E_lab6.ipynb
└─ README.md  ← you are here
```

## Notebooks

- **[D7041E_lab1.ipynb](./D7041E_lab1.ipynb)** — *LAB 1 Fundamentals of Machine Learning*  
  _Summary:_  
  This lab covers the foundational concepts of machine learning through practical examples and experiments.  

  - **Supervised vs. Unsupervised Learning**  
    Examples of supervised tasks are demonstrated using labeled datasets where the target output is known.  
    Unsupervised methods are explored by clustering data without labels, highlighting the structural differences between the two approaches.  

  - **Machine Learning Workflow**  
    The notebook follows the standard ML pipeline: data is loaded and preprocessed, models are trained on a subset of the data, and validation is carried out on held-out samples.  
    The evaluation stage is used to measure model generalization and to compare different algorithmic choices.  

  - **Core Algorithms**  
    Several fundamental algorithms are implemented and tested:  
    - *Linear Regression* for predicting continuous target variables.  
    - *Logistic Regression* for binary classification tasks.  
    - *Decision Trees* for both regression and classification, showing interpretable rule-based decision boundaries.  

  - **Performance Metrics**  
    A set of key evaluation metrics are calculated and analyzed:  
    - *Accuracy* to measure overall correctness in classification problems.  
    - *Precision* and *Recall* to evaluate performance on imbalanced datasets.  
    - *R²* and *Mean Absolute Error (MAE)* to quantify regression performance.  

  The notebook concludes with comparisons of models and metrics, establishing a baseline understanding of how supervised and unsupervised learning methods operate in practice.

---

- **[D7041E_lab2.ipynb](./D7041E_lab2.ipynb)** — *LAB 2 Word Embedding*  
  _Summary:_  
  This lab examines **word representations in Natural Language Processing (NLP)** and demonstrates how raw text can be transformed into numerical vectors that preserve semantic meaning.  

  - **Introduction to Word Embeddings**  
    Word embeddings are presented as an improvement over traditional bag-of-words models, capturing contextual and semantic information rather than relying only on word counts.  

  - **Word2Vec and GloVe**  
    Dense vector representations are generated using Word2Vec and GloVe, showing how similar words are mapped close together in the embedding space.  

  - **Cosine Similarity**  
    Semantic similarity between words is evaluated using cosine similarity, illustrating how embeddings enable meaningful comparisons beyond simple text matching.  

  - **Visualization of Embeddings**  
    High-dimensional embeddings are reduced and visualized with methods such as t-SNE and PCA, making relationships between words visible in two dimensions.  

  - **Downstream Applications**  
    Embeddings are applied to tasks like text classification and similarity search, demonstrating how they can improve performance by leveraging semantic relationships.  

  The lab highlights how modern NLP relies on embeddings as a foundation for capturing meaning and supporting downstream machine learning models.

---

- **[D7041E_lab3.ipynb](./D7041E_lab3.ipynb)** — *LAB 3 Random Hyperdimensional Data Representations*  
  _Summary:_  
  This lab explores the concept of **hyperdimensional computing (HDC)**, where data is represented using very high-dimensional random vectors instead of conventional low-dimensional features.  

  - **Motivation for Hyperdimensional Representations**  
    The lab introduces the rationale for using high-dimensional spaces, emphasizing properties such as robustness to noise, ease of combination, and near-orthogonality of random vectors.  

  - **Generating High-Dimensional Vectors**  
    Random vectors are generated and their statistical properties are analyzed, showing how high dimensionality enables separation and resilience in representation.  

  - **Encoding and Binding Operations**  
    Operations such as addition, multiplication, and permutation are applied to vectors to encode and bind information, demonstrating how symbolic structures can be represented in distributed form.  

  - **Application to Classification**  
    Hyperdimensional representations are used in a simple classification setting, showing how high-dimensional encodings can serve as efficient alternatives to traditional feature engineering.  

  - **Comparison with Conventional ML Pipelines**  
    Results are compared with baseline machine learning methods to highlight the benefits and trade-offs of hyperdimensional approaches.  

  The lab demonstrates how hyperdimensional computing can represent data in compact, noise-tolerant ways and opens a perspective on alternative computing paradigms for AI.

---

- **[D7041E_lab4.ipynb](./D7041E_lab4.ipynb)** — *LAB 4 Self-Organizing Maps*  
  _Summary:_  
  This lab investigates **Self-Organizing Maps (SOMs)**, an unsupervised neural network method used for clustering and visualizing high-dimensional data.  

  - **Concept of Self-Organizing Maps**  
    SOMs are introduced as competitive learning networks that project high-dimensional input data onto a low-dimensional grid of neurons, preserving topological relationships.  

  - **Training Procedure**  
    The iterative training process is demonstrated, where neurons compete to represent input vectors and their weights are updated according to a neighborhood function.  

  - **Visualization of Data Mapping**  
    Data points are mapped to specific regions of the 2D SOM grid, making it possible to see how clusters of similar inputs emerge during training.  

  - **Clustering Applications**  
    SOMs are applied to datasets for clustering tasks, highlighting their ability to group similar items without supervision.  

  - **Comparison with Other Clustering Methods**  
    Results from SOMs are compared with standard techniques such as k-means, showing both the similarities in grouping and the added interpretability of the SOM’s spatial layout.  

  The lab demonstrates how SOMs can reveal structure in complex data and provide an interpretable visualization of clustering outcomes.

---

- **[D7041E_lab5.ipynb](./D7041E_lab5.ipynb)** — *LAB 5 ANN and Backpropagation*  
  _Summary:_  
  This lab focuses on **Artificial Neural Networks (ANNs)** and the use of **backpropagation** to train them effectively.  

  - **Perceptron as a Building Block**  
    The perceptron model is introduced as the simplest form of a neural network, illustrating how linear decision boundaries can be constructed from weighted sums and activation functions.  

  - **Multi-Layer Perceptrons (MLPs)**  
    The perceptron is extended into multi-layer architectures with hidden layers, allowing the network to capture non-linear relationships in data.  

  - **Activation Functions**  
    Different activation functions such as sigmoid, tanh, and ReLU are implemented and compared, showing how they influence learning dynamics and convergence.  

  - **Backpropagation Algorithm**  
    The mechanics of backpropagation are demonstrated, including the calculation of gradients, propagation of errors backward through the network, and weight updates using gradient descent.  

  - **Training and Evaluation**  
    Networks are trained on example datasets, with metrics tracked to evaluate learning progress and to compare the effect of different architectures or hyperparameters.  

  - **Comparison of Shallow vs. Deep Networks**  
    Results highlight how deeper networks with multiple hidden layers outperform single-layer perceptrons in capturing complex patterns.  

  The lab establishes a practical understanding of how ANNs learn and provides insight into the fundamental algorithm that powers modern deep learning.

---

- **[D7041E_lab6.ipynb](./D7041E_lab6.ipynb)** — *LAB 6 Recurrent Neural Networks*  
  _Summary:_  
  This lab explores **Recurrent Neural Networks (RNNs)**, a class of neural networks designed to model sequential and temporal data.  

  - **Sequential Data and Temporal Dependencies**  
    The lab introduces the challenges of sequence modeling, where current predictions depend not only on the present input but also on previous context, such as in text, speech, or time-series data.  

  - **Vanilla RNN Architecture**  
    A basic RNN is implemented to demonstrate how hidden states are updated over time and how information flows through a sequence of inputs.  

  - **Training Behavior and Limitations**  
    Experiments show the strengths of RNNs in capturing short-term dependencies, while also highlighting issues like vanishing and exploding gradients that limit their ability to model long sequences.  

  - **LSTM and GRU Architectures**  
    To address the limitations of vanilla RNNs, the lab explores Long Short-Term Memory (LSTM) and Gated Recurrent Unit (GRU) models, which introduce gating mechanisms to retain information over longer time spans.  

  - **Practical Applications**  
    RNNs are applied to tasks such as character-level prediction and simple time-series forecasting, demonstrating their ability to capture sequential patterns more effectively than feed-forward networks.  

  - **Comparison with Non-Recurrent Models**  
    Results underline the advantages of recurrent architectures in sequence modeling compared to standard ANNs, particularly in handling contextual dependencies.  

  The lab provides a complete overview of recurrent networks, from the basic RNN to advanced gated architectures, and illustrates their role in modern sequence-based machine learning.

---

- **[D7041E_lab3.ipynb](./D7041E_lab3.ipynb)** — *LAB 3 Random Hyperdimensional Data Representations*  
  _Summary:*  
  This lab introduces the emerging field of **hyperdimensional computing (HDC)** and its use for data representation.  
  Instead of working in low-dimensional feature spaces, HDC leverages **very high-dimensional random vectors** to encode and process information.  
  Key concepts and activities include:  
  - Understanding the motivation for hyperdimensional (HD) representations  
  - Generating **random high-dimensional vectors** and exploring their mathematical properties (orthogonality, robustness)  
  - Encoding and binding information using **vector operations** (addition, multiplication, permutation)  
  - Applying HD representations to simple **classification problems**  
  - Comparing HD computing approaches with conventional machine learning pipelines  

---

- **[D7041E_lab4.ipynb](./D7041E_lab4.ipynb)** — *LAB 4 Self-Organizing Maps*  
  _Summary:*  
  This lab explores **Self-Organizing Maps (SOMs)**, an unsupervised learning method introduced by Teuvo Kohonen for projecting high-dimensional data into low-dimensional (typically 2D) grids.  
  The focus is on how SOMs can cluster and visualize complex datasets.  
  Key topics and activities include:  
  - Understanding the structure of a SOM and how **neurons compete** to represent input data  
  - Training a SOM using an **unsupervised competitive learning algorithm**  
  - Visualizing how input vectors are mapped onto a 2D grid  
  - Using SOMs for **clustering tasks** such as grouping similar data points or patterns  
  - Comparing SOM results with conventional clustering approaches (e.g., k-means)  

---

- **[D7041E_lab5.ipynb](./D7041E_lab5.ipynb)** — *LAB 5 ANN and Backpropagation*  
  _Summary:*  
  This lab provides a practical introduction to **Artificial Neural Networks (ANNs)** and the **backpropagation algorithm** used for training them.  
  You will move from the theory of perceptrons to building and training small neural networks.  
  Key topics and activities include:  
  - Revisiting the concept of a **perceptron** and how it models linear decision boundaries  
  - Extending to **multi-layer perceptrons (MLPs)** with hidden layers and nonlinear activation functions  
  - Step-by-step implementation of **backpropagation** for weight updates using gradient descent  
  - Experimenting with different **activation functions** (sigmoid, tanh, ReLU)  
  - Training simple ANNs on toy datasets and monitoring performance metrics  
  - Comparing training outcomes with and without hidden layers to understand model capacity  

---

- **[D7041E_lab6.ipynb](./D7041E_lab6.ipynb)** — *LAB 6 Recurrent Neural Networks*  
  _Summary:*  
  This lab introduces **Recurrent Neural Networks (RNNs)**, a neural architecture designed to handle **sequential data** such as text, speech, and time series.  
  You will study how RNNs differ from feed-forward networks by maintaining hidden states across time steps.  
  Key topics and activities include:  
  - Understanding the need for **temporal context** in modeling sequences  
  - Implementing a basic **vanilla RNN** and observing its strengths and limitations  
  - Exploring issues such as **vanishing and exploding gradients**  
  - Introducing improved architectures: **LSTM (Long Short-Term Memory)** and **GRU (Gated Recurrent Unit)**  
  - Training RNNs on simple sequence tasks (e.g., character prediction or time series forecasting)  
  - Comparing RNN-based models with feed-forward ANNs to highlight their advantages on sequential data  

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
