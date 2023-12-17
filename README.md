# X-ray_deblurring
Deep Learning Model to Deblur the blurred X-ray image (RBG)

We choose to use Chest X-ray radiographs. The particular dataset used consists of the images of chest X-rays diagnosed as Pneumonia stored in .jpeg format. All these images are sharp and perfect for making diagnosis. But we need the pairs of Sharp and corresponding blurred image to effectively train the model.

Blur is introduced to get the pair of blurred and corresponding ground truth.
In Gaussian blur, an image is convolved with a kernel that has a Gaussian distribution.

#SRCNN
The architecture of the network consists of three convolutional layers with ReLU (Rectified Linear Unit) activation functions and different kernel sizes and number of output channels.

#DAE
The encoder is trained to minimize the KL-divergence between the latent distribution and a standard Gaussian distribution, while also minimizing the reconstruction loss between the original and reconstructed images.
The decoder architecture is designed to be symmetric to the encoder architecture, with a series of transposed convolutional layers that gradually increase the size of the feature maps until the final reconstructed image is produced.
#
