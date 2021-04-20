# Autoencoder Pretraining

One of the main challenges with using deep learning to diagnose Melanoma is the lack of images. Specifically, the lack of Melanoma images. There are many images in the non-Melanoma category, but to reduce the imbalance in the dataset, I undersampled (left out) a large number of images from training. 

The code in ```Autoencoder Pretraining.ipynb``` shows an autoencoder which is trained on about 30,000 images without labels, then the earlier weights are copied into the actual classification models. The process overview is outlined in the image below. 
![](unsupervised_pretraining.png)
> Image Source: Géron, A. (2017). Hands-on machine learning with Scikit-Learn, Keras, and TensorFlow concepts, tools, and techniques to build intelligentsystems O'Reilly Media Paperback .