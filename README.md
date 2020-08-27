## Generate Synthetic Images with DCGANs in Keras

In this project, I have built and trained a Deep Convolutional Generative Adversarial Network (DCGAN) with Keras to generate images of fashionable clothes.

In the [GAN setup](https://developers.google.com/machine-learning/gan/gan_structure), we want to be able to sample from a complex, high-dimensional training distribution of the Fashion MNIST images. However, there is no direct way to sample from this distribution. The solution is to sample from a simpler distribution, such as Gaussian noise. We want the model to use the power of neural networks to learn a transformation from the simple distribution directly to the training distribution that we care about. 

The GAN consists of two adversarial players: a discriminator and a generator. I have trained the two players jointly in a [minimax](https://en.wikipedia.org/wiki/Minimax) game theoretic formulation.

Please have a look at the notebook [here](DCGAN-keras.ipynb), or open it on [Colab](https://drive.google.com/file/d/1810chR_kMcR_PoLniIaa-8_GdXJtB-2K/view?usp=sharing).

For reference, have a look at [this](https://www.tensorflow.org/tutorials/generative/dcgan) page on the TensorFlow website.
