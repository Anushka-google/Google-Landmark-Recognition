# 🏛️ Google Landmark Recognition using FAISS & Deep Learning

This project focuses on identifying landmarks from images using a **pretrained deep learning model** combined with **FAISS-based similarity search**.
The goal is to achieve high accuracy **without heavy training**, making the system efficient and scalable.

---

## 🚀 Overview

Instead of training a large neural network from scratch, this project uses:

* 🔹 Pretrained CNN models (ResNet50 / EfficientNet)
* 🔹 Feature extraction (image embeddings)
* 🔹 FAISS for fast similarity search
* 🔹 Weighted nearest neighbor voting for prediction

---

## 🧠 Pipeline

```
Image → Pretrained CNN → Embedding → Normalization → FAISS Index → Top-K Neighbors → Final Prediction
```

---

## 📊 Results

* ✅ Accuracy: **~84%**
* ⚡ Fast inference (no training required)
* 💡 Efficient even with limited compute resources

---

## 📁 Project Structure

```
Google-Landmark-Recognition/
│
├── notebook/
│   └── clean.ipynb
│
├── README.md
├── requirements.txt
```

---

## ⚙️ Tech Stack

* Python
* PyTorch
* FAISS (Facebook AI Similarity Search)
* NumPy / Pandas
* Scikit-learn
* Pillow

---

## 🔥 Key Features

* ❌ No heavy training required
* ✅ Uses pretrained models for feature extraction
* ⚡ Fast and scalable similarity search with FAISS
* 📈 High accuracy with optimized retrieval

---

## 💡 How It Works

1. Extract embeddings from images using a pretrained CNN
2. Normalize embeddings for better similarity comparison
3. Store embeddings in FAISS index
4. For a query image:

   * Retrieve top-K similar images
   * Apply weighted voting based on similarity
   * Predict final landmark

---

## 🏁 Future Improvements

* 🔹 Hybrid model (FAISS + classification fusion)
* 🔹 Re-ranking of retrieved results
* 🔹 Use of advanced losses like ArcFace
* 🔹 API integration (Google Vision / Hugging Face)

---

## 📌 Author

**Anurag Chauhan**

---

⭐ If you found this project useful, consider giving it a star!
