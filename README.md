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
  _Summary:*  
  The basic ideas behind machine learning.  

  - **Supervised vs. Unsupervised Learning**  
    Both labeled and unlabeled approaches are explored: from predicting outcomes with known targets to finding natural groupings in raw data.  

  - **Machine Learning Workflow**  
    The process follows a clear path: preparing the data, fitting models, validating results, and checking how well they hold up on unseen samples.  

  - **Core Algorithms**  
    Classic methods such as linear regression, logistic regression, and decision trees are used to show different ways of handling prediction and classification problems.  

  - **Performance Metrics**  
    Results are measured with accuracy, precision/recall, R², and MAE, giving a balanced view of model strengths and weaknesses.  

  Finally a comparison of models and metrics, building a solid starting point for later experiments.

---

- **[D7041E_lab2.ipynb](./D7041E_lab2.ipynb)** — *LAB 2 Word Embedding*  
  _Summary:*  
  This lab moves into natural language processing, showing how words can be turned into numbers that capture meaning.  

  - **Word Embeddings**  
    Word2Vec and GloVe are introduced as ways of creating dense vector spaces where similar words are placed close together.  

  - **Cosine Similarity**  
    The closeness of word meanings is measured, making it possible to see which terms share context.  

  - **Visualization**  
    Tools like t-SNE and PCA reduce embeddings to two dimensions, making clusters and relationships easier to spot.  

  - **Applications**  
    The embeddings are put to work in tasks such as text classification and similarity search, showing their practical value.  

  The lab shows how embeddings go beyond simple word counts, providing a foundation for modern NLP.

---

- **[D7041E_lab3.ipynb](./D7041E_lab3.ipynb)** — *LAB 3 Random Hyperdimensional Data Representations*  
  _Summary:*  
  Here the focus shifts to hyperdimensional computing — a less common but powerful way of representing information.  

  - **Why High Dimensions?**  
    Random vectors in large dimensions are nearly orthogonal, making them robust to noise and easy to combine.  

  - **Generating Representations**  
    High-dimensional vectors are created and their properties examined, showing how separation comes naturally with scale.  

  - **Encoding and Binding**  
    Operations like addition, multiplication, and permutation are used to build structured representations out of simple random vectors.  

  - **Classification Example**  
    Hyperdimensional encodings are tested in a basic classification setting and compared with conventional ML pipelines.  

  The lab highlights the strengths of this alternative approach and how it can be used for compact, noise-tolerant learning.

---

- **[D7041E_lab4.ipynb](./D7041E_lab4.ipynb)** — *LAB 4 Self-Organizing Maps*  
  _Summary:*  
  Working with Self-Organizing Maps (SOMs), a way of clustering and visualizing complex data.  

  - **Concept**  
    SOMs map high-dimensional input data onto a two-dimensional grid, with nearby neurons representing similar inputs.  

  - **Training**  
    Neurons compete to match input vectors, and their weights are updated together with their neighbors, gradually shaping the grid.  

  - **Visualization**  
    The trained SOM provides a 2D picture of the data, where clusters and groupings become visible.  

  - **Clustering Applications**  
    SOMs are used to group similar items and compared with methods like k-means to see differences and overlaps.  

  The lab shows how SOMs make unsupervised learning interpretable by turning abstract data into something visual.

---

- **[D7041E_lab5.ipynb](./D7041E_lab5.ipynb)** — *LAB 5 ANN and Backpropagation*  
  _Summary:*  
  Focus on neural networks and the algorithm that makes them work: backpropagation.  

  - **Perceptron**  
    The perceptron is introduced as the simplest network, useful for showing how weighted inputs lead to decisions.  

  - **Multi-Layer Networks**  
    Adding hidden layers creates multi-layer perceptrons (MLPs), able to capture non-linear relationships.  

  - **Activation Functions**  
    Sigmoid, tanh, and ReLU are tested to show how different functions affect learning and performance.  

  - **Backpropagation**  
    The error is traced backwards through the network, with weights updated by gradient descent to improve predictions.  

  - **Training and Comparison**  
    Networks of different depths are trained, showing how deeper models handle more complex tasks.  

  The lab gives a hands-on view of how modern neural networks are trained and why backpropagation is essential.

---

- **[D7041E_lab6.ipynb](./D7041E_lab6.ipynb)** — *LAB 6 Recurrent Neural Networks*  
  _Summary:*  
  The lab focuses on sequential data and the networks designed to handle it.  

  - **Sequential Data**  
    Text, speech, and time-series data are used to show why past context matters for current predictions.  

  - **Vanilla RNN**  
    A simple recurrent network is built, passing hidden states forward to capture short-term dependencies.  

  - **Training Challenges**  
    Issues like vanishing and exploding gradients are observed, limiting how well standard RNNs handle long sequences.  

  - **LSTM and GRU**  
    More advanced architectures with gating mechanisms are introduced, making it possible to retain information over longer spans.  

  - **Applications**  
    RNNs are tested on tasks such as character prediction and forecasting, showing their ability to learn patterns over time.  

  The lab provides a clear overview of recurrent models, from the basic RNN to LSTM and GRU, and their role in sequence modeling.

---

- **[D7041E_lab6.ipynb](./D7041E_lab6.ipynb)** — *LAB 6 Recurrent Neural Networks*  
  _Summary:*  
  Explores **Recurrent Neural Networks (RNNs)**, a class of neural networks designed to model sequential and temporal data.  

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
