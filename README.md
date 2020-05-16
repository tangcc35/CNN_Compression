# Canned_Pineapple Data-2040-Final-Project  ![](https://img.shields.io/badge/python-3.7+-pink.svg) ![](https://img.shields.io/badge/tensorflow-2.x-important.svg) 

***Group Member: [Guanzhong Chen](https://github.com/frank07080), [Shiyu Liu](https://github.com/shiyuliu1), [Guansu Niu](https://github.com/francesniu), [Cangcheng Tang](https://github.com/tangcc35), Zhi Wang***   


*Medium: [Initial Blog Post](https://bit.ly/3fTLp5h), [Midway Blog Post](https://bit.ly/2T534Ny), [Final Blog Post](https://bit.ly/CNN_Compression)*  
*[Project on Next Journal](https://bit.ly/NJ_CNN_Compression)*  
*[Screencast](https://youtu.be/rAFYVpmmK1Q)*  

## An Achromatic Approach on Compressing CNN Filters Using Pattern-specific Receptive Fields

### Project Motivation & Goal
In studies of image recognition, there are many gray-scale pictures, such as chest radiographs. Currently, the idea behind training those images is to apply models that are essentially designed for training color pictures, such as ResNet and DenseNet. This can lead to many redundant parameters during the process. Therefore, this project aimed to discover a methodology to modify the models trained on colored images and to apply them to gray-scale images.

### SRC
Merging and clustering notebooks are called `DenseNet_merge_first_layer.ipynb` for merging the first layer and `DenseNet_merge_multipule_layer.ipynb` for merge the first two layers.  

### Dataset
This project used CIFAR-10 dataset which you probably known already. It consists of 60,000 32 by 32 pixels color images in 10 classes, with 6,000 images per class. Also The training to testing ratio is 5:1.

### Results  
| Model                    | Image Type       | Val Accuracy | Number of Parameters |
|--------------------------|------------------|--------------|----------------------|
| Color Model              | Color Images     | 91.16%       | 995,230              |
| Color Model              | Grayscale Images | 83.20%       | 995,230              |
| Modified 1st Layer       | Grayscale Images | 85.43%       | 964,237              |
| Modified 1st & 2nd Layer | Grayscale Images | 84.83%       | 950,046              |
