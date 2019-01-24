# Session 09: Deep Learning

- (25 mins) Mini Lecture
- (15 mins) Activity
- (15 mins) Mini Lecture
- (20 mins) Activity

## (25 mins) Mini Lecture

[Slides](https://docs.google.com/presentation/d/18YLnUL4r4q-bp9l8a9VynJb7gf0wXnyN8wnhBLyjTsg/edit#slide=id.g4c29fe321c_0_30) introduce the basic concepts behind neural networks, inspired by lectures from [Dr. Mustafa Bilgic](http://www.cs.iit.edu/~mbilgic/#courses) at the Illinois Institute of Technology. Main ideas:

- Deep learning models learn “deep” representations for tasks by learning functions that are much more complicated than the supervised learning models discussed in this course. This enables learning on more complicated inputs such as images, audio, text, and other forms of media. For example, [NVIDIA researchers](https://www.youtube.com/watch?v=kSLJriaOumA) used deep learning and style transfer algorithms to generate realistic human faces.
- However, the more complicated representations may make models more difficult to explain and introduce new opportunities for adversaries.
- Neural networks can be built with perceptrons, which take inputs with weights and a bias weight to output a value based on an activation function.
- The effectiveness of a neural network at a task is measured by a loss function.
- Different activation functions and hidden layers determine what kinds of functions a neural network can represent.

## (15 mins) Activity

Share the link to the [Tensorflow Playground](https://playground.tensorflow.org/): a browser-based interactive activity that allows students to configure various components of a neural network and see how well it classifies toy datasets. Ask students to describe their configuration using language learned from the lecture.

When students feel comfortable using the playground, challenge them to configure a neural network that can classify samples in the spiral dataset. The website saves the configuration in the URL, so students can share their neural networks with the instructor or other classmates. However, since the initial weights of the neural networks are randomly-generated, even two runs with the same configuration may have dramatically different results.

## (15 mins) Mini Lecture

[Slides](https://docs.google.com/presentation/d/18YLnUL4r4q-bp9l8a9VynJb7gf0wXnyN8wnhBLyjTsg/edit#slide=id.g4d4fb7ccc9_0_351) introduce the basics of convolutional neural networks (CNNs) for deep learning image classification tasks. Main ideas:

- A CNN is similar to the neural network described in the first mini lecture, except with an input for each channel in each pixel of the image and different kinds of hidden layers.
- Convolution nodes apply a filter to every pixel in the node’s input image, aggregating the values of each pixel and its neighbors into the corresponding pixel of an output image. The output image represents a feature map: regions of the image which, when active, influence the classification output.
- Max pooling nodes apply a filter to each pixel in the node’s input image, selecting the maximum value among each pixel and its neighbors to add to the corresponding pixel of an output image. The output image aims to reduce noise from the input and image and avoid oversaturating the input image through repeated convolution.
- CNNs are typically made up of several layers of convolution and max pooling, one after the other.
- High-level APIs such as Keras allow machine learning practitioners to utilize neural networks by describing the structure, training the model, then evaluating the results.
- CNNs are learning a numerical representation for classifying images, which can often lead to harmful false positives. For example, Google image classification models inappropriately classified pictures of African-Americans as “gorillas.”
- Values of individual pixels could alter the classification result. For example, images of seemingly meaningless noise could be positively classified simply because they pass through convolution and max pooling layers in the same way that the “true” images do.
- Style transfer algorithms are a type of deep learning that can generate new images that have the content of one image but the style of another. These models use special loss functions to quantify how much content or style is lost in the process.

## (20 mins) Activity

Share the link to [Lawrence Francis’](https://github.com/ldfrancis) demo of a style transfer model. Students can make a copy of [the Jupyter notebook on Google Colab](http://bit.ly/2H9gvIW), upload their own content and style images, and run the model in their browser to see the result. Students may not be able to run the Colab notebook if their browser blocks cookies for the page. Remind students to only upload images that they have permission to use and modify.

**Next:** [Common Good](session10.md)
