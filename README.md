# Generate-Faces-Using-GANs
Udacity Deep Learning Nanodegree project - Using generative adversarial networks to generate new images of faces.

Objective: Define and train a DCGAN on a dataset of faces. Goal is to get a generator network to generate new images of faces that look as realistic as possible!

What I learnt:
1. Pre-processing and Loading the Data.
2. Creating a DataLoader with appropriate hyperparameters.
3. Defining the model:
   * Define the Discriminator - A convolutional classifier without any maxpooling layers. To deal with this complex data, created a deep network with normalization.
   * Define the Generator - mostly transpose convolutional layers with normalization applied to the outputs.
   * Initialize the weights of the network -  initialize the weights of the convolutional and linear layers of model. Initialize the weights to a normal distribution, centered around 0, with a standard deviation of 0.02. The bias terms, if they exist, may be left alone or set to 0.
   * Define  models' hyperparameters and instantiate the discriminator and generator from the classes defined.
4. Calculating Generator and Discriminator losses.
5. Defining optimizers for Generator and Discriminator.
6. Training the network, understanding losses and adjusting the hyperparameters.
7. Using the Generator to generate some face samples.
