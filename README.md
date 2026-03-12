<div align="center">

# 🎵 Music Genre Classification

**Classifying music into 10 genres using Deep Learning and Machine Learning**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://www.tensorflow.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-f7931e.svg)](https://scikit-learn.org/)
[![Gradio](https://img.shields.io/badge/Gradio-UI-brightgreen.svg)](https://gradio.app/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[View Notebooks](#notebooks) · [Live Demo](#demo) · [Report](MusicGenreClassification_Report.pdf)

</div>

---

## 📖 Overview

An end-to-end music genre classification system that automatically categorizes audio tracks into **10 genres** using multiple ML/DL approaches. The project compares CNN-based deep learning models (trained on raw and feature-engineered spectrograms) with a traditional Random Forest classifier, and includes a **Gradio web interface** for real-time predictions.

### Supported Genres

`Blues` · `Classical` · `Country` · `Disco` · `Hip-Hop` · `Jazz` · `Metal` · `Pop` · `Reggae` · `Rock`

---

## 🏗️ Architecture

```
Audio Input (.wav)
       │
       ├──► Mel Spectrogram ──► CNN (Raw) ──────────────► Genre Prediction
       │
       ├──► Feature-Engineered Spectrogram ──► CNN ─────► Genre Prediction
       │
       └──► Extracted Features (MFCCs, Spectral, etc.)
                    │
                    └──► Random Forest Classifier ──────► Genre Prediction
```

---

## <a name="notebooks"></a>📓 Notebooks

| # | Notebook | Description | Colab |
|---|----------|-------------|-------|
| 1 | [Data_Pre-Processing.ipynb](Data_Pre-Processing.ipynb) | Data loading, cleaning, and preparation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Purnachander-Konda/MusicGenresClassification/blob/main/Data_Pre-Processing.ipynb) |
| 2 | [Feature_Engineering.ipynb](Feature_Engineering.ipynb) | Audio feature extraction (MFCCs, spectral features) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Purnachander-Konda/MusicGenresClassification/blob/main/Feature_Engineering.ipynb) |
| 3 | [ML-Model.ipynb](ML-Model.ipynb) | Random Forest classifier training & evaluation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Purnachander-Konda/MusicGenresClassification/blob/main/ML-Model.ipynb) |
| 4 | [CNN_raw.ipynb](CNN_raw.ipynb) | CNN trained on raw mel spectrograms | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Purnachander-Konda/MusicGenresClassification/blob/main/CNN_raw.ipynb) |
| 5 | [CNN_featured.ipynb](CNN_featured.ipynb) | CNN trained on feature-engineered spectrograms | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Purnachander-Konda/MusicGenresClassification/blob/main/CNN_featured.ipynb) |
| 6 | [Deployment.ipynb](Deployment.ipynb) | Gradio web app for real-time inference | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Purnachander-Konda/MusicGenresClassification/blob/main/Deployment.ipynb) |

---

## <a name="demo"></a>🚀 Live Demo

Run the Gradio demo locally or in Google Colab:

**Option 1 — Google Colab (no setup needed):**
Click the Colab badge next to [Deployment.ipynb](#notebooks) above to launch the interactive demo instantly.

**Option 2 — Local:**
```bash
# Clone the repo
git clone https://github.com/Purnachander-Konda/MusicGenresClassification.git
cd MusicGenresClassification

# Install dependencies
pip install -r requirements.txt

# Run the deployment notebook
jupyter notebook Deployment.ipynb
```

---

## ⚙️ Installation

### Prerequisites
- Python 3.8+
- pip

### Setup
```bash
git clone https://github.com/Purnachander-Konda/MusicGenresClassification.git
cd MusicGenresClassification
pip install -r requirements.txt
```

---

## 🛠️ Tech Stack

- **Audio Processing:** Librosa
- **Deep Learning:** TensorFlow / Keras
- **Machine Learning:** scikit-learn (Random Forest)
- **Computer Vision:** OpenCV (spectrogram processing)
- **Data Handling:** NumPy, Pandas
- **Deployment:** Gradio
- **Visualization:** Matplotlib, Seaborn

---

## 📂 Project Structure

```
MusicGenresClassification/
├── Data_Pre-Processing.ipynb       # Data preparation pipeline
├── Feature_Engineering.ipynb       # Audio feature extraction
├── ML-Model.ipynb                  # Random Forest model
├── CNN_raw.ipynb                   # CNN on raw spectrograms
├── CNN_featured.ipynb              # CNN on engineered spectrograms
├── Deployment.ipynb                # Gradio web app
├── MusicGenreClassification_Proposal.pdf
├── MusicGenreClassification_Report.pdf
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 📄 Documentation

- [Project Proposal](MusicGenreClassification_Proposal.pdf) — Problem statement, objectives, and methodology
- [Project Report](MusicGenreClassification_Report.pdf) — Detailed analysis, results, and conclusions

---

## 🤝 Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

**⭐ Star this repo if you found it useful!**

</div>
