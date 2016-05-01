# Delete an Empty Directory
Now, where there's construction, the destruction follows. There'll be a time when you want to delete some directory that you accidentally made or no longer need. We got you covered there too. Just say the magic words (or more specifically, type them) and your wish will be granted. 
```
    $ rmdir Test
```
This will find the "Test" directory in the `cwd` and delete it.

There's one catch though, you can only delete those directories that are empty, using this command. If you try to delete a directory that isn't empty by using `rmdir`, an error similar to this one will be shown:
```
    rmdir: failed to remove ‘Downloads’: Directory not empty
```
Deleting non-empty directories is covered [here](files/remove.md).