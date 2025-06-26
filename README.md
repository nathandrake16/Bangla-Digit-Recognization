# bangla-digit-recognization
An Efficient Deep Learning Model for Bangla Handwritten Digit Recognition
Dataset [BHand] : https://github.com/SaadatChowdhury/BHaND

README

The full form of BHaND is "Bengali Handwritten Numerals Dataset".

In this work, we have created a new dataset containing images of handwritten Bengali numerals. Our main goal was to make the dataset similar to MNIST, one of the most well-known datasets for English handwritten digits.

Similar to MNIST, we have collected 70,000 sample images of Bengali digits. Each image is 32×32 in size (MNIST images were 28×28). Everything else closely follows the structure of the MNIST dataset.

Basic Description

This dataset consists of 70,000 samples divided into three sets:

Training set: 50,000 samples

Validation set: 10,000 samples

Test set: 10,000 samples

Each row in these sets has two components: the first component is the image data, and the second component is the label. The label represents the Bengali digit (0 to 9) shown in the corresponding image. For example, the training set contains 50,000 rows, each with two parts: a 1024-dimensional image vector and an integer label.

All samples are in grayscale and normalized to the intensity range [0,1]. The pixel intensities were inverted so that black pixels have a value of 1 and white pixels have a value of 0. The images were then flattened into 1024-dimensional vectors (since 32×32=1024).

Finally, all samples were grouped together into a single pickle file using Python's cPickle serializer and compressed using the GZIP compression algorithm for faster transmission.