# Neural-Style-Transfer

*COMPANY*: CODTECH IT SOLUTIONS
*NAME*: SREEJA R
*INTERN ID*: CT06DR3163
*DOMAIN*: ARTIFICIAL INTELLIGENCE
*DURATION*: 6 WEEKS
*MENTOR*: NEELA SANTHOSH

**DESCRIPTION OF THE PROJECT**:

This project implements a *Neural Style Transfer (NST)* system using Python and the PyTorch deep learning framework. The main objective of the project is to generate a new image that combines the *content* of one image with the *artistic style* of another image. Neural Style Transfer is a popular computer vision technique that uses deep convolutional neural networks to understand and manipulate visual patterns such as textures, colors, and shapes. In this project, a pre-trained *VGG16 convolutional neural network* is used as a feature extractor to separate and represent the content and style information of images.

The project begins by loading the required libraries such as PyTorch, TorchVision, and PIL. Images are loaded at a low resolution to reduce computation time and memory usage, making the system stable and suitable for CPU execution. The VGG16 model, which is pre-trained on the ImageNet dataset, is used only for feature extraction, and its parameters are frozen to prevent training. The convolutional layers of VGG16 are used to extract feature maps, as these layers capture important visual information such as edges, textures, and patterns.

To represent the artistic style of an image, the project uses *Gram matrices*, which capture correlations between feature maps. These matrices effectively represent textures and styles independent of spatial location. Content loss is calculated by comparing feature maps of the target image with those of the content image, while style loss is calculated by comparing Gram matrices of the target image with those of the style image. Both losses are combined using weighted parameters to control how much content and style influence the final output.

The target image is initialized as a copy of the content image and is iteratively updated using the *Adam optimizer*. During each training iteration, gradients are computed and applied to the target image so that it gradually adopts the style patterns while preserving the original content structure. After a small number of epochs, the final stylized image is saved as an output file. Overall, this project demonstrates the practical application of deep learning in artistic image generation and provides a strong foundation for understanding convolutional neural networks, feature extraction, and optimization techniques in computer vision.

**OUTPUT**:

<img width="128" height="128" alt="Image" src="https://github.com/user-attachments/assets/1cd8d735-cc8e-4850-80de-3af7aa86197e" />
