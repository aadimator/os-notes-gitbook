# Directory
You already know what a Directory is, believe me. In Linux, **folders** are known as Directories. Following are some of the most important directories:

## Root Directory ( / )
Everything on your Linux system is located under the root ( / ) directory. You can think of it as C:\\ drive in Windows but there are some significant differences between the two. For example, in Windows, another partition would be located at D:\\ but in Linux, it will appear under the root ( / ) directory. If I mount a USB drive to the PC, it will also appear under the root. So, when I say everything is located under root ( / ), I mean **everything**.

## Home Directory ( ~ )
Home directory contains a home folder for each user. It is usually represented by ( ~ ). This home folder contains user specific data files and configuration files, just as in Windows, there are separate folders for each user in C:\\user where user stores Documents, Pictures, Downloads etc.  
For example, if I am a user in Windows, the path to my Downloads folder will be something like C:\\user\\Aadam\\Downloads, but in Linux, it will be /home/Aadam/Downloads. Similarly, if there is another user, his path to Downloads folder will be something like C:\\user\\OtherUser\\Downloads in Windows and /home/OtherUser/Downloads in Linux. That way each user has a separate Downloads folder and one user can't access the Downloads folder of the other user.

## Current Working Directory ( . )
This is a relative term. It represents the directory that you are currently working in. If we think in terms of Windows, this represents the folder that is currently open in Windows Explorer, the folder that we are currently working in.