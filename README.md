# Image-Text-Recognition
Text Recognition in Natural Images in Python

The idea is to be able to get as input an image (i.e. picture taken with phone) from a user and process it in order to return the text contained in it.

The file you should look at first is main.py. This file instantiates classes and calls appropriate classes methods.

Class UserData (contained in userimageski.py) is instantiated passing to the constructor the image filename to be processed.

Class Cifar (contained in cifar.py) is instantiated passing a config file (with all the parameters) to the constructor. Specifically cifar-config.py, which is used in the merge-with-cifar method inside OcrData class in order to build the dataset to perform the text/no-text classification. The data mentioned inside cifar-config.py was too big to be uploaded on Github but it is available on CIFAR-10 Kaggle Competition.

Class OcrData (contained in data.py) is instantiated passing a config file (with all the parameters) to the constructor. Specifically ocr-config.py and text-config.py are both used in two different contextes. The first one is called to perform the machine learning pipeline on character images. The second one is called only once inside the merge-with-cifar method inside OcrData class in order to build the dataset to perform the text/no-text classification.


