# Canned_Pineapple Data-2040-Final-Project  ![](https://img.shields.io/badge/python-3.7+-pink.svg)

***Group Member: Guanzhong Chen, Shiyu Liu, Guansu Niu, Cangcheng Tang, Zhi Wang***  
[Final Blog Post on Medium](https://bit.ly/CNN_Compression)  
[Project on Next Journal](https://bit.ly/NJ_CNN_Compression)  

## An Achromatic Approach on Compressing CNN Filters Using Pattern-specific Receptive Fields

### Project Motivation & Goal
In studies of image recognition, there are many gray-scale pictures, such as chest radiographs. Currently, the idea behind training those images is to apply models that are essentially designed for training color pictures, such as ResNet and DenseNet. This can lead to many redundant parameters during the process. Therefore, this project aimed to discover a methodology to modify the models trained on colored images and to apply them to gray-scale images.

### Dataset
This project used CIFAR-10 dataset which you probably known already. It consists of 60,000 32 by 32 pixels color images in 10 classes, with 6,000 images per class. Also The training to testing ratio is 5:1.
