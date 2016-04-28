# Removing a File using `rm`
You can easily delete a file by using the `rm` command and giving it the name(s) of the file(s) you want to remove. `rm` stands for "remove", obviously.
```
    $ rm file1
```
This will remove the file1 from the `cwd`. It will be gone permanently. There's no Undo button so be extra careful when using this command. Otherwise, you may shoot yourself in the foot.  
You can specify multiple files like you did in the `touch` command. If you give a wrong filename, an error will be returned specifying that there is no file or directory with that name.