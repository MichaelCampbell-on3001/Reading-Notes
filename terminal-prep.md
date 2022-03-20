# Practice in Terminal

- [The Command Line](https://ryanstutorials.net/linuxtutorial/commandline.php) - **Question** What is it, how does it work and how do I get to one?**Amswer** A command line, or terminal, is a text based interface to the system. A user is able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text.

- [Basic Navigation](https://ryanstutorials.net/linuxtutorial/navigation.php) - An introduction to the Linux directory system and how to get around it.

---

Terminal Command : Description 

**pwd**: Print Working Directory - displays directory user is currently in.

**ls**: list- lists files in working directory 

**~**: shortcut for your home directory

**.(dot)**: a reference to your current directory

**..(dotdot)**: a reference to the parent directory.

**cd**: use this command to change directories

___

- [More About Files](https://ryanstutorials.net/linuxtutorial/aboutfiles.php) - Find out some interesting characteristics of files and directories in a Linux environment. 

    **Fun Facts about files and directories in Linux** 
- Linux is case sensitive
- Spaces in file and directory names are perfectly valid. This can be achieved by using quotes or escape characters.
- You don't even need a special command or action to make a file hidden. If the file or directory's name begins with a . (full stop) then it is considered to be hidden.
-  Everything is a file under Linux
Even directories.
- Linux is an extensionless system
Files can have any extension they like or none at all.
- Linux is case sensitive
Beware of silly typos.


___




- [Manual Pages](https://ryanstutorials.net/linuxtutorial/manual.php) - Learn how to make the most of the Linux commands you are learning.
- You invoke the manual pages with the following command: 

`man <command to look up>`

- To exit the man pages press 'q' for quit.

- To do a keyword search on the Manual pages use the command 

`man -k <search term>`



---

- [File Manipulation](https://ryanstutorials.net/linuxtutorial/filemanipulation.php) - How to make, remove, rename, copy and move - files and directories.
- Make a new directory: 

`mkdir [options] <Directory>`
- Remove a directory: 

`rmdir [options] <Directory>`

- Create a new directory:

`touch [options] <filename>`

- Copy a fie or directory:

`cp [options] <source> <destination>`

- Move a directoy or file:

`mv [options] <source> <destination>`

-Remove a file or directory:

`rm [options] <file>`

**The Linux command line does not have an undo feature. Perform destructive actions carefully.**


- [Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php) - A quick reference for the main points covered in this tutorial.