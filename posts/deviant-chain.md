<!--
.. title: Deviant Chain (2019)
.. slug: deviant-chain
.. date: 2024-03-02
.. tags:
.. category:
.. link:
.. description:
.. type: text
-->
<!-- <style>
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
</style> -->

In 2019 I worked on a concert installation called [*Deviant Chain*](https://stefanmaier.studio/deviant-chain-2019/) with Stefan Maier and Alan Segal. Stefan, a composer, and Alan, a filmmaker, created a sort of art haunted house in which the audience moved from room to room in a former bank vault, encountering a series of short videos and sound works with themes of transhumanism and machine alterity. One of these dealt with the development of language and the human voice, and for this I created neural text-to-speech software for Stefan to gather sound material from. 

At this time, the [WaveNet demo](https://deepmind.google/discover/blog/wavenet-a-generative-model-for-raw-audio/) was in the air. This was one of the first neural generative models to work well with raw audio, and the uncanny babbling of the unconditional speech model was an arresting artifact of the ever-weirder capabilities of statistical autoregressive models. It had a few problems though: no open source implementation, very expensive training process, and extremely slow inference process. After some research, I found an open implementation of Tacotron2 from NVIDIA, which was state of the art for text-to-speech at the time, and substituted a WaveGlow vocoder for the original WaveNet. It turned out to still be quite slow and expensive to train WaveGlow, but it could actually generate audio with close to real-time throughput, and including a full text-to-speech model added many dimensions of control. This was a tool you could iterate with. I found the TTS could be induced to babble by letting it run past the end of its predicted alignment the the text, at which point it would get confused and start jumping around. Finally, I trained a few models on voices from Mozilla's [CommonVoice](https://commonvoice.mozilla.org/en) project to get a much wider range of voice sounds. I built in some extra features to the CLI and got the whole thing running on Stefan's computer using PyInstaller. 

I also developed a small glyph generator which was used in some of the videos -- this took in sounds, extracted features with some machine listening algorithms, and then mapped those features to a set of curves and strokes and stored them as 3D mesh files. 
I traveled to Oslo to install Deviant Chain, setting up the video players and cueing system. I was pretty happy with the results -- it was genuinely spooky working on it with just a few of us in the empty bank basement at night.

<!-- <div class="video-wrapper"> -->
  <!-- <div class="video"> -->
<iframe src="https://player.vimeo.com/video/431684120" width="100%" height="100%" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
  <!-- </div> -->
<!-- </div> -->
