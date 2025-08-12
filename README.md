# knulli-rgc-shader-and-bezel-sets
A series of shader and bezel sets intended for use with Knulli/Batocera based on Retro Game Corps recommendations.

Disclaimer: I am not affiliated with Retro Game Corps or Knulli, I just wanted to find an easier way to implement some of the shader and decorations recommended by RGC.

I have been using [Knulli](https://knulli.org/) on several anbernic XX devices as well as a trimui brick and I have slowly come around to accepting the design philosophy that as much configuration should be done in emulation station (es) as possible.  I also started looking at shaders and overlays as a way to enhance the experience and either improve image quality or generate more nostalga.  To that end, I have found [Retro Game Corps guide to shaders and overlays](https://retrogamecorps.com/2024/09/01/guide-shaders-and-overlays-on-retro-handhelds/) very helpful as it goes into great detail about how different shaders will impact the experience, including performance. However, the downsize is that it doesn't really follow the knulli philosophy for using a top down configuration and, instead, disables those configuration settings in es and uses retroarch overrides to implement any changes. This is fine, but a little fiddly, and I wanted to see if I could create some knulli/batocera shader and decoration sets that would make it easy to apply (most) of the RGC recommended configurations directly in es and have them just automatically apply to the various emulators.

This is very much a work in progress and has not been tested for every emulator in every configuration.  I also realize that these types of configuration options are strongly tied to personal preference, but I wanted a way for someone using knulli to be able to quickly try applying one set of recommended settings as trying to navigate the existing options can be a little overwheming. 

This is an attempt to go a step beyond the [RGC overlay pack](https://github.com/retrogamecorps/RGC-Overlay-Pack) by directly applying the settings in es.  Currently, the only shader it directly borrows from is pixel_aa_fast from retroarch as the others in the RGC pack have arleady made their way into the knulli image.  I believe that pixel_aa_fast will also eventually be included in knulli.  

This adds four shader sets to knulli:
* sharp-shimmerless: although this shader is now included in knully by default, there is no es shader set for it so this is a quick way to simply apply this shader across the board
* retro-game-corp-720x720: this is an implementation of the recommendations for square display handhelds at the end of the RGC article. (e.g. cubexx)
* retro-game-corp-dramatic-crt: this mostly applies the RGC recommendations for a more nostalgic rendering and does not depend on many bezels.  It is not integer scaled.
* retro-game-corp-normal: this applies RGC's other recommendations, mostly with integer scaling and is very much a work in progress.
