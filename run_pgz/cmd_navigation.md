# Windows Command Window - List of commands for file system navigation

These are the basic commands for setting the directory of your Windows Command window.

When you first open the command window it will probably show the current directory as your user's home directory:

![Command window home](../Images/cmd_home.png)

The text before the ```>``` sign shows your current directory. The part of this text before the ```:``` sign represents the current disk drive.

This prompt indicates the window is focussed on disk drive ```C:``` and a directory called ```Users``` and a *sub*-directory of ```Users``` called after your username.

### Changing the disk drive

Type the letter of the drive you want to change to followed by a colon:

```windows
E:
```

### Changing the current directory to a *higher* level directory

Type ```cd``` for "change directory" followed by two dots to change to the next level up

```windows
cd ..
```

![Command window home](../Images/cmd_cdup.png)

The "prompt string" now shows you are in a higher directory.

### Using ```dir``` to list files and directories

The command ```dir``` is key to using the Command window - it will give you a list of all the files and directories in the location where your command window is currently focussed.

![Using dir in a Command window](../Images/cmd_dir.png)


### Link to an internet tutorial

Here is a link to a short tutorial about navigating through the file system using a Command window:

[https://riptutorial.com/cmd/example/8646/navigating-in-cmd](https://riptutorial.com/cmd/example/8646/navigating-in-cmd)