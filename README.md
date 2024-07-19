# Caltech UCSD Bird 200 Classification
 
- This repo contains code to classify 200 species of birds using TensorFlow.
- The dataset consisting of 6033 images was split in a 50-50 train-test split ratio.
- The overall validation accuracy achieved was 66.53%.
- Dataset Files:
  - [images](https://drive.usercontent.google.com/download?id=1jobzMyDXVHE6dSRCqaS-mS1k5Fd8vYwr&export=download)
  - [List of splits](https://drive.google.com/uc?id=1mts78-igyUQRr3wycF9agLM-NSIASzFQ&export=download)
- The model architecture consists of:
  - An input layer with a shape of (400, 400, 3).
  - A data augmentation layer.
  - The base ResNet152V2 model.
  - A global average pooling layer.
  - A dense layer with 512 units, ReLU activation, L2 regularization, and dropout for regularization to prevent overfitting.
  - An output layer with softmax activation.
- The model was first trained on 20 epochs for feature extraction using the RMSprop optimizer.
- It was then trained on another 40 epochs for fine-tuning with Adam optimizer.
- The [visualisations](https://github.com/AbdulRahmaan03/Caltech-UCSD-Birds-200-Classification/tree/main/Visualisations) folder consists of images representing the model performance.
