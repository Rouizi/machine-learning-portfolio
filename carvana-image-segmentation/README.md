## Carvana Image Masking Challenge

The dataset is provided by Carvana, an online used car startup. Carvana wants to superimpose cars on a variety of backgrounds, so the challenge is to develop an algorithm that detect the boundaries of the car in an image and remove the studio background. 

For this purpose I used a modified architecture of an encoder-decoder model: The U-Net. The encoder part was the intermediate layers of a pretrained VGG19 model, and the decoder part consisted of a deconvolution layer followed by a batchnormalization layer and the relu activation function.

The model achieved 99.5% accuracy on the training and the validation set.