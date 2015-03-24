# Introduction #

The Damn thing was made to be live, concrete, and direct. What's with all the UI Builders??? Morphic IS a UI Builder!!!

# Details #

ImageMorph
  * Initially show a default form, like a grayed out question mark
  * UI facility to change the form or image
    * QUESTION: how do we capture the source of the image with options? I.e. ImageMorph takes a form, but that form may have come from a file, which may or may not be owned by the image. Should we (yuck in advance) save the form in a method? Should we copy the file somewhere? Where?

Use Case:
  1. Drag ImageMorph from toolbox. It displays a default image
  1. Interact with the UI to choose an image from a file, scaling if necessary
  1. Self-like UI to add behavior