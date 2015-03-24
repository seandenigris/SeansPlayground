A Morph that plays UI scripts

# Introduction #

Should have all the features one would expect in a media player - fast forward/rewind (both time and logical e.g. next click).

# Details #

We want to have a simulated scalable world in a window.

The idea is to have something like what HandMorphForReplay does, but in a self contained window. The effect would be that there was another World running in a window, where the HandMorphForReplay could carry out a UI script that could be played, sped up, slowed down, rewound - all the actions you would except from a media player.

Unfortunately, starting a World in a window does not seem easy. Most of the time I try it or manually mess with HandMorphs, my image locks up permanently.

I've also had trouble getting the tool to resize. I tried Window -> TransformationMorph -> PasteUpMorph -> MyCoolToolWindow. That seems promising - although I have to open the tool in the world before embedding in the PasteUpMorph. The tool will resize and even interact for a while, but eventually that too seems to lock up the image.

# Requirements #

  * the window feel like a media player e.g. resizing scales its contents proportionally while playback continues
  * recording keeps the full power of the system e.g. one can bring up a world menu inside the window