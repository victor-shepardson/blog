<!--
.. title: Video Feedback
.. slug: video-feedback
.. date: 2017-04-23
.. tags: feedback, visual, video, generative, shader
.. category:
.. link:
.. description:
.. type: text
-->

Douglas Hofstadter's [Gödel, Escher, Bach](https://archive.org/details/GEBen_201404) contains about a hundred captivating ideas, and just one of them is the concept of video feedback: connect a video camera to a screen, and then point it at the screen. Weird stuff happens on the screen as light is projected though the air, captured by the camera and circled back to the screen, mutating each time. Zoom out to get a infinite hall of mirrors effect, zoom in to get kaleidoscopic pulsations, loosen the focus to get bubbling slime.

As an undergrad, I became interested in computer graphics. Particularly, the idea of *procedural graphics*: generating images from nothing but math, as opposed to using assets made by virtually drawing (as with photoshop) or digitizing reality (as with a digital camera). Procedural graphics can translate some of the tantalizing infinites of mathematics into rich sensory experiences! [A brief article](http://www.iquilezles.org/www/articles/warp/warp.htm) by Íñigo Quílez introduced me to the idea of turning a random number generator into an endless alien terrain. One popular way to do this is with *fragment shaders*, specialized programs for doing pixel-by-pixel graphics with the GPUs found in most computers. For more than a few examples, see [Shadertoy](https://www.shadertoy.com/).  

You can put a fragment shader into feedback just like a video camera. Pixels go in, pixels come out, pixels go back in 60 times per second. The shader determines how colors mutate and interact with nearby colors each time. Here are a few of mine:

<iframe width="100%" height="256" frameborder="0" src="https://www.shadertoy.com/embed/4d2BRm?gui=true&t=10&paused=true&muted=false" allowfullscreen></iframe>
<iframe width="100%" height="256" frameborder="0" src="https://www.shadertoy.com/embed/lt2yz3?gui=true&t=10&paused=true&muted=false" allowfullscreen></iframe>
<iframe width="100%" height="256" frameborder="0" src="https://www.shadertoy.com/embed/lsBcRK?gui=true&t=10&paused=true&muted=false" allowfullscreen></iframe>

Other things which resemble digital video feedback:

- 2D Cellular automata like [Conway's game of life](http://golly.sourceforge.net/)
- Finite element physical simulations of fluids and [reaction-diffusion systems](https://pmneila.github.io/jsexp/grayscott/)
- Convolutional neural network visualization techniques like [deep dream](https://research.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html)

Other people working with this kind of stuff:

- [Sabrina Ratté](http://sabrinaratte.com/)
- [Alex Dupuis](http://alexanderdupuis.com/)
- [Cornus Ammonis](https://twitter.com/cornusammonis)
- [Andrew Benson](https://pixlpa.com/)
- [Felix Woitzel](https://twitter.com/Flexi23)

I just can't stay away. See projects such as [ABSTRACT/CONCRETE](../abstract-concrete/), [Video Synthesis With Convolutional Autoencoders](../convnet-video-feedback/) and [Data Sonification Using a Cortical Representation of Sound](../cortical-sonification).
