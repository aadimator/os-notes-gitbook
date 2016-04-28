# Moving with `mv`
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