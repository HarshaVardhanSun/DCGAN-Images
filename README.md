Using two neural networks and matching them against one other (thus the term "adversarial"), generative adversarial networks (GANs) are computational structures that produce new, synthetic instances of data that can be mistaken for actual data. They are extensively employed in the production of voice, video, and images.
GANs are composed of two parts:
--> Generator - creates new instances of data
--> Discriminator: aims to differentiate synthetic or fabricated data from authentic dataset.
By predicting a label or category to which a particular instance of data belongs based on its features, discriminative algorithms attempt to classify input data. Discriminative algorithms thus associate labels with features. That correlation is all that matters to them.Conversely, generative algorithms, to put it loosely, have the opposite effect.They try to anticipate features given a certain label rather than a label given specific features.
They both begin training from scratch together, and throughout the course of the training epochs, the generator learns to shape the random distribution.

DCGAN Model Architecture
Using a typical CNN architecture on the discriminative model, the DCGAN architecture's core operates. Upconvolutions are used in place of convolutions in the generator, resulting in progressively larger representations at each layer as it maps from a low-dimensional latent vector onto a high-dimensional image.
Both the discriminator and the generator should employ batch normalization.
To create deeper architectures, remove all completely connected hidden layers.
For all layers in the generator, use ReLU activation; Tanh is used for the output.
For each layer, use LeakyReLU activation in the discriminator.
