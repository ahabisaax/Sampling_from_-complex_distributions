# Sampling_from_-complex_distributions
Using Machine Learning and generative modelling (GANs) to sample from the Maxwell Juttner Distribution. This distribution appear commonly in astrophysics and is used to model the velocity of high energy particles. It is known to be difficult to sample from using conventional sampling methods (including rejection sampling, Inverse Transform Sampling and MCMC methods) for certain temperature values. As a result the motivation behind this work is a ML based approach to learn the distribution via a set of network weights which can quickly load in random variate from the distribution via a series of matrix multiplications.


An extention of this work is to train a CGAN which is trained on a variety of temperatures values so that the generator learns the family of distributions that makes up the MJ distribution. The training data would be conditioned on $T$ and so the trained model can learn $p(x|T)$ and produce random variate given an input  $T$.
