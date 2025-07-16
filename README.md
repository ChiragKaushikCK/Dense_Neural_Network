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
    <img src="https://placehold.co/600x200/6200EE/FFFFFF?text=Fashion+MNIST+DNN" alt="Fashion MNIST DNN Banner" style="border-radius: 15px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);">
  </a>
  <br>
  🧠 Dense Neural Network for Fashion MNIST 👗
  <br>
</h1>

<p align="center" style="font-size: 1.2em; color: #555; max-width: 800px; margin: 0 auto; line-height: 1.6;">
Dive into the world of deep learning with this **Dense Neural Network** (DNN) project! This Jupyter Notebook demonstrates how to build, train, and evaluate a simple yet effective feed-forward neural network for classifying images from the <a href="https://github.com/zalandoresearch/fashion-mnist" style="color: #6200EE; text-decoration: none;">Fashion MNIST dataset</a>. Perfect for beginners to understand the fundamentals of neural networks and image classification! 🚀
</p>

<br>

<details style="background-color: #F3E5F5; border-left: 5px solid #6200EE; padding: 15px; border-radius: 8px; margin: 20px auto; max-width: 700px; box-shadow: 0 2px 10px rgba(0,0,0,0.1);">
  <summary style="font-size: 1.3em; font-weight: bold; color: #333; cursor: pointer;">Table of Contents</summary>
  <ol style="list-style-type: decimal; padding-left: 25px; line-height: 1.8;">
    <li><a href="#about-the-project" style="color: #6200EE; text-decoration: none;">📚 About The Project</a></li>
    <li><a href="#dataset" style="color: #6200EE; text-decoration: none;">👗 Dataset</a></li>
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
  This project focuses on building and training a **Dense Neural Network (DNN)**, also known as a Feed-forward Neural Network or Multi-Layer Perceptron (MLP), to classify images from the Fashion MNIST dataset. It serves as a practical introduction to:
</p>
<ul style="list-style-type: none; padding: 0; font-size: 1.1em; color: #444;">
  <li style="margin-bottom: 10px; background-color: #EDE7F6; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">Data Loading & Preprocessing:</strong> Handling image data, normalization, and flattening.
  </li>
  <li style="margin-bottom: 10px; background-color: #EDE7F6; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">Model Definition:</strong> Stacking `Dense` layers using Keras's Sequential API.
  </li>
  <li style="margin-bottom: 10px; background-color: #EDE7F6; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">Model Compilation & Training:</strong> Setting up the optimizer, loss function, and metrics, then fitting the model to data.
  </li>
  <li style="margin-bottom: 10px; background-color: #EDE7F6; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">Evaluation & Prediction:</strong> Assessing model performance and making new predictions.
  </li>
  <li style="margin-bottom: 10px; background-color: #EDE7F6; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">Visualization:</strong> Plotting training history and example predictions.
  </li>
</ul>

---

<h2 id="dataset" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  👗 Dataset
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
The <strong style="color: #6200EE;">Fashion MNIST</strong> dataset is used in this project. It is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes of fashion items (e.g., T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot). It serves as a direct drop-in replacement for the original MNIST dataset for benchmarking machine learning algorithms.
</p>

---

