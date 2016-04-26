# Navigation
To work in a new environment, the most necessary skill in order to survive is to learn how to navigate that environment. If you are unable to do so, you won't be able to do anything else. You'll always feel like a mouse trapped in a maze. So, now we'll look at some of the basic commands for navigation in the Linux operating system.

## Finding where you are : pwd
Imagine that you moved into a new city and you don't know anyone else there. You don't know any of the maps and directions and there are no board signs either to guide you. Well that'll be the case if you've never used Linux before and you migrated from another OS like Windows. The very first thing that you'll need in order to survive in this new city is to get a sense of where you are. Whenever you feel like you are lost in the directories, you can easily find out about the directory that you are currently in. Imagine that. You won't have to go knocking on someone's door asking them about where you are. You'll just have to write a simple command in the Terminal and you'll immediately know where you are. Isn't that cool? Okay, no further delay. Let's reveal the magic spell, shall we?
```
    $ pwd
```
Yeah, just that. Just type `pwd` in the Terminal and you'll know where you are. In case you're wondering, `pwd` stands for `print-working-directory`.

## Looking at the Contents : ls
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
## Let's move somewhere else with 'cd'
You can easily move from one directory to another by using the `cd` command (stands for 'change directory'). For example, let's say I'm in my 'home' directory. Now to see where I can go, I'll type the `ls` command and see all the directories that I can go to.
```
    $ ls
```
It returned the following directories:
```
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
```
Now, let's say I want to go into my 'Downloads' directory. To do that, I'll just have to type:
```
    $ cd Downloads
```
and that's it. It'll change my 'cwd' to Downloads. Now if I execute the `ls` command, it'll shown the list of content present in the 'Downloads' folder. Here we provided the argument as a **relative path**, because we were referring to the folder (Downloads) relative to the `cwd`.  
The other way is to use **absolute path**. In this method, we provide the full path of the directory that we want, regardless of the `cwd`. For example, 
```
    $ cd /usr/bin
```
Here we are providing the full path to the "bin" directory that is under "usr" directory, which in return is under the root.

## Let's Create a Directory with mkdir
If you are tired of just roaming around the Linux, and eager to create something yours, I've got just the right tool for you. Let me introduce you to the `mkdir` (stands for (can you guess it?) make-directory). Here's how to use it:
```
    $ mkdir Test
```
This will create a new directory named "Test" in the `cwd`. It's as simple as that. You just have to provide the name of the directory that you want to create and it will create it for you and place it in the `cwd`.
## Let's Delete a Directory with rmdir
Now, where there's construction, the destruction follows. There'll be a time when you want to delete some directory that you accidentally made or no longer need. We got you covered there too. Just say the magic words (or more specifically, type them) and your wish will be granted. 
```
    $ rmdir Test
```
This will find the "Test" directory in the `cwd` and delete it.

## Wrap Up
Now you know how to find where you are in the maze of directories, how to see the content of these directories, how to move from one directory to another, how to create a new directory and how to delete one.  
In the next chapter, we'll see some commands to work with files.