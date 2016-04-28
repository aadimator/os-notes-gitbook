# File Manipulation
Up until now, we've been working with directories only, how to create them, delete them etc. Now, we'll turn our focus towards the Files and learn how to create them, delete them, copy them, edit them etc. So without further ado, let's get started.

## File Creation using `touch`
Imagine if you're like a wizard and could create anything by just touching with your wand. Well in Linux, you are. You could create any file by just giving the `touch` command and specifying the name of the file that you want to create.
```
    $ touch file
```
This will create a new empty file in the `cwd`. You can specify multiple file names and it will create multiple files with the given names.
```
    $ touch file1 file2 file3
```
In this case, three files will be created named file1, file2 and file3 respectively. They'll all lie in the `cwd` unless specified otherwise.

## Removing a File using `rm`
You can easily delete a file by using the `rm` command and giving it the name(s) of the file(s) you want to remove. `rm` stands for "remove", obviously.
```
    $ rm file1
```
This will remove the file1 from the `cwd`. It will be gone permanently. There's no Undo button so be extra careful when using this command. Otherwise, you may shoot yourself in the foot.  
You can specify multiple files like you did in the `touch` command. If you give a wrong filename, an error will be returned specifying that there is no file or directory with that name.

## View the File using `cat` or `less`
You can view the contents of the file by using either `cat` or `less` command. The difference between these two is that `cat` just prints out all the contents of the file on the terminal while `less` command give you extra control over the content like scrolling etc. and only shows the content that can fit on your screen. You can use the "arrow keys" to navigate inside the file and press `q` when you want to quit.
```
    $ cat file1

    $ less file1
```

## Copying Files using `cp`
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

## Moving with `mv`
When using `cp`, it will copy the file; the original file will remain intact. But when we're moving a file, it'll be like "cut-paste". It's syntax is just like `cp` command, only replace `cp` with `mv` which stands for .......
```
    $ mv path/to/source path/to/dest
```
For example, if I want to move `file1` from `Documents` to `Downloads` directory, I will issue a command like this from my home directory:
```
    $ mv Documents/file1 Downloads/
```
This will "cut" the `file1` from `Documents` directory and "paste" it in `Downloads` directory. Just like `cp` command, you can specify the name of the file for the Destination folder. If there's already a file with the same name, then it will be replaced with the moved file.  
`mv` command is also used for renaming the files. For example
```
    $ mv hello bye
```
This will rename the file named `hello` to `bye`. If you think about it, it cuts the previous file named `hello` and pastes that file with a new name `bye`, which results in the file renaming. Neat, isn't it?