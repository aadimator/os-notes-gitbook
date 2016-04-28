# Let's move somewhere else with 'cd'
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
and that's it. It'll change my `cwd` to Downloads. Now if I execute the `ls` command, it'll shown the list of content present in the 'Downloads' folder. Here we provided the argument as a **relative path**, because we were referring to the folder (Downloads) relative to the `cwd`.  
The other way is to use **absolute path**. In this method, we provide the full path of the directory that we want, regardless of the `cwd`. For example, 
```
    $ cd /usr/bin
```
Here we are providing the full path to the "bin" directory that is under "usr" directory, which in return is under the root.
