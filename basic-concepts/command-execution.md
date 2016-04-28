# Executing Commands
You can execute commands by typing them after the command prompt. There are many standard Linux commands and utilities that are installed with the OS, that allow you to navigate the system, install software packages and configure system and applications.  
It is important to note that almost everything in Linux is case-sensitive including file and directory names, commands, arguments, flags etc. So, if something is not working the way it should, double check the spelling and case of your commands.

### Without Arguments or Options
To execute a command without any arguments or options, simply type the command in the command prompt and hit `Enter`.
If you run a command like this, it will exhibit its default behavior. For example, Try running this in the command prompt :

    $ ls

This will print a list of file and directories in the current directory. This is the default behavior of the `ls` command.

### With Arguments
Most of the commands accept arguments or parameters, which can affect the behavior of a command. Try running this command:

    $ ls /usr/bin

Did you notice anything different? Yeah, you're right. This time it printed the list of files and directories in the /usr/bin directory. So, instead of printing the list of files in the current working directory, which is the default behavior of the 'ls' command, when we give an argument to the command, it will print out the list of files in the directory provided to it as an argument.

### With Options
Most of the commands accept options, also known as flags, that modify the behavior of the command. They are special arguments, and are indicated by a single `-` followed by one or more options, which are represented by one or more upper- or lower-case letters.  

For example, these are some of the most used options that are used with `ls` :

- `-l`: print a 'long-listing' which includes extra details such as permissions, ownerships, file size etc
- `-a`: lists *all* of a directory's files including hidden ones

To use `l` flag with 'ls', use this command:

    $ ls -l

You can also combine multiple flags like this:

    $ ls -l -a

or this :

    $ ls -la

Whichever way you feel comfortable. I personally prefer the second one.
### With Arguments and Options
Options and arguments can almost always be combined, when running commands.

For example, you can always check the contents of `/home` regardless of your current working directory, by running this `ls` command:

    $ ls -la /home

Here, `ls` is the command, `-la` are the options and `/home` is the argument that indicates which file or directory to list.