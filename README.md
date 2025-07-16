# Dense_Neural_Network on MNIST

<img width="141" height="113" alt="download" src="https://github.com/user-attachments/assets/016cc970-65e8-4a5a-9b8b-3286d5b58838" />

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow" />
  <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white" alt="Keras" />
  <img src="https://img.shields.io/badge/Matplotlib-EE6633?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
</div>

<h1 align="center" style="color: #6200EE; font-family: 'Segoe UI', sans-serif; font-size: 3.5em; text-shadow: 2px 2px 4px rgba(0,0,0,0.2);">
  <br>
  <a href="https://github.com/your-username/dense-neural-network">
    <img src="https://placehold.co/600x200/6200EE/FFFFFF?text=MNIST+Digits+DNN" alt="MNIST Digits DNN Banner" style="border-radius: 15px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);">
  </a>
  <br>
  🧠 Dense Neural Network for MNIST Digits ✍️
  <br>
</h1>

<p align="center" style="font-size: 1.2em; color: #555; max-width: 800px; margin: 0 auto; line-height: 1.6;">
  Dive into the world of deep learning with this **Dense Neural Network** (DNN) project! This Jupyter Notebook demonstrates how to build, train, and evaluate a simple yet effective feed-forward neural network for classifying handwritten digits from the <a href="http://yann.lecun.com/exdb/mnist/" style="color: #6200EE; text-decoration: none;">MNIST dataset</a>. Perfect for beginners to understand the fundamentals of neural networks and image classification! 🚀
</p>

<br>

<details style="background-color: #F3E5F5; border-left: 5px solid #6200EE; padding: 15px; border-radius: 8px; margin: 20px auto; max-width: 700px; box-shadow: 0 2px 10px rgba(0,0,0,0.1);">
  <summary style="font-size: 1.3em; font-weight: bold; color: #333; cursor: pointer;">Table of Contents</summary>
  <ol style="list-style-type: decimal; padding-left: 25px; line-height: 1.8;">
    <li><a href="#about-the-project" style="color: #6200EE; text-decoration: none;">📚 About The Project</a></li>
    <li><a href="#dataset" style="color: #6200EE; text-decoration: none;">🔢 Dataset</a></li>
    <li><a href="#model-architecture" style="color: #6200EE; text-decoration: none;">🏗️ Model Architecture</a></li>
    <li><a href="#features" style="color: #6200EE; text-decoration: none;">🎯 Features</a></li>
    <li><a href="#prerequisites" style="color: #6200EE; text-decoration: none;">🛠️ Prerequisites</a></li>
    <li><a href="#how-to-run" style="color: #6200EE; text-decoration: none;">📋 How to Run</a></li>
    <li><a href="#example-output" style="color: #6200EE; text-decoration: none;">📊 Example Output</a></li>
    <li><a href="#code-breakdown" style="color: #6200EE; text-decoration: none;">🧠 Code Breakdown</a></li>
    <li><a href="#contribute" style="color: #6200EE; text-decoration: none;">🤝 Contribute</a></li>
  </ol>
</details>

---

<h2 id="about-the-project" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  📚 About The Project
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  This project focuses on building and training a **Dense Neural Network (DNN)**, also known as a Feed-forward Neural Network or Multi-Layer Perceptron (MLP), to classify handwritten digits from the MNIST dataset. [cite: uploaded:Dense_Neural_Network.ipynb] It serves as a practical introduction to:
</p>
<ul style="list-style-type: none; padding: 0; font-size: 1.1em; color: #444;">
  <li style="margin-bottom: 10px; background-color: #EDE7F6; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">Data Loading & Preprocessing:</strong> Handling image d
