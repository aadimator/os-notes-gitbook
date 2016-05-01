# Removing a File using `rm`
You can easily delete a file by using the `rm` command and giving it the name of the file you want to remove. `rm` stands for "remove", obviously.
```
    $ rm file1
```
This will remove the file1 from the `cwd`. It will be gone permanently. There's no Undo button so be extra careful when using this command. Otherwise, you may shoot yourself in the foot.  
You can specify multiple files and give relative or absolute paths, like you did in the [touch](files/create.md) command. If you give a wrong file name or a directory name, an error will be returned specifying that there is no file or directory with that name.

## Removing a Directory
Later, we saw how to [remove an empty directory](directories/rmdir.md). Now we'll see how to remove a non-empty directory. To remove a non-empty directory, the same command, i-e `rm`, is used but with one additional flag.
```
    $ rm Downloads -r
```
This will delete the non-empty Downloads directory. All the files and directories inside this "Downloads" directory will be deleted permanently. So, there's no going back. Use this command with caution, because
    With great power, comes great responsibility
The additional flag, `-r`, stands for "recursive". What's happening behind the scenes is, that `rm` command is being applied to all the files in the "Downloads" folder, recursively.