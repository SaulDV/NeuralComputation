# Neural Computation

For this project we were tasked with the semantic segmentation of magnetic resonance (MR) images of the heart using deep learning.

***

## Instructions

In digital image processing and computer vision, semantic image segmentation is the
process of assigning a label to every pixel in an image such that pixels with the same label share
certain characteristics. This process can simplify and/or change the representation of an image into
something that is more meaningful and easier to analyze. 

### Figure 1.

![image](/Images/NCfig1.JPG)

Specifically, we are concerned with semantic image segmentation of cardiovascular MR (CMR)
images. CMR imaging is the gold standard for assessing cardiac chamber volume and mass for
many cardiovascular diseases. For decades, clinicians have been relying on manual segmentation
approaches to derive quantitative measures such as left ventricle volume, mass and ejection fraction.
However, manual expert segmentation is tedious, time-consuming and prone to subjective errors.
It becomes impractical when dealing with large-scale datasets. For this, the aim of this coursework
is to develop an automated methodology using a Convolutional Neural Network (CNN) that is capable
of segmenting a CMR image into four regions: the background, the left ventricle (LV), the right
ventricle (RV) and the myocardium (Myo). Figure 1 gives you an example of such a segmentation.

### Figure 2.

![image](/Images/NCfig2.JPG)

### Figure 3.

![image](/Images/NCfig3.JPG)

The dataset contains a totoal of 200 CMR images in a PNG format. We split the data into 50%
for training, 10% for validation and 40% for testing. For the training set, there are 100 CMR
images and 100 respective ground truth mask images. Figure 2 shows all images and their masks
in the training set. You should use the images and masks in this set to train your network. For
the validation set, there are 20 CMR images and 20 mask images, which look similar to those in
the training set. You should use this set to tune the hyperparameters (ie. CNN architectures, loss
functions, optimization algorithms, etc) of your method so as to maximize the overall performance.
For the test set, there are 80 CMR images but no ground truth masks are given. Figure 3 displays
all 80 test images. For the test set, we hold the ground truth masks. Your mission is to see how
accurately your method can segment these CMR images in the test set, by comparing
your segmentation masks with the ground truth masks we hold. Good luck!
