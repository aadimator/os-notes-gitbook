# Basic Linux Concepts

## Basic Terminology

### Terminal
Terminal is a command-line-interface (CLI) where you write commands which are then executed by the operating system. It is equivalent to the Command Prompt in Windows but in the Linux world, it is a first-level citizen, meaning that most of the time we use terminal (writing commands) to do tasks instead of GUI (clicking and dragging). This is very fast as compared to GUI and  gives the user more control over what he can do. It has a steep learning curve for those who are accustomed to the GUI way of doing things, but when you do master it, it's a really valuable skill to have in your arsenal, which makes you more productive and also it looks really cool because all the hardcore programmers and hackers use it in the movies.

### Directory
You already know what a Directory is, believe me. In Linux, **folders** are known as Directories.
#### Root Directory ( / )
Everything on your Linux system is located under the root ( / ) directory. You can think of it as C:\\directory in Windows but there are some significant differences between the two. For example, in Windows, another partition would be located at D:\\ but in Linux, it will appear under the root ( / ) directory. So, when I say everything is located under root ( / ), I mean **everything**.
#### Home Directory ( ~ )
Home directory contains a home folder for each user. It is usually represented by ( ~ ). This home folder contains user specific data files and configuration files. This is just like as in Windows there are separate folders for each user in C:\\user where user stores Documents, Pictures, Downloads etc.  
For example, if I am a user in Windows, the path to my Downloads folder will be something like C:\\user\\Aadam\\Downloads, but in Linux, it will be /home/Aadam/Downloads. Similarly, if there is another user, his path to Downloads folder will be something like C:\\user\\OtherUser\\Downloads in Windows and /home/OtherUser/Downloads in Linux. That way each user has a separate Downloads folder and one user can't access the Downloads folder of the other user.
#### Current Working Directry ( . )
This is a relative term. It represents the directory that you are currently working in.

## The Command Prompt
When you first open the terminal, you are greeted with a cryptic looking command prompt like this :

    aadam@my-pc:~$

Although, this can be customized by the user, this is the default Command Prompt in Ubuntu.
Now, let's break it down:

- `aadam` name of the current user
- `my-pc` the name of the system you are running it on
- ` ~ ` You already know what this is ( Hint : cwd ) In this case, it is /home/aadam
- ` $ ` The prompt symbol. This denotes the end of the command prompt, your input will appear after this.

From now on, instead of writing the whole command prompt as shown above, I will only display the prompt symbol to indicate the commands.

    $ some command

## Executing Commands
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

## Wrap Up
Now you have learned about the basics of the Linux terminal ( and some basic commands), you should have a good foundation for expanding your knowledge of Linux commands. In the next tutorial, we will learn how to navigate, view and edit files.

If you have any questions, feel free to ask in the comments.
