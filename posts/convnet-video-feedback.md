<!--
.. title: Video Synthesis With Convolutional Autoencoders
.. slug: convnet-video-feedback
.. date: 2017-01-09 18:26:25 UTC-05:00
.. tags:
.. category:
.. link:
.. description:
.. type: text
-->

Context: see [my post on video feedback](../video-feedback)

In spring of 2015 I took a [seminar in deep learning](http://www.cs.dartmouth.edu/~lorenzo/teaching/cs189/Archive/Spring2015/) with Lorenzo Torresani. It was one of the most exciting classes I've ever taken. I had been introduced to the field of machine learning by Lorenzo's class the previous fall, and was already riding high on the concept of solving generic problems by optimization. The idea of deep learning for *representation learning*--extending ML to more generic problems by learning to interpret raw data--was exciting on its own. I'd also been talking a lot to cool dudes [Parag Mital](http://pkmital.com/home/), and [Andy Sarroff](http://www.cs.dartmouth.edu/~sarroff/) about their work with machine learning, sound and video. And what really blew my mind about deep learning was the similarity between neural networks and the audio/video feedback I'd been using to make noise. This project was my attempt to incorporate a convolutional network trained to encode images as part of a video feedback process.

I really bit off more than I could chew for a seminar project: my approach demanded that I design and train my own neural network with caffe *and* re-implement the forward pass with OpenGL *and* spend time exploring the feedback behavior. I was able to train my autoencoders with some success, and I was able to make some singular boiling multicolored nonsense. I didn't get the spectacular emergence of natural image qualities I hoped for. A few months later deep dream came out, articulating a clearly superior approach with jaw-dropping results. I may still try to get the openFrameworks app running again and capture some video, for posterity.

Here's the [GitHub](https://github.com/victor-shepardson/feature-feedback), which includes a [writeup](https://github.com/victor-shepardson/feature-feedback/blob/master/notebooks/writeup.ipynb), a [jupyter notebook](https://github.com/victor-shepardson/feature-feedback/blob/master/notebooks/presentation.ipynb) with the autoencoder experiments in it, and the source code for an openFrameworks app which runs the process interactively.
