# Emotion Recognition from Speech

## Project Overview

This project focuses on recognizing human emotions from speech audio using Deep Learning techniques. The model analyzes speech signals and classifies them into different emotional categories such as Happy, Sad, Angry, Fearful, Neutral, Disgust, and Surprised.

Emotion recognition from speech has applications in human-computer interaction, virtual assistants, customer service analysis, mental health monitoring, and intelligent communication systems.

---

## Objective

To develop a speech emotion recognition system capable of identifying human emotions from audio recordings using extracted acoustic features and Deep Learning models.

---

## Dataset

Dataset Used: RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)

The dataset contains professionally recorded speech samples representing multiple emotional states.

### Emotion Classes

- Neutral
- Calm
- Happy
- Sad
- Angry
- Fearful
- Disgust
- Surprised

---

## Project Workflow

### 1. Data Collection

- Downloaded and organized the RAVDESS dataset.
- Loaded speech audio files from all actor folders.
- Extracted emotion labels from file names.

### 2. Data Preprocessing

- Audio loading using Librosa.
- Resampling audio signals.
- Noise reduction and normalization.
- Feature extraction from speech signals.

### 3. Feature Extraction

Mel-Frequency Cepstral Coefficients (MFCCs) were extracted from audio samples.

Features extracted:

- MFCC
- Chroma Features
- Mel Spectrogram
- Spectral Contrast
- Tonnetz Features

---

## Model Architecture

A Deep Neural Network (DNN) was implemented for emotion classification.

### Layers

- Input Layer
- Dense Layer
- ReLU Activation
- Dropout Layer
- Dense Layer
- ReLU Activation
- Dropout Layer
- Output Layer (Softmax)

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Librosa
- TensorFlow
- Keras
- Scikit-learn

---

## Data Visualization

The following visualizations were generated during analysis:

### Emotion Distribution
Shows the number of samples available for each emotion class.

### Training Accuracy
Tracks model learning performance across epochs.

### Validation Accuracy
Measures generalization performance on unseen data.

### Training Loss
Shows reduction in prediction error during training.

### Validation Loss
Helps monitor overfitting and model convergence.

### Confusion Matrix
Visualizes correct and incorrect emotion classifications.

---

## Model Performance

Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1-Score

### Results

| Metric | Score |
|----------|----------|
| Training Accuracy | 54% |
| Validation Accuracy | 50% |
| Training Loss | 1.28 |
| Validation Loss | 1.39 |

The model demonstrates the ability to learn emotional patterns from speech audio and classify emotions with reasonable performance.

---

## Project Structure

```
Task2_Emotion_Recognition_From_Speech/
│
├── emotion_recognition.py
├── ravdess_dataset/
├── saved_model/
├── training_accuracy.png
├── validation_accuracy.png
├── training_loss.png
├── validation_loss.png
├── confusion_matrix.png
├── requirements.txt
└── README.md
```

---

## How to Run

### Clone Repository

```bash
git clone https://github.com/your-username/CodeAlpha_ML_Internship.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Project

```bash
python emotion_recognition.py
```

---

## Future Improvements

- Use CNN and LSTM architectures.
- Apply audio data augmentation.
- Increase dataset size.
- Hyperparameter optimization.
- Real-time emotion prediction from microphone input.
- Deploy as a web application.

---

## Conclusion

This project demonstrates the application of Deep Learning and speech signal processing techniques for Speech Emotion Recognition. By extracting meaningful audio features and training a neural network, the system can identify emotional states from human speech and serve as a foundation for intelligent audio-based applications.

---

## Internship Information

**Internship:** CodeAlpha Data Science Internship

**Task:** Task 2 - Emotion Recognition from Speech

**Domain:** Machine Learning and Deep Learning
