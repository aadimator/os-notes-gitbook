# Looking at the Contents
Now that you know where you are, let's move on. We'll learn how to look at the contents of a directory. We'll see which files and directories are located in a particular directory.  
To see the contents of a directory, just enter the following command:
```
    $ ls
```
It will print out the contents of the `cwd` (current-working-directory). This is the default behavior of this command. 

### with arguments 
If you want to find out about the contents of some other directory, besides the `cwd`, you can provide extra arguments to the command, like:
```
    $ ls /usr
```
It printed out the files and directories inside the `/usr` :
```
    bin  games  include  lib  local  locale  sbin  share  src
```
### with flags
You can modify the output or the behavior of the command by using some flags with the command.  
For example, if we issue `ls` in our home directory along with the `-l` flag (for 'long' output), it will list all the files and directories in the 'cwd' with extra details, like
```
    $ ls -l
```
```
drwxr-xr-x 2 aadimator aadimator 4096 اپريل 21 09:23 Desktop
drwxr-xr-x 2 aadimator aadimator 4096 اپريل 21 09:23 Documents
drwxr-xr-x 2 aadimator aadimator 4096 اپريل 26 06:35 Downloads
drwxr-xr-x 2 aadimator aadimator 4096 اپريل 21 09:23 Music
drwxr-xr-x 3 aadimator aadimator 4096 اپريل 21 17:35 Pictures
drwxr-xr-x 2 aadimator aadimator 4096 اپريل 21 09:23 Public
drwxr-xr-x 2 aadimator aadimator 4096 اپريل 21 09:23 Templates
drwxr-xr-x 2 aadimator aadimator 4096 اپريل 21 09:23 Videos

```
Here, a lot of extra information was provided along with the names of the files and directories.  
Similarly, to show all the hidden files and directories in 'cwd', you can pass this flag :
```
    $ ls -a
```