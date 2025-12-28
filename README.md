# Car Body Type Classification

A deep learning project that classifies car images into 5 body types using Convolutional Neural Networks (CNN) built with TensorFlow/Keras.

## 🚗 Classification Categories

- **Coupe**
- **Pickup**
- **Sedan**
- **SUV**
- **Van**

## 📁 Project Structure

```
car-body-type-classification/
├── categorize_data.ipynb   # Data organization and preprocessing
├── model.ipynb             # CNN model training
├── keras_tuner.ipynb       # Hyperparameter optimization
├── results/                # Training results and sample predictions
└── README.md
```

## 🛠️ Technologies

- **Python 3.11**
- **TensorFlow / Keras** - Deep learning framework
- **Keras Tuner** - Hyperparameter optimization
- **NumPy** - Numerical operations

## 🏗️ Model Architecture

A Sequential CNN model with the following layers:

| Layer | Configuration |
|-------|--------------|
| Conv2D (1) | 48 filters, 3x3 kernel, ReLU |
| MaxPooling2D | 2x2 pool size |
| Conv2D (2) | 96 filters, 3x3 kernel, ReLU |
| MaxPooling2D | 2x2 pool size |
| Conv2D (3) | 128 filters, 3x3 kernel, ReLU |
| MaxPooling2D | 2x2 pool size |
| GlobalAveragePooling2D | - |
| Dense | 384 units, ReLU |
| Output | 5 units, Softmax |

## 📊 Data Preprocessing

- **Image Size**: 224x224 pixels
- **Data Augmentation**:
  - Rescaling (1./255)
  - Shear transformations (0.2)
  - Zoom transformations (0.2)
  - Horizontal flips
- **Validation Split**: 20%

## 🚀 Getting Started

### Prerequisites

```bash
pip install tensorflow keras-tuner numpy
```

### Usage

1. **Organize your data**: Run `categorize_data.ipynb` to organize images into class folders
2. **Train the model**: Execute `model.ipynb` to train the CNN
3. **Optimize hyperparameters** (optional): Use `keras_tuner.ipynb` for hyperparameter tuning

## 📈 Results

The model achieves classification across all 5 car body types. Training results and sample predictions are available in the `results/` directory.

![Training Accuracy](results/accuracy-val-accuracy%20graph.png)

## 📝 License

This project is open source and available for educational purposes.
