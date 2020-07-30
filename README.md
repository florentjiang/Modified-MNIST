# Modified-MNIST

You are given a dataset of 40,000 images containing MNIST digits. However, each image may contain multiple digits, and each digit will have a different size. Moreover, each digit may have been transformed (rotated, translated, etc.). Finally, each image contains a background which consists of noise.

The task at hand is to **find which number occupies the most space**. (To be perfectly clear, this is not the number with the highiest arithmetic value)

![Modified MNIST](./image/modified_mnist.png)

In this task, various pre-processing techniques are implemented (such as normalization, noise reducing, bounding box, resizing, image augmentation, etc) and optimizers (Adam, SGD, and RMSprop). Then the performance of both 4-layer convolutional neural network (CNN) and some existing model architectures (DenseNet, MobileNetV2, Xception, and InceptionResNetV2) are tested. All of the experiments are measured in accuracy using hold-out validation. 