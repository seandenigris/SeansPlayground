## Notes ##
  * "In the future, sprouting will cause the contents box to detach and smoothly grow into the full object; a contents box will be just like a condensed form of an object." (1, 127)
  * In ARK [9, 10], for example, objects have mass and velocity, and obey such physical laws as gravity and inertia (1, 129)
  * The ideal is for the notion of an interface to vanish completely, to be replaced by a portal through which the user enters an artificial world populated by the objects at hand. (1, 130)
  * Examine slots that reference the object
  * Experiment more natural interface than buttons and menus
  * What does it look like to view only the exterior e.g. public slots?
  * Pose = saved geometrical layout of objects; can be reconstructed later; but still preserve "each object only once in the world"
  * No Run vs. Edit distinction - composing a UI and using an application are the same (2)
  * Morph disassembly requires design discipline: "In particular, morphs need to be built without assuming anything in particular about embedding relationships… [that they](so.md) can keep running even when disassembled" (2)
  * object-focused model
    * What - attempts to foster the notion that objects themselves are directly available for interaction (3)
    * Tools - recast as organizers and coordinators of multiple objects, rather than as repositories for remote views of objects

## Principles ##
  * Availability - achieved via object-centricity, frees the programmer from modes in which limited portions of object functionality are available at any one time because, rather than centralizing functionality into a monolithic tool, smaller chunks of functionality are coupled to the object (3)
  * Primacy - the programmer must go to the object to get at its properties and behavior, because they are properly owned by the object (3)
  * direct engagement (3)
    * What: a sense of immediacy with the semantic objects of interest
    * When: the offered concrete manifestation is easier to embrace than an abstract one, and the object is at hand to be examined and manipulated
    * Why: This identification encourages programmers to feel as if they are directly dealing with the objects of the language
  * immediacy - a concrete representation that the  user accepts as the object itself (3)

## Implementation ##
  * abstractWindowCanvas has:
    * #boundingBoxInWorld - the part of the world it is focused on
    * #boundingBoxOnScreen - its absolute coordinates

## Ideas ##
  * Sometimes you really do want to have a token representing the object instead of the actual object. For example, I'm trying to understand the execution of a complex system. I want to see the object in the context of the call chain, but when I open it somewhere else, I don't want it to disappear and be dragged somewhere else. What I want is a stand-in. Like a baseball card. Everyone knows that it is not the real player, but it depicts them as relevant to a particular context.
  * Open a new World to work on display code, so if that world stops, the system doesn't crash. When a World stops running, Self also brings up a debugger in a separate window - damn that's better than the emergency evaluator! (2)

## Questions ##
  * Q: Why does gasTank have methods copied from the trait? e.g. addAtom appears in both places

_Answered_
  * Q: How does one create a button on a method taking an argument? A: The same way as unary message. There will be a text field to type in the argument
  * Q: How to set the receiver of the message? A: Can be done via the outliner. There is a 'Set target' button, but I'm waiting on a ml question on its use

## Future Research ##
  * Self
    * Objects have personality (4). I've thought about this often. Maybe the Debugger's token looks like an exterminator van. There was a cool demo, I think in ARK of a mail truck delivering an email. Maybe an inspector on 1 plays "one is the loneliest number" in the background. Of course, these could get very annoying. But maybe simpler things like different colors, although then you run into the "Squeak is a toy" criticism… the fact that programming has to be so serious is a smell in itself; secure people can laugh at themselves
  * Other: Garnet, ThingLab, Reno, SUIT UI Builder (2)

## References ##
  1. Experiencing Self Objects
  1. The Self-4.0 User Interface: Manifesting a System-wide Vision of Concreteness, Uniformity, and Flexibility
  1. Getting Close to Objects: Object-Focused Programming Environments
  1. Experiencing SELF Objects: An Object-Based Artificial Reality