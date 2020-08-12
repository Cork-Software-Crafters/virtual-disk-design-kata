# Virtual storage design kata
## Requirement 1
* User can store files in this virtual disk.
* We are not going to move/save any real file; just store file's name and size.

A starting class for this virtual disk could be:
```
class Storage
{
   public Directory rootDirectory();
}
```
That is, the method rootDirectory will return the base Directory (with name "/").
* A Directory has a name and stores File(s).
    * It should allow to add and delete a file(s).
* A File will be created with a name (a string) and a size (an int).

## Next Requirement
* [Requirement two](../requirement-2/README.md)
