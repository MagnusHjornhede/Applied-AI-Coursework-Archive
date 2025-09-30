# Applied Artificial Intelligence — Labs & Notebooks

This repository collects a hands-on set of Jupyter notebooks covering core techniques in applied AI/ML—data handling, modeling, evaluation, and explainability. Each lab is self-contained and designed to be run locally or in the cloud (e.g., Colab).

---

## Repository Structure
```
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
- **[D7041E_lab1.ipynb](./D7041E_lab1.ipynb)** — *LAB 1  Fundamentals of Machine Learning*  
  _Focus:_ Classification, Computer Vision  
  _Stack:_ NumPy, scikit-learn, matplotlib, zipfile, PIL, os  
  _Summary:_ # LAB 1 Fundamentals of Machine Learning ## D7041E “Applied artificial intelligence”
- **[D7041E_lab2.ipynb](./D7041E_lab2.ipynb)** — *LAB 2 Word	Embedding*  
  _Focus:_ Classification  
  _Stack:_ nltk, NumPy, gensim, scipy  
  _Summary:_ # LAB 2 Word Embedding ## D7041E “Applied artificial intelligence”
- **[D7041E_lab3.ipynb](./D7041E_lab3.ipynb)** — *LAB 3 Random Hyperdimensional Data Representations*  
  _Focus:_ Classification, NLP  
  _Stack:_ zipfile, os, re, NumPy, matplotlib, seaborn  
  _Summary:_ # LAB 3 Random Hyperdimensional Data Representations ## D7041E “Applied artificial intelligence”
- **[D7041E_lab4.ipynb](./D7041E_lab4.ipynb)** — *LAB 4 Self-Organized Maps*  
  _Focus:_ Classification, Computer Vision  
  _Stack:_ NumPy, matplotlib, math, time, pandas, TensorFlow/Keras  
  _Summary:_ # LAB 4 Self-Organized Maps ## D7041E “Applied artificial intelligence”
- **[D7041E_lab5.ipynb](./D7041E_lab5.ipynb)** — *LAB 5 ANN and Backpropagation*  
  _Focus:_ Classification  
  _Stack:_ NumPy, sys, TensorFlow/Keras  
  _Summary:_ # LAB 5 ANN and Backpropagation ## D7041E “Applied artificial intelligence”
- **[D7041E_lab6.ipynb](./D7041E_lab6.ipynb)** — *LAB 6 Recurrent Neural Networks*  
  _Focus:_ Classification, Regression  
  _Stack:_ NumPy, matplotlib, scipy  
  _Summary:_ # LAB 6 Recurrent Neural Networks ## D7041E “Applied artificial intelligence”

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

