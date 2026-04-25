# LocaLens 🔍🎨

LocaLens is a visual search prototype that retrieves images from a user’s gallery based on **dominant color and shape features**. Instead of relying on text or metadata, it enables **content-based image retrieval (CBIR)** using computer vision techniques.

The system leverages the YOLO model for object detection and combines it with color and shape analysis to deliver visually relevant results.

---

## 🚀 Problem Statement

Traditional image search depends on filenames, tags, or manual organization. This project explores a more intuitive approach:

> “Find images that *look similar*, not just those that are labeled similarly.”

---

## 🧠 Core Features

* 🎨 **Color-based filtering** (dominant color extraction)
* 🔷 **Shape-based similarity detection**
* 🧩 **Object detection using YOLO**
* 🔍 **Content-Based Image Retrieval (CBIR) pipeline**
* 📂 Works directly on local image collections (gallery-style input)

---

## 🏗️ Project Structure

```
LocaLens/
│── prototype_2.1.ipynb   # Main notebook (pipeline)
│── README.md             # Documentation
```

---

## ⚙️ Tech Stack

* Python
* Jupyter Notebook
* OpenCV
* NumPy / Pandas
* YOLO (object detection)

---

## 🔄 Workflow

1. **Image Input**

   * Load images from dataset / local directory

2. **Preprocessing**

   * Resize and normalize images
   * Prepare for feature extraction

3. **Feature Extraction**

   * Dominant color detection (clustering)
   * Shape detection (contours / structural features)

4. **Object Detection**

   * Apply YOLO to identify key objects

5. **Similarity Matching**

   * Compare images based on extracted features

6. **Result Retrieval**

   * Return visually similar images

---

## 📊 Results & Observations

* Successfully retrieves visually similar images based on:

  * Color similarity
  * Shape patterns
* Performs well for clearly distinguishable visual features
* Limitations observed in:

  * Complex backgrounds
  * Multiple overlapping objects
---

## 📦 Dataset

* Dataset sourced from Kaggle
* Contains diverse images used for testing visual similarity and detection
---


## 💡 Key Insight

This project demonstrates how combining **object detection + low-level visual features (color & shape)** can create a functional visual search system without relying on text annotations.

---

