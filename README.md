# 🏏 Generative Cricket Commentary Bot

An automated sports commentary system that uses Deep Learning to analyze cricket shots and generate play-by-play audio commentary.

## 🚀 Features
* **Image Understanding:** Uses **ViT (Vision Transformer)** to extract features from cricket images.
* **Caption Generation:** Uses **GPT-2** to generate context-aware commentary (e.g., "A glorious cover drive").
* **Shot Classification:** Distinguishes between similar shots (Cover Drive vs. Straight Drive) using **CLIP**.
* **Audio Output:** Converts the generated text into spoken commentary using **gTTS** with a British accent.

## 🛠️ Tech Stack
* **Python** (PyTorch, Transformers)
* **Models:** ViT-GPT2 Image Captioning, OpenAI CLIP
* **Interface:** Gradio
* **Dataset:** [Cricket Shot Dataset](https://www.kaggle.com/datasets/aneesh10/cricket-shot-dataset)

## 📂 Project Structure
* `Train_Model.ipynb`: The complete training pipeline. Handles data augmentation, fine-tuning ViT-GPT2, and saving the model to Drive.
* `Cricket.ipynb`: The inference app. Loads the saved model and runs a Gradio web interface for users to test images.

## ⚡ How to Run
1.  Open `Train_Model.ipynb` in Google Colab to fine-tune the model on your dataset.
2.  Once trained, run `Cricket.ipynb`, point it to your saved model path, and use the GUI to generate commentary.

## 👨‍💻 Author
* **Huzaifa** - BSCS Student at Sukkur IBA
