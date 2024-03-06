<!--
.. title: Reproducing α-GAN
.. slug: reproducing-alpha-gan
.. date: 2018-05-06
.. tags: machine learning, deep learning, computer vision, GAN, autoencoder, pytorch
.. category:
.. link:
.. description:
.. type: text
-->

<!-- Generative Adversarial Networks or *GANs* are one the most exciting ideas to emerge from the deep learning boom.

Generally speaking, generation seems hard compared to classification. Think of images -- you can tell if an image has a bear in it. But drawing a convincing bear of your own is more difficult. To *classify* images as bear/non-bear is easy, to *generate* bears is hard. And indeed this is true for computers; feed a large neural network enough labeled images and it will be able to label new ones for you fairly well. But the best methods for generating original images will give you bizarre mutants or vague blurs.

GANs use two networks to transmute generation into classification. A *generator* (G) network turns random codes into images, and a *discriminator* (D) network classifies images as either real or generated. Each network provides an objective for the other -- G tries to fool D while the D learns from data to stay one step ahead. G and D can be any differentiable neural network, so G can be trained by backpropagation through D. In limited domains, this works [spooky good](https://www.youtube.com/watch?v=G06dEcZ-QTg&t=1m25s).

Ideally, a GAN gives you a dense code space from which you can sample random points on the data manifold. You can even take any two points in the code space and interpolate them to morph between images. Theoretically, any real (non-generated) image should have a corresponding point in the code space, but how do we find that point?

This is what Rosca et al. tackle in [Variational Approaches for Auto-Encoding
Generative Adversarial Networks](https://arxiv.org/abs/1706.04987) -->

I implemented Rosca, Mihaela, et al. ["Variational Approaches for Auto-Encoding
Generative Adversarial Networks"](https://arxiv.org/abs/1706.04987) using Pytorch. It's a modular implementation -- plug in any torch modules as encoder, generator, discriminator and code discriminator.

On [GitHub](https://github.com/victor-shepardson/alpha-GAN)
