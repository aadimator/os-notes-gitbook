# File Creation using `touch`
Imagine if you were a wizard and could create anything by just touching it with your wand. Well in Linux, you are. You could create any file by just giving the `touch` command and specifying the name of the file that you want to create.
```
    $ touch file
```
This will create a new empty file in the `cwd`. You can specify multiple file names and it will create multiple files with the given names.
```
    $ touch file1 file2 file3
```
In this case, three files will be created named file1, file2 and file3 respectively inside the `cwd`.

To create file somewhere other than the `cwd`, you can provide the path of the directory in which you want to create the new file.
```
    $ touch Downloads/file1 Downloads/file2
```
This will create "file1" and "file2" inside the Downloads folder which is under the `cwd`. This, in effect, is a relative path as we are specifying a folder ("Downloads") relative to the `cwd`.  
You can also give the absolute path like this:
```
    $ touch /tmp/file1
```
This will create an empty file named "file1" inside the `tmp` directory which is under the `root` directory, no matter where you are.

