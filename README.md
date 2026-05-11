# 🎵 Music Genre Classification (GTZAN Dataset)

This project implements music genre classification using **Convolutional Neural Networks (CNN)** and **Traditional Machine Learning** models. We specifically focused on enhancing accuracy through advanced feature engineering and overlapped data chunking.

---

## 🚀 Key Improvements & Methodology
To outperform the baseline models in the original paper, we implemented several key changes:

* **Overlapped Chunking:** Instead of simple splitting, we used 3-second audio windows with 1.5-second overlaps, significantly increasing the training data density.
* **Enhanced Feature Set:** For traditional ML models, we extracted a comprehensive set of **94 spectral descriptors** (instead of the standard basic set).
* **CNN Architectures:** Designed custom layers with **Batch Normalization** and **Dropout** to stabilize training and prevent overfitting.

---

## 📊 Performance Metrics
The initial testing phase across 10 genres yielded the following results:

| Model Architecture | Accuracy Rate |
| :--- | :--- |
| **CNN (Mel-Spectrogram)** | **85%** |
| **CNN (MFCC)** | **~70%** |
| **Traditional ML (MLP/RF)** | **Significantly Improved** |

---

## 📂 Repository Structure
- `notebook_and_models/`: Contains all Jupyter Notebooks (`.ipynb`) for CNN and ML pipelines.
- `data/features/`: Pre-processed `.csv` files containing the extracted spectral features.
- `documents/`: Technical notes and implementation details.

> [!IMPORTANT]  
> **Note on Audio Files:** Due to GitHub's file size limitations, raw audio files (.au/.mp3) are not included. The models run directly using the pre-processed features located in the `data/features/` folder.

---

## 🛠️ How to Run
1. Clone this repository.
2. Ensure you have `TensorFlow`, `Librosa`, and `Scikit-learn` installed.
3. Run the notebooks inside the `notebook_and_models/` directory.
