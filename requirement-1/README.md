#Virtual disk design kata
##Requirement 1
* User can store files in this virtual disk.
* We are not going to move/save any file; just store file's name and size.

A base interface for this virtual disk could be:
```
interface StorageInterface
{
   public Directory rootDirectory();
}
```
That is, the method rootDirectory will return the base Directory "/".
* A Directory has a name and stores File(s). It should allow to add a file, delete a file and get all files (getting an array of File).
* A File will be created with a name (a string) and a size (an int).

##Next Requirement
* [Requirement two](../blob/master/requirement-2/README.md)