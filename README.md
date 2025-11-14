<h1 align="center">📘 Betel Bloom: A Comparative Performance Study 📘</h1>



<p align="center">
  <img src="https://i.pinimg.com/736x/55/5e/f9/555ef9c5cb740f9cb3ac47c3eeacdacd.jpg" alt="Web Development Showcase Banner" width="1200">
</p>



## 🚀 Overview  
This project compares **Supervised Learning** vs **Self-Supervised Learning (SSL)** on the **PriBeL Betel Leaf Dataset**.  
The goal is to understand how well models learn visual features with labels vs without labels — through clean, reproducible experiments.



## 🔥 Key Features  
- 📊 Comprehensive EDA (RGB/HSV stats, sharpness, noise, augmentations, duplicates, class balance)  
- 🧠 Supervised Baselines (EfficientNet)  
- 🌀 SSL Methods (SimSiam)  
- 🧪 Downstream Evaluation (Linear Probe, MLP, SVM, k-NN, Fine-tuning)  
- 🌐 Embedding Visualization (t-SNE, UMAP, PCA + Silhouette)  
- ⚖️ Ablations & Statistical Tests (t-test, Wilcoxon, Friedman)  
- 🔁 Checkpointing + Resumable Training  
- ⚡ Fully reproducible on Kaggle  

📌 Note: Some project files are not included in this repository because they belong to other collaborators. Only the work I personally completed is shared here.

## 📦 Dataset  
**PriBeL — Primary Betel Leaf Dataset (1,800 images)**  
- Healthy  
- Diseased  
- Dried  
- On-field + Controlled Environment  
- All images: 1080×1080 resolution  

Dataset link: [PriBeL Betel Leaf Dataset](https://data.mendeley.com/datasets/btdym2t6mt/1)

---

## 📁 Project Structure  
```text
├── EDA/
│   └── eda_notebook.ipynb
├── Supervised/
│   └── efficientnet_baseline.ipynb
├── SSL/
│   └── simsiam.ipynb
├── Ablations/
│   └── ssl_ablations.ipynb
├── Results/
│   ├── metrics/
│   └── embeddings/
├── models/
│   └── saved_checkpoints/
├── LICENSE
└── README.md
```


## 🛠 Installation
```bash
git clone https://github.com/Shourav-Deb/Betel-Bloom.git
```

## ▶️ Usage
- Run on Kaggle / Collab: Open any notebook and click Run All for a fully reproducible workflow.
- Local (optional): python train_supervised.py

## 📜 License

Shared under the Neo Non-Commercial Learning License (NCLL 1.0).
Use for learning only, not commercial.

For commercial licensing: [contact me](mailto:heyneeddev@gmail.com)

---
