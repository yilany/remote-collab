# Cloning a Repository

Have you found a cool project on Github and you want to contribute to it, but doing so entails more than just editing a text document using the Github user interface? If so, you will need to clone the project so that you can work on it locally.

In this tutorial, we will walk you through how to do so.

## Table of Contents

0. [Prereqs](#prereqs)
1. [Setting the Scene](#setting-the-scene)
2. [Cloning a Repository](#cloning-a-repository)

## Prereqs

- You are reading this on a computer with a keyboard of some sort
- You have [Git installed and configured](InstallGit.md)
- You have the `Terminal` application or an equivalent command line interface installed

## Setting the Scene

Before we can clone the repository we want to work on, we need make sure we are going to put in a nice location. To do so, we will do some shell scripting.

Let's start by opening up the `Terminal` application (or your favorite shell interface). You should see something like this:

![Empty terminal](img/empty_terminal.png)

_Your terminal should most likely not say `bean@Jamess-Mac-mini`, it may be a different color, etc._

Type in the following and then press **return** or **enter**:

	ls
	
_You can copy and paste or manually type that command into the `Terminal`._

You have just _run_ the "list directory contents" _command_. It should have dumped a list of files and directories of your home directory.

For another way to get a sense of your environs, run the following command:

	pwd
	
In this case, `pwd` stands for "print working directory". Running this command should result in a display the name of your home directory. It should look familiar.

If you don't have any prior experience with working in the shell, try running the following command:

	open .
	
This will open up the current working directory in the `Finder` application.



## Cloning a Repository






Next, copy-and-paste or type-by-hand the Github url of the repository you would like to work on.