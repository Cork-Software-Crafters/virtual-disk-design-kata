#Virtual disk design kata
##Requirements
* A Directory has a name and stores File(s). It can add and delete files, and get all files.
* A File has a name (a string) and a size (an int).
* Directories can contain File(s) but also Directory(s). So generalize both as Resource(s).
    * Did you use Composite pattern?
* Storage should implement ```int totalSize();```.
* Storage should implement ```int totalMP3()```. A file which name finishes with “mp3” is an MP3.
    * Did you consider Visitor pattern or domain service? Did you implemented it in Directory?
* We need to allow zip files.

##Concepts to discuss
###Composite pattern
* Structural component
* Composite should be used when clients ignore the difference between compositions of objects and individual objects. If programmers find that they are using multiple objects in the same way, and often have nearly identical code to handle each of them, then composite is a good choice; it is less complex.
* Variant: As it is described in Design Patterns, the pattern also involves including the child-manipulation methods in the main Component interface, not just the Composite subclass.

###Visitor pattern or domain service
* When should a logic that processes a structure be coded in the structure itself? When should it be coded separately?

* Approaches:
    * GOF's Visitor
        * The visitor design pattern is a way of separating an algorithm from an object structure on which it operates. A practical result of this separation is the ability to add new operations to existing object structures without modifying those structures.
    * DDD domain service