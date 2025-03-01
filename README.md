NLP Text-to-Speech for Swahili Using BRNN
This repository presents a Text-to-Speech (TTS) system for Swahili using Bidirectional Recurrent Neural Networks (BRNN). The model generates high-quality synthetic speech based on Swahili text input, aimed at improving accessibility, human-computer interaction, and language preservation.

Data
The dataset is too large (more than 25MB) to be uploaded directly here. Therefore, I have provided links to the Google Drive folders containing the data before and after preprocessing.

Data Before Preprocessing: https://drive.google.com/drive/folders/1-d-PvXTqR951f9nmEzGPeb-6N34v1LiA?usp=drive_link
Data After Preprocessing: https://drive.google.com/drive/folders/1j49Y4ceKga3VJfs-xfQ3vYLzqtdAgXsK?usp=drive_link
File Mapping
The dataset includes mapping files, which contain the paths to the mel spectrograms and the corresponding text files. This mapping is essential for training the model and generating accurate speech.

Preprocessing Pipeline
Convert Audio files to .WAV format
Generate Mel Spectrograms from the audio files
Map Text to Mel Spectrogram using the provided mapping files
Model Overview
The system employs deep learning-based architectures, including Bidirectional RNNs with attention mechanisms and a hybrid CNN-GRU network. The primary objective is to accurately synthesize natural-sounding speech by modeling both linguistic and prosodic features of Swahili.