<h2 id="model-architecture" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
🏗️ Model Architecture
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  The Dense Neural Network designed for this task is a sequential model comprising several fully connected layers.
</p>
<div style="background-color: #FFFDE7; border: 1px solid #FFD700; padding: 15px; border-radius: 8px; margin: 20px auto; max-width: 600px; box-shadow: 0 2px 10px rgba(0,0,0,0.1);">
  <h3 style="color: #6200EE; font-size: 1.8em; margin-top: 0;">Layers:</h3>
  <ul style="list-style-type: none; padding: 0; font-size: 1.1em; color: #444;">
    <li style="margin-bottom: 10px;"><strong style="color: #6200EE;">Input Layer:</strong> Flattens the 28x28 image into a 784-dimensional vector.</li>
    <li style="margin-bottom: 10px;"><strong style="color: #6200EE;">Hidden Layers:</strong> Multiple `Dense` layers with `relu` activation functions, responsible for learning complex patterns.</li>
    <li style="margin-bottom: 10px;"><strong style="color: #6200EE;">Output Layer:</strong> A `Dense` layer with `softmax` activation, producing probability distributions over the 10 fashion classes.</li>
  </ul>
  <h3 style="color: #6200EE; font-size: 1.8em; margin-top: 20px;">Compilation:</h3>
  <ul style="list-style-type: none; padding: 0; font-size: 1.1em; color: #444;">
    <li style="margin-bottom: 10px;"><strong style="color: #6200EE;">Optimizer:</strong> Adam (Adaptive Moment Estimation) - an efficient stochastic optimization algorithm.</li>
    <li style="margin-bottom: 10px;"><strong style="color: #6200EE;">Loss Function:</strong> Sparse Categorical Crossentropy - suitable for integer-encoded labels in multi-class classification.</li>
    <li style="margin-bottom: 10px;"><strong style="color: #6200EE;">Metrics:</strong> Accuracy - measures the proportion of correctly classified images.</li>
  </ul>
</div>

---

<h2 id="features" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  🎯 Features
</h2>
<ul style="list-style-type: none; padding: 0; font-size: 1.1em; color: #444;">
  <li style="margin-bottom: 15px; background-color: #F8E6FD; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">🚀 End-to-End Workflow:</strong> Covers data loading, preprocessing, model building, training, evaluation, and prediction.
  </li>
  <li style="margin-bottom: 15px; background-color: #F8E6FD; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">📊 Performance Visualization:</strong> Plots training and validation accuracy/loss over epochs to monitor model performance.
  </li>
  <li style="margin-bottom: 15px; background-color: #F8E6FD; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">🔍 Prediction Samples:</strong> Displays sample images with their true and predicted labels, highlighting correct and incorrect classifications.
  </li>
  <li style="margin-bottom: 15px; background-color: #F8E6FD; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #6200EE;">✍️ Clear & Concise Code:</strong> Well-structured and commented code for easy understanding and modification.
  </li>
</ul>

---

<h2 id="prerequisites" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  🛠️ Prerequisites
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  To run this project, ensure you have the following installed:
</p>
<ul style="list-style-type: disc; padding-left: 20px; font-size: 1.1em; color: #444;">
  <li><strong style="color: #6200EE;">Python 3.x</strong></li>
  <li><strong style="color: #6200EE;">Jupyter Notebook</strong> (or JupyterLab, Google Colab)</li>
  <li>Required Libraries:
    <pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code>pip install tensorflow keras matplotlib</code></pre>
  </li>
</ul>

---

<h2 id="how-to-run" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  📋 How to Run
</h2>
<ol style="list-style-type: decimal; padding-left: 20px; font-size: 1.1em; color: #444; line-height: 1.8;">
  <li style="margin-bottom: 10px;">
    <strong style="color: #6200EE;">Download the Notebook:</strong>
    <p style="margin-top: 5px;">Download <code>Dense_Neural_Network.ipynb</code> from this repository.</p>
    <p style="margin-top: 5px;">Alternatively, open it directly in <a href="https://colab.research.google.com/" style="color: #6200EE; text-decoration: none;">Google Colab</a> for a zero-setup experience.</p>
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #6200EE;">Install Dependencies:</strong>
    <pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code>pip install tensorflow keras matplotlib</code></pre>
  </li>
  <li style="margin-bottom: 10px;">
    <strong style="color: #6200EE;">Run the Notebook:</strong>
    <p style="margin-top: 5px;">Open <code>Dense_Neural_Network.ipynb</code> in Jupyter or Colab.</p>
    <p style="margin-top: 5px;">Execute each cell sequentially to load data, build, train, and evaluate the DNN!</p>
  </li>
