# Image Caption Generator

## Project Overview
This project implements an **Image Caption Generator** using a **CNN (Convolutional Neural Network)** for feature extraction and an **LSTM (Long Short-Term Memory)** network for text generation. The model is trained on the **Flickr30k** dataset to automatically generate descriptive captions for input images.

## Team Members
- **Shreyas** (CB.EN.U4CSE22154)  
- **Uma Mahesh** (CB.EN.U4CSE22534)  
- **Sathvik Reddy** (CB.EN.U4CSE22160)  
- **Hemanth Reddy** (CB.EN.U4CSE22558)  

## Features
- ✔ **CNN (VGG16)** for extracting image features  
- ✔ **LSTM Network** for generating captions  
- ✔ **BLEU Score Evaluation** for assessing caption quality  
- ✔ **Hyperparameter Tuning** (learning rate, batch size, dropout)  

## Dataset Used
- 📁 **Flickr30k** (Primary dataset)  
- 📁 **Flickr8k** (Alternative dataset)  
- 📁 **Tiny ImageNet-200** (For additional training)  

## Installation

### Prerequisites
- Python 3.8+  
- TensorFlow / Keras  
- OpenCV  
- NLTK  

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/image-caption-generator.git
   cd image-caption-generator
   ```
2. Install dependencies
   ```
   pip install -r requirements.txt
    ```
Model Architecture
CNN (VGG16) → Extracts image features

Embedding Layer → Maps words to vectors

LSTM → Generates captions from features

Dense Layers → Final caption output
   
