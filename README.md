# dog_breeds_classification
https://www.kaggle.com/c/dog-breed-identification

split the training data downloaded from Kaggle into training and testing data (0.8: 0.2)

**Stage 1**

Manually preprocessed the images to meet the requirement of VGG16 transfer learning. However, bottleneck features extracted this way together with the two Dense layer, one Dropout layer, one GlobalAveragePooling layer classifier only gives a testing accuracy of [8.0196%](https://github.com/yueying-teng/dog_breeds_classification/blob/master/transfer_learning_hand.ipynb)

Tried to extract bottleneck features using preprocess_input from keras.applications.vgg19, with the same classifier as that in VGG16 transfer learning, VGG19 transfer learning gives as testing accuracy of [66.1614%](https://github.com/yueying-teng/dog_breeds_classification/blob/master/transfer_learning%26preprocess_input.ipynb) 

**Stage 2**

Fine tuning 
