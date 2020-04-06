# Cloning a Repository

Have you found a cool project on Github and you want to contribute to it, but doing so entails more than just editing a text document using the Github user interface? 

In this tutorial, we will walk you through how to clone a remote repository project so that you can work on it on your own machine.

![Wallace and Gromit Clone Dog](https://media.giphy.com/media/9x6fPJVGpq9HO/giphy.gif)

## Table of Contents

0. [Prereqs](#prereqs)
1. [Preparing to Clone](#preparing-to-clone)
2. [Cloning a Repository](#cloning-a-repository)

## Prereqs

- You are reading this on a computer with a keyboard of some sort
- You have [Git installed and configured](InstallGit.md)
- You have the `Terminal` application or an equivalent command line interface installed

## Preparing to Clone

Before we can clone the repository we want to work on, we need make a nice home for it. Using the `Terminal` (or your favorite shell interface), [navigate to a directory of your choice](GettingAroundShell.md) and [create a new directory](ModifyingContentsShell.md) with the name of your choosing. Change into your nascent directory.

## Cloning a Repository

In the directory, run the following command:

	git clone https://github.com/learninglab-dev/remote-collab

This will copy the entirety of the contents of this repository into your current working directory. `cd` into the cloned repository and feel free to poke around!

Try the following:

	git log
	
This will display the history of all of the changes made to the repository, when they are made, and who made them.

*In order to clone a repository other than this one, just replace the URL in the `git clone` command above with the URL of your desired repository.*