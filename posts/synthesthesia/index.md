<!--
.. title: Synesthesia Music Visualizer Scenes
.. slug: synthesthesia
.. date: 2024-03-03
.. tags: visual, sonic, audiovisual, glsl, shadertoy, feedback
.. category:
.. link:
.. description:
.. type: text
-->
<style>
  .video-wrapper {
   width: 100%;
   display: inline-block;
   position: relative;
  }
  .video-wrapper:after {
      padding-top: 56.25%; /*16:9 ratio*/
      display: block;
      content: '';
  }
  .video {
      position: absolute;
      top: 0; bottom: 0; right: 0; left: 0;
  }
</style>

[Synesthesia](http://synesthesia.live/) is VJ software for making audio-reactive visuals. It draws from the [Shadertoy](https://www.shadertoy.com/) community, where everything is made with GLSL fragment shaders, but includes an easy way to add audio and video inputs and build simple MIDI-mappable control interfaces. Basically, everything a VJ needs to actually perform live with some shaders. The folks building Synesthesia seem super respectful of free-sharing ethos of Shadertoy -- they reached out to shader programmers like me and comissioned new works for Synesthesia, while keeping the actual shaders always hackable by users within the application. I wound up making a few fun video feedback and cellular-automata based scenes, and recently was goaded into using some of them to mess up the live stream from an algorave concert at the AIMC conference: 

<!-- https://youtu.be/d0RMUqcbhmQ?t=8639 -->

<div class="video-wrapper">
  <div class="video">
<iframe width="100%" height="100%" src="https://www.youtube.com/embed/d0RMUqcbhmQ?start=8639&rel=0" title="AIMC 2023 Concert 3 – Algorave" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
  </div>
</div>
