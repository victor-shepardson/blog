<!--
.. title: Bear Cult and HOFSTADTERPILLAR
.. slug: bear-cult-and-hofstadterpillar
.. date: 2018-04-19
.. tags: animation, visual, sonic, joseph campbell, douglas hofstadter, jodie mack, aftereffects, bear cult, hofstadterpillar, feedback, max
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

These are two animations I made for FS35 with Jodie Mack in winter 2015.

## Bear Cult

*Bear Cult* was inspired by a collection of Joseph Campbell's essays I found in a used book store, specifically one entitled "Renewal Myths and Rites of the Primitive Hunters and Planters". It's about the prehistoric origins of myth. In Campbell's telling, the purpose of myth is to conquer death. Campbell cites preserved arrangements of cave bear bones as evidence for the ancient roots of a bear-baiting ritual still practiced by indigenous peoples in northern Japan. In the bear-baiting ritual, a young bear is captured, raised in captivity, and then ritually tormented, killed and eaten. The bear is believed to contain the soul of a demigod which yearns to be released from its fleshy bear-prison. For Campbell, this is the coping mechanism of an animal which kills to survive but understands death. It's the hunter's moral justification for killing: death isn't terminal, killing is a kindness. Ritualized death is a point of contact with the numinous; the fear of death is transmuted to awe. I found the deep connection Campbell makes between this sacred feeling and human capacity for cruelty heartbreaking.

I decided to depict a bear-baiting ritual. Not the specific cultural practice Campbell recounts, but the abstracted elements of a hypothetical prehistoric bear cult. The body of the bear would be made by hand with paper drawings and cutouts, while the soul would be made in software with [virtual video feedback](../video-feedback). These material and digital components would interact via fluorescent orange paper which could be keyed out in video editing software. A possible alternate title: "Mind-Body Chromakey". Originally I had storyboarded a longer narrative including human hands and spears piercing the bear and the escape of its soul, but only part proved feasible in the time I had.

I'm happy with how the bear soul material turned out. After shooting the paper animation, I exported just the key as a binary mask. As an input to the feedback process, the mask lets the roiling cloud-forms conform to the geometry of the bear eyes and nose-hole. Unfortunately the black-on-black paper was unwise; there's a lot of camera noise after adjusting the levels to make everything visible. A darker background of black felt or something might have worked better.

This project taught a lesson about how sound influences the perception of time in film. What felt like a good visual rhythm when I was silently animating seems weirdly abbreviated with the soundtrack added. The sound was a bit rushed, but I like the general effect. It's some recordings of bear vocalizations and carcass-mangling sounds chopped up into phase-rhythms with the same methods I used for [SIBA](../siba). I'd like to revisit this project someday.

<div class="video-wrapper">
  <div class="video">
    <iframe src="https://player.vimeo.com/video/199104868" width="100%" height="100%" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
  </div>
</div>

## HOFSTADTERPILLAR

*HOFSTADTERPILLAR* is a many-looped negotiation between rules, materials and intuition, an effort to explore Hofstadter's idea of [strange loop](https://en.wikipedia.org/wiki/Strange_loop) by drawing.

Drawing is an act of alternating abstraction and reification, recognition and construction of forms among materials. I draw, I see what I have drawn, I draw more. Animating by hand can be seen as a sort of [image feedback loop](../video-feedback); each frame is drawn with reference to previous frames, which are visible beneath transparent cels. I developed loose sets of rules to draw by, of the type "a silver line extends and curves more each frame". Other rules emerge from the materials; paint markers pool and smear when the next cel is placed on top. I used the "maximum cycle" technique of repeatedly drawing new material into the same set of frames to construct rich and evolving loops. The sound is another set of feedback loops, a Max doodle with chaotic noise generators stimulating banks of tuned filters.

<div class="video-wrapper">
  <div class="video">
    <iframe src="https://player.vimeo.com/video/121756116" width="100%" height="100%" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
  </div>
</div>
