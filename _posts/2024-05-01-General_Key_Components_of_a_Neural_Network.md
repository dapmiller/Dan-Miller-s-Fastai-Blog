# General Key Components of a Neural Network

I've now done a few courses where I've got to play around with neural networks. Let's break it down using the Fastai library and focus on a Convolutional Neural Network (CNN).

![Sandwich Neural Network](https://editor.analyticsvidhya.com/uploads/59954intro%20to%20CNN.JPG)
*Image Source: [Convolutional Neural Network: An Overview](https://editor.analyticsvidhya.com/uploads/59954intro%20to%20CNN.JPG)*

## Let's Think of the Network as a Sandwich 🥪

1. **Convolutional Layer** – these are like the solid layers in a sandwich. They are core building blocks that give the neural network flavor or help learn features through each layer. In Fastai, you can easily define a convolutional layer with `conv_layer()`.

2. **Pooling Layer** – these are like the action when you grip the sandwich, you are condensing the size. Pooling layers, such as max pooling or average pooling, are used to reduce the spatial dimensions of the input volume. Fastai uses the functions `pool()`.

3. **Activation Layer** – this is like when you take a bite of that sandwich but miss the patty. Activation functions introduce non-linearity and essentially determine if a neuron is activated or not and used in the input of the network to make a prediction. Fastai has various activation functions such as ReLu, sigmoid, and Tanh.

4. **Batch Normalization** – this is like when you cut the sandwich up into even slices. Batch normalization helps in stabilizing and accelerating the training of the neural network. Fastai provides `nn.BatchNorm2d()`.

5. **Dropout** – this is when half your sandwich falls out of your bread. Dropout is a regularization technique that randomly drops a fraction of neurons during training. This is used to prevent overfitting. Fastai incorporates this dropout layer with `nn.Dropout()`.

6. **Metrics and Loss Functions** – this is like adding new things to the sandwich and comparing it to a previously glorious sandwich taste in your head; then using a few metrics to evaluate its looks, tastes, and ease to make. Essentially, a loss function measures the difference between predicted and expected outputs of a model. The goal of training is to minimize this difference. Whereas a performance metric is used to evaluate the model after training. Fastai supports numerous loss functions and metrics tailored for classification problems.

7. **Transfer Learning** – is like stealing your sibling’s sandwich and then putting an olive on top to say it's yours. Fastai has simplified transfer learning by providing high-level functions like `cnn_learner()`. This enables you to easily fine-tune pre-trained models on custom datasets.

Overall, Fastai has made eating a sandwich fun, I mean making a neural network simple. The process of building, training, and interpreting CNNs is both accessible and simple for beginners like me and experienced programmers.
