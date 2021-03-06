# Create a new Directory
If you are tired of just roaming around the Linux, and eager to create something yours, I've got just the right tool for you. Let me introduce you to the `mkdir` (stands for (can you guess it?) make-directory). Here's how to use it:
```
    $ mkdir Test
```
This will create a new directory named "Test" in the `cwd`. It's as simple as that. You just have to provide the name of the directory that you want to create and it will create it for you and place it in the `cwd`.

You can specify multiple directory names as arguments and it will create all those directories for you in the `cwd`.
```
    $ mkdir Dir1 Dir2 Dir3 Dir4 Test1
```
This command will result in all the above specified folders being created in the `cwd`.

You can also specify a path where you want to create the directory. For example:
```
    $ mkdir Downloads/Test
```
This will create a new directory names "Test" inside the `Downloads` directory which in turn is inside the `cwd`.