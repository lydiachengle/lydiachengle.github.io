---
layout: post
Title: Final Project_Handwriting Recognition
---
Project Description and Goal:

The final project I did for my Machine Learning class is a handwriting recognition model which takes in
imgaes of handwriting sentences from different writers and recognize the writers. The dataset I chose contains
4900 images from hundreds different writers. My goal was to classify the writers according to their
different writing styles. 

<img src="/images/image_demo.png" width="600"/>


Data Preprocessing:

(1) Predicted Target: The file names of all images are written in a dash separated filename format and I
was taking the middle part of the filename (writer id) from filenames as my predicted target in a list. 
And my final prediction result would come in a number format.

<img src="/images/image format name.png" width="600"/>

(2) Cross Validation: My dataset was split in to train, test and validation in a 4:1:1 ration.

(3) Image Preprocessing: There is a step of resizing all images into a dimension of 113*113. The function 
randomly crop same size patches from these images as an input which would be helpful to increase the 
accuracy for further prediction.

<img src="/images/crop.png" width="600"/>

Example of a patch:

<img src="/images/Patch 3.png" width="600"/>


Model Build_in:

The model I chose is Keras which is more complicated than Fastai. As I resized image tp 64*64 within the
neutral network for easy computation and built in the model, I got the model summary shown below:

<img src="/images/model summary.png" width="600"/>

Later, I fit my dataset using the built_in model for 8 epochs which took over 8 hours to run it.

<img src="/images/epoch summary.png" width="600"/>

Result:

The final accuary I got was around 68%. Since I split all into 50 categories which is a lot, the accuracy
was not bad. As a result I could use for further prediction.

<img src="/images/Accuracy.png" width="600"/>

I also loaded in my test dataset to predict the writers and here are one of the twenty handwriting patches 
predicted to be the same writer as the first writer in the test set as an example.

<img src="/images/all writers similar code.png" width="600"/>

<img src="/images/Patch 1.png" width="600"/>