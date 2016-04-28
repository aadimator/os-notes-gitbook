# File Creation using `touch`
Imagine if you're like a wizard and could create anything by just touching with your wand. Well in Linux, you are. You could create any file by just giving the `touch` command and specifying the name of the file that you want to create.
```
    $ touch file
```
This will create a new empty file in the `cwd`. You can specify multiple file names and it will create multiple files with the given names.
```
    $ touch file1 file2 file3
```
In this case, three files will be created named file1, file2 and file3 respectively. They'll all lie in the `cwd` unless specified otherwise.