# OpenFOAM Cavity Tutorial

OpenFOAM Version: 6

Ubuntu Version: 18.04

The following tutorial aims to get a beginner linux user up to speed with using OpenFOAM with Ubuntu. A basic Unix primer is provided to help the user get aquainted with using terminal commands. The OpenFOAM walkthrough covers installation of OpenFOAM and the completion of the cavity case using BlockMesh for geometry definition. An alternative meshing approach using gmsh is also presented. 

## Basic Unix Commands

Log into your Ubuntu System. Open a terminal by pressing "cmd + a" (Mac keyboards) or "windows key + a" (Windows keyboards) to open a list of applications installed on your machine. Alternatively, you can press the menu button on the dock as shown below. Note: My icons and theme may be slightly different than yours.

![Ubuntu Applications Menu](./Images/Open_Terminal.jpg)

Scroll down the list until you find the terminal application. You can right click the icon and add Terminal to your favorites. This will place the Terminal icon in your dock for easy access. Open Terminal by clicking the icon in the applications list or clicking it in your dock. A window like the one below will open.


![Terminal Window](./Images/terminal.png)

Terminal allows the user to interact with a program called Bash. Bash is a type of program known as a shell and provides an interface to the system itself. A user can enter text commands to navigate the file system, install software, and do other common tasks using the shell interactively. Bash can also run script files.

### Navigating the File System

The directory system begins at the root directory represented by /. All files on the system exist within this directory. A special directory exists within / called home. The home directory contains directories corresponding to the users of the system. You will have a special directory just for you located at /home/your_username. This is referred to as YOUR home directory (whenever you see someone mention the home directory, they are usually referring to /home/your_username, not /home) and it is used quite often. This is where directories that store items like your Documents, Pictures, Downloads will be located. It is used so often that it has its own special shortcut, the tilde: ~. 

When you open Terminal, the current working directory will be your home directory. The current working directory is displayed as part of the prompt located to the left of your cursor in the terminal window. Your prompt should look something like this:

```your_username@your_computer_name:~$```

The text between the : and the $ is the current working directory. In this case you are currently in your home directory, represented by the tilde. You can also verify this using the pwd command (print working directory). You enter a command by typing its name and then pressing enter. 

```$ pwd```

Dont type the $. The $ signifies the end of the terminal prompt and will be used to indicate that the following line of code is intended to be entered as a terminal command. After typing the command and pressing enter, you should see the location of your home directory printed to the screen. 

![pwd command](./Images/pwd.png)

Note: If you want to paste into the terminal window, you have to use ctrl + shift + v instead of the usual ctrl + v. Similary to copy from the terminal window to the clipboard you must use ctrl + shift + c.

We can list files and directories that exist in the current working directory by typing the ls command (short for list):

```$ ls ```
