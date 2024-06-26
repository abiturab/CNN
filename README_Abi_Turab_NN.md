# Melanoma Detection Assignment CNN
> The approach uses Convolutional Neural Network (CNN) to classify nine types of skin cancer from outlier lesions images.

# Problem Solving approach
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images.

Class	No. of Image
0	melanoma	438
1	seborrheic keratosis	77
2	nevus	357
3	actinic keratosis	114
4	dermatofibroma	95
5	basal cell carcinoma	376
6	squamous cell carcinoma	181
7	pigmented benign keratosis	462
8	vascular lesion	139

To overcome the issue of class imbalance, used a python package Augmentor (https://augmentor.readthedocs.io/en/master/) to add more samples across all classes so that none of the classes have very few samples

To achieve higher accuracy and results on the classification task, I have built custom CNN model.

### Rescalling Layer - To rescale an input in the [0, 255] range to be in the [0, 1] range.

### Convolutional Layer - Convolutional layers apply a convolution operation to the input, passing the result to the next layer. A convolution converts all the pixels in its receptive field into a single value. 

### Pooling Layer - Pooling layers are used to reduce the dimensions of the feature maps. Thus, it reduces the number of parameters to learn and the amount of computation performed in the network. The pooling layer summarises the features present in a region of the feature map generated by a convolution layer.

### Dropout Layer - The Dropout layer randomly sets input units to 0 with a frequency of rate at each step during training time, which helps prevent overfitting.

### Flatten Layer - Flattening is converting the data into a 1-dimensional array for inputting it to the next layer. We flatten the output of the convolutional layers to create a single long feature vector. And it is connected to the final classification model, which is called a fully-connected layer.

### Dense Layer - The dense layer is a neural network layer that is connected deeply, which means each neuron in the dense layer receives input from all neurons of its previous layer.

### Final Outcome:
Accuracy on training data has increased by using Augmentor library
In 50 epochs, Model has achieved 80% accuracy on train and validation sets.
The Model can be further improved by increasing number of epochs and tuning the hyperparameter.


## Contact
Created by abiturab - feel free to contact me!
