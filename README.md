# 🎨 RetroColor: Coloring Old Photographs Using Autoencoders

RetroColor is a deep learning-based web application that colorizes grayscale images using an autoencoder neural network. Built using Python, Flask, and TensorFlow/Keras, this project aims to breathe new life into old black-and-white photographs with the power of neural networks.

## 🚀 Features

- 🖤➡️🎨 Converts grayscale images to color
- 📂 Upload and preview images directly from your browser
- 🧠 Trained using CIFAR-10 dataset for demonstration
- 🌐 Lightweight Flask-based web app
- 🖼️ Autoencoder model trained for image colorization
- 📦 Easy-to-use interface and codebase for further development

---

## 🧠 How It Works

RetroColor uses a Convolutional Autoencoder trained on CIFAR-10 dataset images. The model learns the mapping between grayscale and RGB representations and can colorize new grayscale images with similar features.

**Autoencoder Architecture**:
- Encoder: Compresses the input grayscale image
- Decoder: Reconstructs the image in color (RGB)

---

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, Bootstrap (optional)
- **Backend**: Flask (Python)
- **Model**: Keras + TensorFlow (Autoencoder)
- **Dataset**: CIFAR-10 (Keras built-in)
- **Deployment**: (Optional) Flask or platforms like Render/Heroku/Colab

---

## 📁 Project Structure

retrocolor/
│
├── static/
│ └── styles.css
├── templates/
│ ├── index.html
│ └── result.html
├── uploads/
│ └── (uploaded grayscale images)
├── model/
│ └── autoencoder_model.h5
├── app.py
├── utils.py
├── train_model.py
└── README.md



## 🚧 Installation and Setup

### 1. Clone the repository

git clone https://github.com/Satyexe/RetroColor.git
cd retrocolor

### 2. Create a virtual environment (optional but recommended)

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

### 3. Install required packages

pip install -r requirements.txt

### 4. Train or load the model
To train the autoencoder model:


python train_model.py
Or use the pre-trained model (autoencoder_model.h5) if provided.

### 5. Run the Flask server

python app.py
Visit http://127.0.0.1:5000 in your browser.
