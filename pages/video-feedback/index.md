<!--
.. title: Video Feedback
.. slug: video-feedback
.. date: 2017-01-11 22:08:22 UTC-05:00
.. tags: feedback, visual, douglas hofstadter, shadertoy
.. category:
.. link:
.. description:
.. type: text
-->

Way back in high school I read Douglas Hofstadter's [Gödel, Escher, Bach](https://archive.org/details/GEBen_201404). If you aren't familiar, I have to advise you to go read it instead of looking at my dumb blog. There are about a hundred captivating ideas in there, and just one of them is the concept of video feedback: connect a video camera to a screen, and then point it at the screen. Weird stuff happens on the screen. (Meanwhile I was learning to play the guitar, and discovering that the electro-acoustic feedback of wiggling the thing around in front of an amp is much more fun than drilling scales.)

<iframe src='https://archive.org/stream/GEBen_201404/GEBen?ui=embed#page/n496/mode/1up' width='480px' height='430px' frameborder='0' ></iframe>

As an undergrad, I became interested in computer graphics. (I know of two things that teach you to really see: studying the science of computer graphics, and learning to paint or draw from life.) I was especially taken with the idea of *procedural graphics*: generating images from nothing but math, as opposed to using assets made by virtually drawing (as in photoshop) or digitizing reality (as with a digital camera). Procedural graphics can translate some of the tantalizing infinites of mathematics into rich sensory experiences! In particular [this brief article](http://www.iquilezles.org/www/articles/warp/warp.htm) by Íñigo Quílez had me enthralled by the idea of turning a random number generator into an endless alien terrain.

Eventually I put two and two together: you can dispense with the video camera and program a completely virtual video feedback process. And once you do, it can do much weirder things than a video camera. This was hardly unknown in computer graphics, yet was weirdly unpopular. There's a preoccupation with statelessness in the scene Quílez is part of; [Shadertoy](https://www.shadertoy.com/) didn't render to texture until 2016! Academic CG tends to focus on predictability and utility for efficient, photorealistic rendering; feedback is unruly and difficult to analyze. Then there are fractals, which are iterated, but not open ended: you iterate to convergence, rather than letting the image evolve as in video feedback. However [Jim Crutchfield](http://csc.ucdavis.edu/~chaos/) has written about the dynamics of digital video feedback from a math/physics perspective. 2-D cellular automata like Conway's game of life can be thought of as digital video feedback, and there's a whole [hobbyist community](http://golly.sourceforge.net/) there, not to mention the [academic artificial life community](http://alife.org/) or [Stephen Wolfram](http://www.wolframscience.com/)'s insular "new kind of science". The whole field of computational fluid dynamics is doing a similar thing with a different set of priorities! And of course video feedback shows up in fine art beginning (?) with video artists like Nam June Paik.

Finally in the fall of 2014 after encountering such cool dudes as [Sabrina Ratté](http://sabrinaratte.com/) and [Alex Dupuis](http://www.alexanderdupuis.com/) I was galvanized to get some feedback of my own going. Still blissfully ignorant of much, I started making stuff like this (more recent) doodle:

<iframe width="100%" height="332" frameborder="0" src="https://www.shadertoy.com/embed/MdcSW8?gui=true&t=10&paused=false&muted=false" allowfullscreen></iframe>

(Incidentally [these folks](https://synesthesia.live/) licensed the above shader to use in their music-reactive visuals software Synesthesia. It looks pretty neat, though I haven't been able to mess with it myself since I don't have a Mac. Maybe take a look if you do.)

Eventually this would grow into such projects as [ABSTRACT/CONCRETE](../abstract-concrete/), [Video Synthesis With Convolutional Autoencoders](../convnet-video-feedback/) and [Data Sonification Using a Cortical Representation of Sound](../cortical-sonification).
