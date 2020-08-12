# Virtual storage design kata
## Requirements reminder
* A Directory has a name and stores File(s). It can add and delete file(s).
* A File has a name (a string) and a size (an int).
* Directories can contain File(s) but also Directory(s). So generalize both as Resource(s).

## Did you consider...
* Have you create a Resource following the **Composite pattern?**

![Composite pattern](https://github.com/liopic/virtual-disk-design-kata/raw/master/summary/CompositePattern.png)

## Requirement 3
* We need to know the total size our virtual storage is using.
    * So add the following method to Storage: ```int totalSize();```

## Next Requirement
* [Requirement four](../requirement-4/README.md)
