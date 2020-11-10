# Dogs Breed Classification

The goal of this task is to develop an algorithm to learn to classify images containing objects of the same category into specific sub-categories, i.e. specific dog breeds.

## Dataset


The Stanford Dogs dataset contains images of 120 breeds of dogs from around the world. This dataset has been built using images and annotation from ImageNet for the task of fine-grained image categorization. Contents of this dataset:

* Number of categories: 120
* Number of images: 20,580
* Annotations: Class labels, Bounding boxes

#### Dataset Reference

##### Primary:
  Aditya Khosla, Nityananda Jayadevaprakash, Bangpeng Yao and Li Fei-Fei. Novel dataset for Fine-Grained Image Categorization. First Workshop on Fine-Grained Visual Categorization (FGVC), IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2011.

##### Secondary:
  J. Deng, W. Dong, R. Socher, L.-J. Li, K. Li and L. Fei-Fei, ImageNet: A Large-Scale Hierarchical Image Database. IEEE Computer Vision and Pattern Recognition (CVPR), 2009.
  
#### Baseline Results
This section contains baseline results on two tasks:

* Mean Accuracy: The number of training images per class is varied from 1 to 100.

* Comparison of Accuracy per Class: The accuracy of each class is compared for 15 and 100 training images per class.

![out1](https://github.com/Gkontopodis/Image-classification---Stanford-dogs/blob/main/mean_accuracy.png)

#### Experimental Setting
All of the experiments use image regions from the bounding box only for both training and testing.

The remaining parameters are set to the following values:

* Type of SIFT descriptors: Grayscale
* SIFT patch sizes: 8, 10, 14, 18, 22, 26, 30
* SIFT grid spacing: 4 pixels
* Spatial pyramid: 1*1+2*2+4*4 (3 levels)
* Dictionary Size: 256
* Kernel: histogram intersection kernel

![out2](https://github.com/Gkontopodis/Image-classification---Stanford-dogs/blob/main/bar_graph_small.jpg)

#### Source: http://vision.stanford.edu/aditya86/ImageNetDogs/

## Packages

The script is composed in Python and it can be executed from the command line. Executing the tool requires the support of Python 3. In addition, the following libraries must be installed locally:

* Keras
* Split_folders
* ImageDataGenerator from keras.preprocessing.image
* Sequential from keras.models
* Dense, Dropout, Flatten from keras.layers 
* Conv2D, MaxPooling2D from keras.layers 
* models from keras 
* layers from keras 
* vgg16 from keras.applications.vgg16 
* optimizers from keras 
* plot_model from keras.utils
* load_model from keras.models
* xception from keras.applications.xception 
* to_categorical from keras.utils.np_utils 
* confusion_matrix from sklearn.metrics 
* load_model from keras.models 
* matplotlib.pyplot
* itertools
* sklearn.metrics
* numpy
* pandas
