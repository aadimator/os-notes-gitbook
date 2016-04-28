# Copying Files using `cp`
To copy file from one place to another, execute the following command:
```
    $ cp path/to/source path/to/dest
```
This will copy the file specified in source to the destination. For example, if I want to copy `file1` from `Documents` directory to the `Downloads` directory, I'll execute the command like this:
```
    $ cp Documents/file1 Downloads/
```
This will copy `file1` from `Documents` directory to the `Downloads` directory and save it with the original name i-e, in this case, `file1`.  
We can specify the name of the file too, like this:
```
    $ cp Documents/file1 Downloads/newName
```
This will copy the `file1` from the `Documents` directory and save it as `newName` in the `Downloads` directory. If there's already a file with that name in the "destination" directory, it will be replaced with the copied file. 