</ol>

---

<h2 id="example-output" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  📊 Example Output
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  After training, the notebook will display a summary of the model's performance during training (accuracy and loss plots) and show predictions on test images.
</p>

<h3 style="color: #6200EE; font-size: 1.8em; margin-top: 25px;">Training History Plots:</h3>
<div style="text-align: center; background-color: #F8F8F8; padding: 15px; border-radius: 10px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin-top: 20px; display: flex; flex-wrap: wrap; justify-content: center; gap: 20px;">
  <div style="flex: 1 1 45%; min-width: 300px;">
    <h4 style="color: #4CAF50; font-size: 1.3em; margin-bottom: 10px;">Model Accuracy:</h4>
    <img src="https://placehold.co/400x250/C8E6C9/333333?text=Accuracy+Plot" alt="Accuracy Plot Placeholder" style="width: 100%; height: auto; border-radius: 8px; border: 1px solid #ddd;">
    <p style="font-size: 0.9em; color: #666; margin-top: 10px;">Accuracy progression during training.</p>
  </div>
  <div style="flex: 1 1 45%; min-width: 300px;">
    <h4 style="color: #FF7043; font-size: 1.3em; margin-bottom: 10px;">Model Loss:</h4>
    <img src="https://placehold.co/400x250/FFCCBC/333333?text=Loss+Plot" alt="Loss Plot Placeholder" style="width: 100%; height: auto; border-radius: 8px; border: 1px solid #ddd;">
    <p style="font-size: 0.9em; color: #666; margin-top: 10px;">Loss reduction during training.</p>
  </div>
</div>

<h3 style="color: #6200EE; font-size: 1.8em; margin-top: 25px;">Sample Predictions:</h3>
<div style="text-align: center; background-color: #F8F8F8; padding: 15px; border-radius: 10px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin-top: 20px;">
  <img src="https://placehold.co/600x200/CFD8DC/333333?text=Fashion+MNIST+Predictions" alt="Fashion MNIST Predictions Placeholder" style="width: 100%; max-width: 600px; height: auto; border-radius: 8px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #666; margin-top: 10px;">
    Visual examples of predictions on test images, showing original image, predicted label, and true label.
  </p>
</div>

---

<h2 id="code-breakdown" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  🧠 Code Breakdown
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  Key parts of the notebook's code structure:
</p>

<h3 style="color: #6200EE; font-size: 1.8em; margin-top: 25px;">Data Loading and Preprocessing:</h3>
<pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code><span style="color: #569CD6;">import</span> <span style="color: #9CDCFE;">tensorflow</span> <span style="color: #C586C0;">as</span> <span style="color: #9CDCFE;">tf</span>
<span style="color: #569CD6;">from</span> <span style="color: #9CDCFE;">tensorflow</span> <span style="color: #C586C0;">import</span> <span style="color: #9CDCFE;">keras</span>
<span style="color: #569CD6;">import</span> <span style="color: #9CDCFE;">matplotlib.pyplot</span> <span style="color: #C586C0;">as</span> <span style="color: #9CDCFE;">plt</span>

(<span style="color: #9CDCFE;">train_images</span>, <span style="color: #9CDCFE;">train_labels</span>), (<span style="color: #9CDCFE;">test_images</span>, <span style="color: #9CDCFE;">test_labels</span>) <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">keras.datasets.fashion_mnist.load_data</span>()

<span style="color: #9CDCFE;">train_images</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">train_images</span> <span style="color: #CE9178;">/</span> <span style="color: #B5CEA8;">255.0</span>
<span style="color: #9CDCFE;">test_images</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">test_images</span> <span style="color: #CE9178;">/</span> <span style="color: #B5CEA8;">255.0</span></code></pre>

