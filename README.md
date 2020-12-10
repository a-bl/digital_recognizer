# Digital Recognizer
Python Jupyter Notebook with Convolutional Neural Network digit recognizer implemented in Keras. 

Part of the [Kaggle](https://www.kaggle.com/c/digit-recognizer) competition.

Submitted [Kernel](https://www.kaggle.com/anastasiiablyzniuk/digital-recognizer-cnn) with 0.99728 score.

# Data
Dataset: [MNIST Handwritten digits](https://www.kaggle.com/c/digit-recognizer/data)

Description: Classification of handwritten digits, 10 classes (0-9).

Training: 60k images

Validation: 10k images

Testing: 28k images

# Model
```
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d (Conv2D)              (None, 28, 28, 32)        832       
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 28, 28, 32)        25632     
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 14, 14, 32)        0         
_________________________________________________________________
dropout (Dropout)            (None, 14, 14, 32)        0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 14, 14, 64)        18496     
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 14, 14, 64)        36928     
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 7, 7, 64)          0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 7, 7, 64)          0         
_________________________________________________________________
flatten (Flatten)            (None, 3136)              0         
_________________________________________________________________
dense (Dense)                (None, 256)               803072    
_________________________________________________________________
dropout_2 (Dropout)          (None, 256)               0         
_________________________________________________________________
dense_1 (Dense)              (None, 10)                2570      
=================================================================
Total params: 887,530
Trainable params: 887,530
Non-trainable params: 0
_________________________________________________________________
```

# Loss and accuracy curves
![](/images/loss_and_accuracy_curves.PNG)

# Confusion matrix
![](/images/confusion_matrix.PNG)

# Results
Kaggle score: 0.99728
