
# Image Caption Generator

## Problem Statement
The project aims to develop an Image Caption Generator using a **CNN** for feature extraction and an **LSTM** for text generation. The model is trained on the **Flickr8k** dataset to automatically generate descriptive captions for input images. 
## Dataset source 
 - **flicr8k dataset**
[https://www.kaggle.com/datasets/adityajn105/flickr8k](URL)
- **flicr30k dataset**
[https://www.kaggle.com/datasets/adityajn105/flickr30k](URL)
- **Tiny Imagenet dataset**
[https://www.kaggle.com/datasets/akash2sharma/tiny-imagenet](URL)




## Team Members
- **Shreyas** (CB.EN.U4CSE22154)  
- **Uma Mahesh** (CB.EN.U4CSE22534)  
- **Sathvik Reddy** (CB.EN.U4CSE22160)  
- **Hemanth Reddy** (CB.EN.U4CSE22558) 

## Dataset Used
- 📁 **Tiny ImageNet-200**  
- 📁 **Flickr30k**  
- 📁 **Flickr8k** 

## Preprocessing of Data
1. **Image Processing**  
   - Resize images to uniform dimensions.  
   - Convert to numerical arrays for CNN input.  
2. **Caption Processing**  
   - Tokenize captions and convert words to integer sequences.  
   - Pad sequences to a fixed length.  
   - Generate word mappings and embeddings to improve text representation. :contentReference[oaicite:6]{index=6}:contentReference[oaicite:7]{index=7}

## Model Architecture & Design
1. **CNN (VGG16)**  
   - Pretrained VGG16 extracts high-level image features.  
2. **Embedding Layer**  
   - Maps each word token to a dense vector representation.  
3. **LSTM Network**  
   - Generates captions based on extracted features and previous word inputs.  
4. **Dense Layers**  
   - Output layer predicts the next word in the sequence. :contentReference[oaicite:8]{index=8}:contentReference[oaicite:9]{index=9}

## Optimization & Hyperparameter Tuning
- **Optimizer:** Adam (and comparisons with SGD)  
- **Hyperparameters Tuned:**  
  - Learning rate  
  - Batch size  
  - Sequence length  
  - Dropout rate  
- Tuning performed by monitoring validation loss to avoid overfitting. :contentReference[oaicite:10]{index=10}:contentReference[oaicite:11]{index=11}

### Results & Evaluation
Model performance is evaluated using 
-BLEU
-RMSE
-ACCURACY
-LOSS
-MSE
 



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
   ````

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Download datasets (Tiny ImageNet-200, Flickr30k, Flickr8k) and place them in the `data/` directory.


* **Output:** A generated caption for the input image (e.g., *"A dog is playing in the park"*).

## Contributing

1. Fork the repository
2. Create a branch:

   ```bash
   git checkout -b feature-branch
   ```
3. Commit your changes:

   ```bash
   git commit -m "Description of feature"
   ```
4. Push to your branch:

   ```bash
   git push origin feature-branch
   ```
5. Open a Pull Request

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## Contact

📧 **Email:** [your-email@example.com](mailto:your-email@example.com)


⭐ Star the repo if you find it useful!
Happy Coding! 🚀

