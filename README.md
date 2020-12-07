# Digital Recognizer
Python Jupyter Notebook with Convolutional Neural Network digit recognizer implemented in Keras. 

Part of the [Kaggle](https://www.kaggle.com/c/digit-recognizer) competition.

Submitted [Kernel](https://www.kaggle.com/anastasiiablyzniuk/digital-recognizer-cnn?scriptVersionId=48741453) with 0.99025 score.

# Data
Dataset: [MNIST Handwritten digits](https://www.kaggle.com/c/digit-recognizer/data)

Description: Classification of handwritten digits, 10 classes (0-9).

Training: 37.8k (0.9) images

Validation: 4.2k (0.1) images

Testing: 28k images

# Model
```
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d (Conv2D)              (None, 26, 26, 32)        320       
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 24, 24, 32)        9248      
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 12, 12, 32)        0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 10, 10, 64)        18496     
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 8, 8, 64)          36928     
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 4, 4, 64)          0         
_________________________________________________________________
flatten (Flatten)            (None, 1024)              0         
_________________________________________________________________
dense (Dense)                (None, 512)               524800    
_________________________________________________________________
dropout (Dropout)            (None, 512)               0         
_________________________________________________________________
dense_1 (Dense)              (None, 256)               131328    
_________________________________________________________________
dense_2 (Dense)              (None, 10)                2570      
=================================================================
Total params: 723,690
Trainable params: 723,690
Non-trainable params: 0
_________________________________________________________________
```

# Results
Kaggle score: 0.99025
