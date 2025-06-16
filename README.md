# 🎧 Deepfake Audio Detection

This project is a deep learning-based system for detecting audio deepfakes using neural networks. It analyzes various audio features to determine whether a given voice clip is real or AI-generated (fake).

## 🚀 Demo

A simple Gradio interface allows users to upload audio files and instantly get a prediction.

---

## 🧠 Model Overview

- Built using `TensorFlow` / `Keras`
- Trained on real and fake audio samples
- Final model saved as: `mano.h5`

### 📈 Features Extracted

The system uses `librosa` to extract a rich set of features:

- MFCC (Mel-frequency cepstral coefficients)
- Chroma Features
- Spectral Centroid
- Spectral Bandwidth
- Spectral Rolloff
- Zero-Crossing Rate
- RMS Energy
- Tonnetz

These features are stacked and fed into the model for time-series analysis.

---

## 🛠️ Tech Stack

- Python 🐍
- TensorFlow / Keras
- Librosa (for audio feature extraction)
- Gradio (for UI)

---

## 💡 How It Works

1. User uploads an audio file (`.wav`, `.mp3`, etc.)
2. Features are extracted and reshaped
3. The model predicts whether the input is **Real** or **Fake**

---

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
