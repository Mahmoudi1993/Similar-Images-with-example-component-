# Image Similarity Model  based on  Image Classification
we propose, a Image Similarity method based on Image Classification. that It ensures semantic consistency between the original and similarity images, and achieves good image diversity. 
This model is trained using Image Classifier  and Resnet18 in such a way that it can retrieve the similar images of the query image.

**Steps :**
1. Image Classifier

    cifar10 Training an image classifier:
    For this tutorial, we will use the CIFAR10 dataset. It has the classes: ‘airplane’,‘automobile’, ‘bird’, ‘cat’, ‘deer’, ‘dog’, ‘frog’, ‘horse’, ‘ship’, ‘truck’.
    The images in CIFAR-10 are of size 3x32x32, i.e. 3-channel color images of 32x32 pixels  in size.

     We will do the following steps in order:
   
     *	Load and normalizing the CIFAR10 training and test datasets using torchvision.
   
     *	Define a Convolution Neural Network
   
     *	Define a loss function
   
     *	Train the network on the training data
   
     *	Test the network on the test data
   
     *	Loading and normalizing CIFAR10

2. Resnet18

   First, we predict the class of the input images with using a image classifier model that pre-trained. then each image is placed in a folder with its class images, this folders is given as input to the Resnet18 
   network one by one.Based on the resnet18 implementation from PyTorch it creates feature vectors from the input images, compares it to the other images and sorts for each image a similarity list. Eventually, the 
   result is visualized for a tiny test set that is provided within the repository.

Architecture of Image Similarity method based on Image Classification:
   

