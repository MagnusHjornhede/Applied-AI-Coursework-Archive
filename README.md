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
  This lab introduces the foundational concepts of machine learning.  
  You will explore:
  - The differences between **supervised** and **unsupervised** learning  
  - Key steps in a machine learning workflow: data preprocessing, model training, validation, and evaluation  
  - Core algorithms such as **linear regression**, **logistic regression**, and **decision trees**  
  - Basic performance metrics including **accuracy**, **precision/recall**, and **R²/MAE** for regression tasks  
  - Hands-on implementation in Python using common libraries like **NumPy**, **pandas**, and **scikit-learn**  

---

- **[D7041E_lab2.ipynb](./D7041E_lab2.ipynb)** — *LAB 2 Word Embedding*  
  _Summary:*  
  This lab focuses on **word representations in Natural Language Processing (NLP)**.  
  You will learn how raw text data can be transformed into numerical vectors that capture semantic meaning.  
  Topics and activities include:  
  - Introduction to **word embeddings** and why they are superior to bag-of-words models  
  - Using **Word2Vec** and **GloVe** to generate dense vector representations  
  - Exploring **cosine similarity** to measure semantic closeness between words  
  - Visualizing embedding spaces with techniques like **t-SNE** or **PCA**  
  - Applying embeddings in simple downstream tasks such as **text classification** or **similarity search**  

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
