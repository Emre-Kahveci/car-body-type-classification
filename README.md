<div align="center">

  <a href="">![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)</a>

</div>

<p align="center"><img src="https://socialify.git.ci/Emre-Kahveci/car-body-type-classification/image?font=Rokkitt&language=1&name=1&pattern=Solid&theme=Dark"></p>

<p id="description">Code written to train logistic regression, XGB, Random Forest, SVM, GaussianNB, KNN algorithms for the bughunter dataset

### **Data preprocessing and augmentation**
 - rescale=1./255
 - shear_range=0.2
 - zoom_range=0.2
 - horizontal_flip=True

### **CNN algorithm layer structure**

 - **1. Convolutional Layer**
   - Conv2D -> filters=48 (3, 3), activation=relu
   - MaxPooling2D
 - **2. Convolutional Layer**
   - Conv2D -> filters=128 (3, 3), activation=relu
   - MaxPooling2D
 - **3. Convolutional Layer**
   - Conv2D -> filters=96 (3, 3), activation=relu
   - MaxPooling2D
 - **Global Average Pooling 2D**
 - **Fully connected Layer (Dense Layer)**
   - Dense -> units=384 activation=relu
 - **Output Layer**
   - Dense -> units=len(class_indices) activation=softmax
 - **Compile Model**
   - Compile -> optimizer=Adam, loss='categorical_crossentropy', metrics='accuracy'

Link to download the dataset: [dataset link](https://universe.roboflow.com/ana-lowela-l--lucas/vehicle-classification-sgcum)

  ### **Result Graphs**
  **Line chart**
  ![line-chart](https://github.com/Emre-Kahveci/car-body-type-classification/blob/7ab5ed4d43f63c4d144eafc9ad4aaeac9d332897/results/accuracy-val-accuracy%20graph.png)

</p>