<h3 style="color: #6200EE; font-size: 1.8em; margin-top: 25px;">Model Definition, Compilation, and Training:</h3>
<pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code><span style="color: #9CDCFE;">model</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">keras.Sequential</span>([
    <span style="color: #9CDCFE;">keras.layers.Flatten</span>(<span style="color: #9CDCFE;">input_shape</span><span style="color: #CE9178;">=</span>(<span style="color: #B5CEA8;">28</span>, <span style="color: #B5CEA8;">28</span>)),
    <span style="color: #9CDCFE;">keras.layers.Dense</span>(<span style="color: #B5CEA8;">128</span>, <span style="color: #9CDCFE;">activation</span><span style="color: #CE9178;">=</span><span style="color: #CE9178;">'relu'</span>),
    <span style="color: #9CDCFE;">keras.layers.Dense</span>(<span style="color: #B5CEA8;">10</span>, <span style="color: #9CDCFE;">activation</span><span style="color: #CE9178;">=</span><span style="color: #CE9178;">'softmax'</span>)
])

<span style="color: #9CDCFE;">model.compile</span>(<span style="color: #9CDCFE;">optimizer</span><span style="color: #CE9178;">=</span><span style="color: #CE9178;">'adam'</span>,
              <span style="color: #9CDCFE;">loss</span><span style="color: #CE9178;">=</span><span style="color: #CE9178;">'sparse_categorical_crossentropy'</span>,
              <span style="color: #9CDCFE;">metrics</span><span style="color: #CE9178;">=</span>[<span style="color: #CE9178;">'accuracy'</span>])

<span style="color: #9CDCFE;">history</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">model.fit</span>(<span style="color: #9CDCFE;">train_images</span>, <span style="color: #9CDCFE;">train_labels</span>, <span style="color: #9CDCFE;">epochs</span><span style="color: #CE9178;">=</span><span style="color: #B5CEA8;">5</span>, <span style="color: #9CDCFE;">validation_split</span><span style="color: #CE9178;">=</span><span style="color: #B5CEA8;">0.1</span>)</code></pre>

<h3 style="color: #6200EE; font-size: 1.8em; margin-top: 25px;">Model Evaluation and Prediction:</h3>
<pre style="background-color: #2D2D2D; color: #E0E0E0; padding: 15px; border-radius: 8px; overflow-x: auto; font-family: 'Fira Code', monospace; font-size: 0.95em; box-shadow: 0 2px 10px rgba(0,0,0,0.15);"><code><span style="color: #9CDCFE;">test_loss</span>, <span style="color: #9CDCFE;">test_acc</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">model.evaluate</span>(<span style="color: #9CDCFE;">test_images</span>, <span style="color: #9CDCFE;">test_labels</span>, <span style="color: #9CDCFE;">verbose</span><span style="color: #CE9178;">=</span><span style="color: #B5CEA8;">2</span>)
<span style="color: #569CD6;">print</span>(<span style="color: #CE9178;">f"Test accuracy: {test_acc}"</span>)

<span style="color: #9CDCFE;">predictions</span> <span style="color: #CE9178;">=</span> <span style="color: #9CDCFE;">model.predict</span>(<span style="color: #9CDCFE;">test_images</span>)</code></pre>

---

<h2 id="contribute" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  🤝 Contribute
</h2>
<p align="center" style="font-size: 1.2em; color: #555; max-width: 800px; margin: 0 auto; line-height: 1.6;">
  Contributions are always welcome! If you have ideas for improvements, new features (e.g., adding more layers, different activation functions, or other datasets), or just want to fix a bug, please feel free to open an issue or submit a pull request. Let’s build better neural networks together! 💡
</p>
<p align="center" style="font-size: 1.2em; color: #555; max-width: 800px; margin: 15px auto 0; line-height: 1.6;">
  Star this repo if you find it helpful! ⭐
</p>
<p align="center" style="font-size: 1em; color: #777; margin-top: 30px;">
  Created with 💖 by Chirag
</p>

