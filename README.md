<div align="center">

# 🧠 Deep Learning Projects

### 9 Applied Deep Learning Projects — Computer Vision, NLP, Regression & Classification

> _Not tutorials. Actual problems, actual datasets, actual models that work._

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://tensorflow.org)
[![Keras](https://img.shields.io/badge/Keras-Deep_Learning-D00000?style=for-the-badge&logo=keras&logoColor=white)](https://keras.io)
[![OpenCV](https://img.shields.io/badge/OpenCV-Vision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org)
[![Google Colab](https://img.shields.io/badge/Google_Colab-Ready-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)](https://matplotlib.org)

</div>

---

## 📌 What It Does

**Deep_Learning_Projects** is a collection of 9 applied deep learning notebooks spanning Computer Vision, NLP, and Regression — each solving a real, concrete problem end-to-end: data loading, preprocessing, model building, training, and evaluation.

Every notebook is **self-contained and Colab-ready** — open, run all cells, see results.

---

## 📂 Projects Catalogue

### 👁️ Computer Vision

| Project | What It Does | Key Technique |
|---|---|---|
| `Cat_Breed_Classification.ipynb` | Identifies cat breed from photo | Transfer Learning (VGG16) |
| `Dogs_vs_Cats_Classification.ipynb` | Binary classifier — dog or cat | CNN + Data Augmentation |
| `Human_vs_Monkeys_Classification.ipynb` | Distinguishes humans from monkeys | Transfer Learning + Fine-tuning |
| `Age_Gender_Prediction.ipynb` | Predicts age & gender from face image | Multi-output CNN |
| `Binary_Classification_Custom.ipynb` | Custom binary image classifier | CNN from scratch |
| `MNIST_(Multi)Classification.ipynb` | Digit recognition 0–9 | Dense / Conv Neural Net |

### 📝 NLP

| Project | What It Does | Key Technique |
|---|---|---|
| `IMDB_Data_Analysis.ipynb` | Sentiment analysis on movie reviews | LSTM / Embedding + Dense |
| `Next_Jock_Predictor.ipynb` | Predicts next word / joke completion | RNN / LSTM Language Model |

### 📈 Regression

| Project | What It Does | Key Technique |
|---|---|---|
| `Regression_Car_Fuel_Consu.ipynb` | Predicts car fuel consumption | Neural Network Regression |

---

## 🏛️ Architecture Patterns Used

```
  COMPUTER VISION PROJECTS
  ────────────────────────────────────────────────────────
  Input Image (224×224×3 or 28×28)
       │
  ┌────▼──────────────────────────────────────┐
  │  Option A: CNN from Scratch               │
  │  Conv2D → ReLU → MaxPool (×N)             │
  │  → Flatten → Dense → Softmax/Sigmoid      │
  └────────────────────────────────────────────┘
       │
  ┌────▼──────────────────────────────────────┐
  │  Option B: Transfer Learning (VGG16)      │
  │  Pretrained Base (frozen)                 │
  │  → GlobalAvgPool → Dense → Output         │
  └────────────────────────────────────────────┘

  NLP PROJECTS
  ────────────────────────────────────────────────────────
  Raw Text
       │
  Tokenize → Integer encode → Pad sequences
       │
  Embedding Layer (vocab_size × embed_dim)
       │
  LSTM(128) → Dense(64) → Output
  (sentiment: sigmoid | next word: softmax)

  REGRESSION PROJECT
  ────────────────────────────────────────────────────────
  Tabular features (engine size, cylinders...)
       │
  Normalize → Dense(64,relu) → Dense(32,relu) → Dense(1)
  Loss: MSE  │  Metric: MAE / R²
```

---

## 🖥️ Demo

> Run any notebook — Colab loads in ~10 seconds with free GPU.

```
📸  Best screenshots to capture per project:

  Dogs_vs_Cats     → Validation accuracy curve + sample predictions grid
  Age_Gender       → Face image with predicted "Age: 24, Gender: Male"
  IMDB Sentiment   → Review text + "Positive 94%" output
  MNIST            → 10×10 digit grid with predicted labels
```

**Sample — Dogs vs Cats prediction output:**

```
  ┌──────────────────────────────────────────────┐
  │  [🐕 image]  →  Dog    97.3%  ████████████  │
  │  [🐈 image]  →  Cat    91.8%  ███████████   │
  │  [🐕 image]  →  Dog    88.5%  ██████████    │
  │  Val Accuracy: 94.2%  │  Epochs: 15         │
  └──────────────────────────────────────────────┘
```

---

## ⚡ How to Run

### One-Click — Google Colab (No Setup)

1. Click any `.ipynb` file in this repo
2. Click **"Open in Colab"** button at top  
   *(or prefix URL with `colab.research.google.com/github/Rohan171819/Deep_Learning_Projects./blob/main/`)*
3. Runtime → **Run All**

> GPU recommended for vision projects: Runtime → Change runtime type → T4 GPU (free)

### Local Setup

```bash
git clone https://github.com/Rohan171819/Deep_Learning_Projects..git
cd Deep_Learning_Projects.

pip install tensorflow keras numpy pandas matplotlib seaborn opencv-python pillow jupyter
jupyter notebook
```

---

## 🗺️ Roadmap

- [x] Binary & multi-class image classification
- [x] Transfer learning (VGG16 fine-tuning)
- [x] Multi-output CNN (Age + Gender)
- [x] NLP sentiment analysis (IMDB)
- [x] Language model (Next word prediction)
- [x] Neural network regression
- [ ] Add Colab badges to all notebooks
- [ ] Add sample output images per project
- [ ] Grad-CAM visualization for vision models

---

## 👤 Author

**Rohan Sharma** — AI/ML Engineer · LangGraph Developer  
MCA @ GL Bajaj | BCA @ GGSIPU — 9.5 CGPA

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/rohan-sharma-048266246)
[![Email](https://img.shields.io/badge/Email-sharma1718rohan@gmail.com-D14836?style=flat-square&logo=gmail)](mailto:sharma1718rohan@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat-square&logo=github)](https://github.com/Rohan171819)

---
<div align="center">

**⭐ Star if any of these models correctly classified your pet**

</div>

