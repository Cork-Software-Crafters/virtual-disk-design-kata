# Virtual storage design kata
## Requirements reminder
* A Directory has a name and stores File(s). It can add and delete file(s).
* A File has a name (a string) and a size (an int).
* Directories can contain File(s) but also Directory(s). So generalize both as Resource(s).
* Storage should implement ```int totalSize();```.
* Storage should implement ```int totalMP3()```. A file which name finishes with “mp3” is an MP3.

## Did you consider...
* While implementing totalMP3(), did you use a **Visitor pattern**? Maybe a DDD's domain service? Or did you implemented it in Directory?

![Visitor pattern](https://github.com/liopic/virtual-disk-design-kata/raw/master/summary/VisitorPattern.png)

File and Directory could implement it like: ```public acceptVisitor(ResourceVisitor visitor) {visitor.visit(this);}```

## Requirement 5
* We need to allow zip files.
* They can contain other files, zips and directories.
* The size of a zip file is defined in its creation; that is, zip’s filesize doesn’t depend on its content.

## Summary
* [Summary](../summary/README.md)
