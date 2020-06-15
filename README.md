# Pneumonia Detection using Pediatric Chest X-Ray Images

## Overview
This study proposes the AI framework for diagnosis of pediatric pneumonia using chest X-ray images. We constructed a convolutional neural network model from scratch to extract features from a given chest X-ray image and classify it to determine if a child is infected with pneumonia.

We deployed data augmentation algorithms and used Transfer Learning approaches to improve the validation and classification accuracy of the CNN model and achieved remarkable Recall (99.23%) and F1 Score (93.08%) under different Classification setup, that are currently better and robust than State-of-the-Art results available. Our study aims to ultimately aid in expediting the diagnosis and referral of these treatable conditions, thereby facilitating earlier diagnosis, resulting in improved clinical outcomes.


## Dependencies
Tensorflow
Keras

## Dataset
Chest X-Ray Images - Pneumonia [https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia]

## CNN Architecture

![alt text](https://github.com/KarthikeyaR/pneumonia-detection/blob/master/model-plots/model-arch-ConvNet.PNG?raw=true)

## Results

### Normal vs Pneumonia Classification

|   Models  | Precision | Recall | Accuracy | F1 Score | AUC |
|:---------:|:---------:|:------:|:--------:|:--------:|:---:|
|   VGG16   |   87.55   |  99.23 |   90.71  |   93.02  |  88 |
| Inception |   87.27   |  98.46 |   90.06  |   92.53  |  87 |
|  Densenet |   90.77   |  95.89 |   91.34  |   93.26  |  90 |
|   Resnet  |   92.95   |  95.64 |   92.95  |   94.43  |  92 |
|    CNN    |   89.76   |  96.66 |   91.03  |   93.08  |  91 |

![alt text](https://github.com/KarthikeyaR/pneumonia-detection/blob/master/model-plots/normal-accuracy.PNG?raw=true)



### Bacterial vs. Viral Pneumonia Classification

|   Models  | Precision | Recall | Accuracy | F1 Score |  AUC |
|:---------:|:---------:|:------:|:--------:|:--------:|:----:|
|   VGG16   |    100    |  66.89 |   87.43  |   80.16  | 0.83 |
| Inception |   87.27   |  98.46 |   90.06  |   92.53  | 0.87 |
|  Densenet |   89.47   |  57.43 |  81.282  |  69.958  | 0.77 |
|   Resnet  |   86.98   |  85.81 |   89.74  |   86.39  | 0.89 |
|    CNN    |   94.736  |  72.97 |  88.205  |   82.44  | 0.85 |

![alt text](https://github.com/KarthikeyaR/pneumonia-detection/blob/master/model-plots/pneumonia-accuracy.PNG?raw=true)
