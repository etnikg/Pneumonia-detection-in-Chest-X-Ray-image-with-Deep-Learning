# Pneumonia detection in Chest X-Ray image with Deep Learning

## Get started

Lung disease “Pneumonia” was detected in Chest X-Ray images using the Deep
Neural Networks model. The architecture of this model consists of Convolutional Neural Networks-CNN. The model also includes the Dense Neural Network so that the output is positive or negative for the particular image chosen for preaching whether there is pneumonia or not.


For the detection of pneumonia, the model was initially trained with a dataset with thousands of Chest X-Ray images from people with this disease but also from healthy ones so that the dataset is divided into categories for training, validation and testing of the model.


The prediction model was done in Python language using the Tensorflow framework and using as editor, Google Colab. While this work also touches on the field of medicine, then it has been worked out that the model should be created with the highest possible degree of accuracy.

## Dataset

The dataset was used by D. Kermany with co-authors (https://www.cell.com/cell/fulltext/S0092-8674(18)30154-5), which includes 5856
images. This dataset was created by collecting and labeling a total of 5,232 X-ray images from children's breasts, including 3,883 characterized as pneumonia (2,538 bacterial and 1,345 viral) and 1,349 normal, out of a total of 5,856 patients to train and test the model preacher. The database is organized into 3 files (train, test, validation) and contains sub-folders for each category of images (Pneumonia / Normal). There are 5,863 images with X-ray of JPEG format, ie with 2 categories (Pneumonia / Normal). The date is divided in the report 80:20 for model training and testing 
X-ray images of the chest (anterior-posterior) were selected from retrospective groups of
pediatric patients aged one to five years. The entire X-ray image from the chest was performed as
part of the routine clinical care of patients.
For analysis of X-ray images of the chest, all chest radiographs were initially taken.
checked for quality control by removing all low quality scans or
unreadable. The diagnoses for the images were then evaluated by two expert physicians before
to be purged for the training of the preaching model. To calculate the estimation errors, group i
the assessment was also checked by a third expert.

## Model

Prediction DL model consists of the sequential extension of 5 layers
CNN (each layer includes two CNN blocks). Between each layer is applied max pooling 2 × 2. As input comes the formatted photo at 150 × 150 × 3 pixels so with respect to RGB. The data enters batch clusters with 4 of them and 100 epoch repetitions for each image. It was first asked to generate 16 3 madh 3 kernels where this number is doubled for each CNN layer reaching 128 3 × 3 kernels in the last layer.

## Accuracy

Achieved accuracy 93.59% with 20 epoch and validation accuracy 94%.

As an objective function is used categorical crossentropy.

Stochastic Gradient Descent is choosed as optimizer.

## Try it
__________________________________________________________________________________
 
The script for pneumonia detection is: Pneumonia_detection_with_DL.ipynb
 
If you want to get the model for Transfer Learning, the model is saved in .h5 file: pneumonia_classifier_model(weights).h5
 
Also if you want to download the dataset, you can find it at dataset branch.
__________________________________________________________________________________

## License

This software is licensed with GNU General Public License v3.0

