# veery

Veery is a simple machine learning model for MNIST using [TensorFlow](https://www.tensorflow.org).

### Background

This project is part of [52projects](https://donny.github.io/52projects/) and the new stuff that I learn through this project: [TensorFlow](https://www.tensorflow.org).

### Project

Veery is my attempt to learn more about machine learning using TensorFlow. It's my first exposure to this area and I've been watching and reading quite a few resources:

- [Learn TensorFlow and deep learning, without a Ph.D.](https://cloud.google.com/blog/big-data/2017/01/learn-tensorflow-and-deep-learning-without-a-phd)
- [TensorFlow and deep learning - without a PhD by Martin Görner](https://www.youtube.com/watch?v=vq2nnJ4g6N0)
- [Getting Started with TensorFlow](https://www.tensorflow.org/get_started/get_started)
- [MNIST for ML Beginners](https://www.tensorflow.org/get_started/mnist/beginners)

Shown below is a screenshot of running a trainable linear regression model from [Getting Started with TensorFlow](https://www.tensorflow.org/get_started/get_started) and a model for MNIST from [MNIST for ML Beginners](https://www.tensorflow.org/get_started/mnist/beginners):

![Screenshot](https://raw.githubusercontent.com/donny/veery/master/screenshot.png)

### Implementation

The code [`linear_model.py`](https://github.com/donny/veery/blob/master/linear_model.py) shows how we use TensorFlow to solve the equation: `y = W * x + b`. Given `x` and `y`, find the value of `W` and `b`, with the following training data: `x: [1, 2, 3, 4], y: [0, -1, -2, -3]`. From the screenshot above, the solution was `W` equals -0.9999969 and `b` equals 0.99999082; which is very close to the actual answer of `W` equals -1 and `b` equals 1.

The code [`mnist_softmax.py`](https://github.com/donny/veery/blob/master/mnist_softmax.py) shows how we use TensorFlow to recognise images of handwritten digits. A more detailed explanation on the MNIST problem and how the code works can be found in [MNIST for ML Beginners](https://www.tensorflow.org/get_started/mnist/beginners). The screenshot above shows the accuracy of our model which is 92% (0.9196). It means that with 100 images of handwritten digits, the model fails to recognise 8 of them. Although the accuracy looks good, especially for beginners in ML, actually it's quite bad given that the best model can get to over 99.7%.

### Conclusion

I did a subject on artificial intelligence before and this project is my first attempt to learn more about machine learning using TensorFlow. I find it very fascinating. I was particularly impressed on how TensorFlow can find a solution to a given equation (I am still a beginner that can be easily impressed). I believe machine learning and artificial intelligence will be the foundation of many smart solutions in the future.
