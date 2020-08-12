# Virtual storage design kata
## Requirements reminder
* A Directory has a name and stores File(s). It can add and delete file(s).
* A File has a name (a string) and a size (an int).
* Directories can contain File(s) but also Directory(s). So generalize both as Resource(s).
* Storage should implement ```int totalSize();```.

## Requirement 4
* As per business request, we need to know how many MP3 files are stored.
    * Implement in Storage ```int totalMP3()```
    * Consider a file is an MP3 if it’s name finishes with “mp3”.

## Next Requirement
* [Requirement five](../requirement-5/README.md)
