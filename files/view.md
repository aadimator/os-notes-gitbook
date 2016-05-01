# View the File
You can view the contents of the file by using either `cat` or `less` command. The difference between these two is that `cat` just prints out all the contents of the file on the terminal while `less` command give you extra control over the content like scrolling etc.

## Using `cat`
You can view the contents of the file by using the `cat` command like this:
```
    $ cat file1
```
This will print out all of the text from "file1" onto the terminal. You can specify multiple files also:
```
    $ cat file1 file2 file3
```
This will print out all of the text from all the files, in order, i-e "file1" will be displayed first, immediately followed by "file2" and then by "file3".  
Usually `cat` is used when we know that the content is not that long. Otherwise, it feels so overwhelming and it's very difficult to find the required information from a long list of text.

## Using `less`
When the content of the file is long and we need extra functionality like scrolling and searching, we use the `less` command. It's syntax is exactly the same as that of `cat` command:
```
    $ less file1
```
This will open "file1" in a new interactive environment. Here, you can scroll up and down using the arrow keys. You can also search for a word by pressing `/` and typing the word that you want to find. After that, press `Enter` and it will find that word in the current open file. You can cycle through the found words using `n` for "next" word and `p` for "previous" one. To **quit** this interactive environment, press `q` and you will be returned back to the terminal.

Just like `cat` command, you can also specify multiple files:
```
    $ less file1 file2 file3
```
This will first open the "file1" and after you quit it, it will open the next open, i-e "file2", and so on.