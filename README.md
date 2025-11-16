# CIFAR-10-Object-Recognition-Using-RESNET50
A complete deep-learning project that trains a ResNet50 model on the CIFAR-10 dataset, evaluates accuracy, predicts user-uploaded images

___________________________________________________________________________________________________________________________

🚀 Features

🔹 Transfer Learning using ResNet50 (ImageNet pretrained)

🔹 Achieves ~88–90% accuracy on CIFAR-10

🔹 Clean visualization: sample images, accuracy graph, prediction demo

🔹 Flask API for real-time image classification

🔹 Ready for deployment on Render / HuggingFace / Fly.io

🔹 Requirements file included

___________________________________________________________________________________________________________________________

📂 Dataset

This project uses the CIFAR-10 dataset by Alex Krizhevsky, published in the “Learning Multiple Layers of Features from Tiny Images” report.

🔗 Source

The dataset is available publicly through TensorFlow/Keras and can be loaded directly:

from tensorflow.keras.datasets import cifar10
(x_train, y_train), (x_test, y_test) = cifar10.load_data()

📦 Dataset Details
1) Total images: 60,000
2) Image size: 32 × 32 × 3
3) Training set: 50,000 images
4) Test set: 10,000 images
5) Number of classes: 10

| Label | Class      |
| ----- | ---------- |
| 0     | Airplane   |
| 1     | Automobile |
| 2     | Bird       |
| 3     | Cat        |
| 4     | Deer       |
| 5     | Dog        |
| 6     | Frog       |
| 7     | Horse      |
| 8     | Ship       |
| 9     | Truck      |



🛠 Preprocessing Applied

To prepare the images for ResNet50:
1) Resized all images to 224 × 224 × 3
2) Normalized pixel values to range 0–1
3) Labels kept as sparse integers
4) Implemented train/test split using default CIFAR-10 loader

📄 License

CIFAR-10 is available for research and educational purposes, distributed by the University of Toronto.


___________________________________________________________________________________________________________________________

🧠 Model Details

Backbone: ResNet50 (pretrained on ImageNet)

Input size: 224×224×3 (CIFAR images resized)

Optimizer: Adam

Loss: Sparse Categorical Crossentropy

Epochs: 10–20

Test Accuracy: ~88–90%
___________________________________________________________________________________________________________________________

🏋️ Training Notebook

Located in: Object_Recognition_Cifar_10.ipynb

The notebook includes:
1) Dataset loading
2) Preprocessing
3) Model creation
4) Training
5) Accuracy & loss graphs
6) Prediction
___________________________________________________________________________________________________________________________

🙌 Acknowledgements

1) CIFAR-10 dataset by Alex Krizhevsky
2) ResNet50 (He et al.)
3) TensorFlow / Keras
___________________________________________________________________________________________________________________________

⭐ Show Some Support
If you like this project, ⭐ star the repo!
   


