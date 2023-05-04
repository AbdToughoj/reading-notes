1.**The Command Line:** What is it, how does it work and how do I get to one\.

- What is the Command Line: A command line, commonly referred to as a terminal or shell, is a text-based user interface that enables one to type instructions to communicate with an operating system (OS) on a computer. A command line requires users to input text-based instructions to carry out operations like accessing the file system, running applications, and managing system settings instead of utilizing a graphical user interface (GUI) with icons and menus.
- How does it work: The operating system interprets and executes the user's text commands once they are entered into a terminal or console using the command line. The user's input is generally followed by a prompt, which is a special character that shows the system is prepared to take a command, in a command line interface.
- You can open the terminal by following these steps:

If you're on a Mac then you'll find the program **Terminal** under **Applications -> Utilities**. An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up.

If on Linux then you will probably find it in **Applications -> System** or **Applications -> Utilities**. Alternatively you may be able to 'right-click' on the desktop and there may be an option 'Open in terminal'.

If you are on Windows and intend to remotely log into another machine then you will need an SSH client.

**2)Basic Navigation:** An introduction to the Linux directory system and how to get around it.

On a Linux system, directories and files are arranged hierarchically using the Linux directory system. The root directory, indicated by a forward slash (/), is at the top level and contains all other files and directories.

In Linux, you can use the "cd" (change directory) command and the directory name you want to go to to navigate through the file system. To access the "user" directory inside the "home" directory, for instance, type "cd /home/user".

The "ls" (list) command can be used to display a directory's contents in a list. The "-l" flag will display more details about each file or directory, such as the owner, size, and permissions.

Other significant folders in Linux, besides the root directory, are the "bin" directory, which houses crucial system binaries, the "etc" directory, which houses system configuration files, and the "home" directory, which houses user home directories.

3)**More About Files**: Find out some interesting characteristics of files and directories in a Linux environment.

Linux is an Extension less System : On most systems, a file's type is indicated by a set of characters that follow a full stop at the end of the file; however, on Linux, the system disregards the extension and instead determines the file type based on its contents. On Linux, for instance, a file with the name "myself.png" can still be identified as an image file even after being renamed to "myself.txt". Because of this, figuring out the file type can be difficult, however the Linux "file" command can be used to do so.

Linux is Case Sensitive:This is crucial and frequently causes issues for Linux newcomers. When referring to files, other systems, like Windows, don't care about case. This is not how Linux works. As a result, it is conceivable for there to be two or more files and directories with the same name but different case of the letters.

Spaces in names: Although they are perfectly acceptable, spaces in file and directory names require a little extra care. As you probably recall, we separate objects on the command line with spaces. They allow us to recognize each command line argument and determine the name of the program.

4)**Manual Pages:** Learn how to make the most of the Linux commands you are learning.

"Man pages," also referred to as "manual pages," are documentation files that offer in-depth details about the many commands, utilities, and functions accessible on a Linux system. By typing "man" and the name of the command or utility you wish to learn more about in the terminal, you can access them. For instance, by typing "man ls," the "ls" command's manual page, which details its usage, parameters, and examples, will be displayed. For information on how to use and communicate with the various components of a Linux system, manual pages are a crucial resource. Users can more easily comprehend and make use of the functionality of the commands and tools accessible on their system because of the detailed information and examples they provide.

5)**File Manipulation**: How to make, remove, rename, copy and move files and directories.

- Making a file: To create a new file, use the "touch" command followed by the name of the file.
- Making a directory: To create a new directory, use the "mkdir" command followed by the name of the directory.
- Removing a directory: To delete a directory, use the "rmdir" command followed by the name of the directory.
- Removing a file: To delete a file, use the "rm" command followed by the name of the file.
- Renaming a file: To rename a file, use the "mv" command followed by the old file name and the new file name.
- Copying a file: To copy a file, use the "cp" command followed by the name of the file and the name of the new file.
- Moving a file: To move a file to a new location, use the "mv" command followed by the name of the file and the new location.

  6)**Cheat Sheet:** In the cheat sheet you can find quick reminder for the main concepts involved in using the command line.

Cheat sheet link: https://ryanstutorials.net/linuxtutorial/cheatsheet.php
