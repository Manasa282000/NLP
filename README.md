# NLP Text-to-Speech for Swahili Using BRNN

This repository presents a Text-to-Speech (TTS) system for Swahili using Bidirectional Recurrent Neural Networks (BRNN). The model generates high-quality synthetic speech based on Swahili text input, aimed at improving accessibility, human-computer interaction, and language preservation.

## Data

The dataset is too large (more than 25MB) to be uploaded directly here. Therefore, the dataset has been split into two parts: **Before Preprocessing** and **After Preprocessing**. You can download the dataset from the following Google Drive links:

- [Data Before Preprocessing](https://drive.google.com/drive/folders/1-d-PvXTqR951f9nmEzGPeb-6N34v1LiA?usp=drive_link)
- [Data After Preprocessing](https://drive.google.com/drive/folders/1j49Y4ceKga3VJfs-xfQ3vYLzqtdAgXsK?usp=drive_link)

### File Mapping

The dataset includes mapping files, which contain the paths to the mel spectrograms and the corresponding text files. This mapping is essential for training the model and generating accurate speech.

## Preprocessing Pipeline

1. **Convert Audio Files to .WAV Format**: The raw audio files are converted into the `.WAV` format.
2. **Generate Mel Spectrograms**: Mel spectrograms are generated from the audio files to capture the frequency and time-domain information.
3. **Map Text to Mel Spectrogram**: The provided mapping files associate the text with the corresponding Mel spectrograms.

The **Data After Preprocessing** folder contains the necessary files for training and evaluating the model.

## Model Overview

The system employs deep learning-based architectures, including:

- **Bidirectional RNN (BRNN)**: For capturing both forward and backward temporal dependencies in speech.
- **Attention Mechanisms**: To focus on the most relevant parts of the input text during speech synthesis.
- **Hybrid CNN-GRU Network**: Combines Convolutional Neural Networks (CNN) and Gated Recurrent Units (GRU) for better feature extraction and sequence learning.

The primary objective of the model is to accurately synthesize natural-sounding speech by modeling both linguistic and prosodic features of Swahili.

## How to Run

### Requirements

- Python 3.6+
- PyTorch
- librosa
- GPU support (recommended for faster training and inference)

### Steps

1. **Upload the necessary dataset**:
   - Use the **Data After Preprocessing** folder for training the model.
   - Ensure that you have the **File Mapping**, **Mel Spectrogram**, and **Text** files ready in your dataset.

2. **Install Dependencies**:
   - You need to install the following Python libraries:

   ```bash
   pip install torch librosa
