# VGG_Subclassing
impalement VGG model using subclassing , i will build a class that implements a [VGG network](https://towardsdatascience.com/vgg-neural-networks-the-next-step-after-alexnet-3f91fa9ffe2c) that can be trained to classify images. The model will look something like this:

![image](https://github.com/HadeerArafa/VGG_Subclassing/blob/main/VGG.png)

It is primarily made up of a series of `Conv2D` layers followed by a `softmax` activated layers to classify the image. As you can see, this will be a handful and the code will look huge if you specify each layer individually. so can instead use model subclassing to build complex architectures. 

And we can see that there are repeated blocks of ` number of Conv2D layers "two or three" followed by a MaxPooling2D layer` so we can encapsulate repeating parts of a network then reuse that code when building the final model.
