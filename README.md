# ☝✌ Hand-Gesture-Recognition-using-CNN 🤘🤙

In this project, we have created a Convolution Neural Network for recognizing the hand gestures which are predominantly used for communicating to humans with speech and hearing impairment. The CNN is built and trained on a set of 20 types of hand gestures and the same is tested aginst a different set of same 20 types of hand gestures.
<br>
The libraries used are:
- Numpy & Pandas
- Matplotlib (for displaying images)
- Sklearn (for classification report)
- Pytorch & Torchvision (for building & optimizing the CNN)
<br>
Before we start building the CNN, we shall prepare the image set by performing normalization & other image transformations to bring about variability to these image sets. Next, we prepare the dataloaders for training, validation and testing sets with a predefined batch size. Here, we have used the dataloader object instead of simple OpenCV imports because the time taken for loading such a large image set is a lot.
<br>
<br>
Now, we initialize the device for running the CNN (either CPU or GPU : but choose GPU else the kernel might crash). Create the dataloader for the device and load the tensors (ofc coz we are using Pytorch) of the datasets into the device. Now, create a Base image classifer using "cross entropy" as the loss function.
<br>
<br>
Finally, we create a CNN on top of this Base image classifier and keep the optimizer as "Adam" optimizer for handling large datasets. Fit to this CNN for 10 epochs and validate it aginst the validation set. Finaaly, test it against the test set to get the classification report. The results of loss and accuracy across the 10 epochs are given below:
<br>
<br>
<div style="display:grid">
  <img src="Acc Vs Epochs.jpg" style="height:300px;width:300px;float:left">
  <img src="Loss Vs Epochs.jpg" style="height:300px;width:300px;float:left">
</div>
<br>
<br>
<b>We acquire 99% accuracy !!!</b>
