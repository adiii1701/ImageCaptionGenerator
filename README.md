# 🖼️ Image Caption Generator using Deep Learning

This project implements an **Image Caption Generator**, a deep learning model that automatically generates textual descriptions for images. By combining **Computer Vision** and **Natural Language Processing (NLP)** techniques, the model is capable of understanding the content of an image and describing it in natural, grammatically correct language.

## 🚀 Project Overview

The model architecture is based on two core components:

- **CNN (Convolutional Neural Network)** for image feature extraction  
- **LSTM (Long Short-Term Memory Network)** for generating sequential text (captions)

A pre-trained CNN model such as **InceptionV3** or **VGG16** is used to extract high-level image features, which are then fed into an LSTM model that predicts the next word in a caption sequence based on the previous words and the image context.

## 📚 Dataset

The model is trained on the **Flickr8k Dataset**, which contains **8,000 images**, each annotated with **five unique human-written captions**. This diversity helps the model understand multiple ways of describing the same image. Captions are tokenized, cleaned, and padded for consistency during training.

📦 Dataset link: [Flickr8k on Kaggle](https://www.kaggle.com/datasets/adityajn105/flickr8k)

## 🧠 Training & Evaluation

The LSTM is trained using categorical cross-entropy loss to predict the most likely next word in a sequence. During evaluation, the model generates captions which are then compared against reference captions using the **BLEU Score**, a standard metric for machine translation and captioning accuracy.

## 🔍 Key Features

- Pre-trained CNN for efficient visual understanding  
- LSTM for context-aware language modeling  
- BLEU score evaluation for measuring caption quality  
- Clean, modular code in Jupyter Notebook format  

## 💡 Applications

This system can be integrated into:

- Accessibility tools for the visually impaired  
- Content tagging and organization platforms  
- Automated surveillance and media analysis  
- E-commerce product captioning

## 📁 How to Run

1. Clone the repo  
2. Install dependencies  
3. Download the [Flickr8k dataset](https://www.kaggle.com/datasets/adityajn105/flickr8k) and place it in the appropriate directory  
4. Run the notebook and follow the instructions to train or test the model

